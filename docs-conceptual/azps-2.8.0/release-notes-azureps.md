---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/15/2019
ms.openlocfilehash: 0fc897579e8caef999c337303428fd12740c3606
ms.sourcegitcommit: 7839b82f47ef8dd522eff900081c22de0d089cfc
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/14/2020
ms.locfileid: "83386107"
---
## <a name="280---october-2019"></a><span data-ttu-id="4ad1d-103">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-103">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="4ad1d-104">Geral</span><span class="sxs-lookup"><span data-stu-id="4ad1d-104">General</span></span>
* <span data-ttu-id="4ad1d-105">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="4ad1d-105">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="4ad1d-106">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-106">Az.Accounts</span></span>
* <span data-ttu-id="4ad1d-107">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-107">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="4ad1d-108">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="4ad1d-108">Az.ApiManagement</span></span>
* <span data-ttu-id="4ad1d-109">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="4ad1d-109">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="4ad1d-110">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="4ad1d-110">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="4ad1d-111">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="4ad1d-111">Az.Automation</span></span>
* <span data-ttu-id="4ad1d-112">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-112">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="4ad1d-113">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="4ad1d-113">Az.Batch</span></span>
* <span data-ttu-id="4ad1d-114">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-114">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-115">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-115">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-116">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="4ad1d-116">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="4ad1d-117">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="4ad1d-117">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="4ad1d-118">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-118">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="4ad1d-119">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-119">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="4ad1d-120">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="4ad1d-120">Az.DataFactory</span></span>
* <span data-ttu-id="4ad1d-121">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-121">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="4ad1d-122">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-122">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="4ad1d-123">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="4ad1d-123">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="4ad1d-124">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4ad1d-124">Az.DataLakeStore</span></span>
* <span data-ttu-id="4ad1d-125">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="4ad1d-125">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="4ad1d-126">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="4ad1d-126">Az.HealthcareApis</span></span>
* <span data-ttu-id="4ad1d-127">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="4ad1d-127">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="4ad1d-128">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="4ad1d-128">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="4ad1d-129">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="4ad1d-129">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="4ad1d-130">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-130">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="4ad1d-131">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="4ad1d-131">Az.IotHub</span></span>
* <span data-ttu-id="4ad1d-132">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="4ad1d-132">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="4ad1d-133">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="4ad1d-133">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="4ad1d-134">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="4ad1d-134">Az.Monitor</span></span>
* <span data-ttu-id="4ad1d-135">Foram adicionados novos recetores de grupos de ações para New-AzActionGroupReceiver:   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="4ad1d-135">New action group receivers added for New-AzActionGroupReceiver:   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="4ad1d-136">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-136">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="4ad1d-137">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="4ad1d-137">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="4ad1d-138">Os webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-138">Webhooks now supports Azure active directory authentication.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-139">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-139">Az.Network</span></span>
* <span data-ttu-id="4ad1d-140">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-140">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="4ad1d-141">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="4ad1d-141">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="4ad1d-142">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-142">New cmdlets added:</span></span>
        - <span data-ttu-id="4ad1d-143">New-AzIpsecTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="4ad1d-143">New-AzIpsecTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="4ad1d-144">Foram atualizados cmdlets com o parâmetro opcional -TrafficSelectorPolicies</span><span class="sxs-lookup"><span data-stu-id="4ad1d-144">Cmdlets updated with optional parameter -TrafficSelectorPolicies</span></span>
        - <span data-ttu-id="4ad1d-145">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-145">New-AzVirtualNetworkGatewayConnection</span></span>
        - <span data-ttu-id="4ad1d-146">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-146">Set-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="4ad1d-147">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="4ad1d-147">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="4ad1d-148">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-148">Updated cmdlets:</span></span>
        - <span data-ttu-id="4ad1d-149">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-149">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="4ad1d-150">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-150">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="4ad1d-151">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-151">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="4ad1d-152">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="4ad1d-152">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="4ad1d-153">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="4ad1d-153">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="4ad1d-154">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-154">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="4ad1d-155">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-155">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="4ad1d-156">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="4ad1d-156">Az.RedisCache</span></span>
* <span data-ttu-id="4ad1d-157">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-157">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-158">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-158">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-159">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="4ad1d-159">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="4ad1d-160">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-160">Az.Storage</span></span>
* <span data-ttu-id="4ad1d-161">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="4ad1d-161">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="4ad1d-162">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="4ad1d-162">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="4ad1d-163">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="4ad1d-163">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="4ad1d-164">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="4ad1d-164">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="4ad1d-165">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="4ad1d-165">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="4ad1d-166">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="4ad1d-166">Az.StorageSync</span></span>
* <span data-ttu-id="4ad1d-167">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-167">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="4ad1d-168">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="4ad1d-168">Az.Websites</span></span>
* <span data-ttu-id="4ad1d-169">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="4ad1d-169">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="4ad1d-170">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-170">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="4ad1d-171">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="4ad1d-171">Az.ApiManagement</span></span>
* <span data-ttu-id="4ad1d-172">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-172">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="4ad1d-173">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-173">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="4ad1d-174">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="4ad1d-174">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="4ad1d-175">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="4ad1d-175">Az.Automation</span></span>
* <span data-ttu-id="4ad1d-176">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-176">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="4ad1d-177">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="4ad1d-177">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="4ad1d-178">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-178">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-179">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-179">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-180">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-180">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="4ad1d-181">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-181">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="4ad1d-182">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-182">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="4ad1d-183">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-183">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="4ad1d-184">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-184">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="4ad1d-185">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-185">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="4ad1d-186">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-186">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="4ad1d-187">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-187">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="4ad1d-188">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-188">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="4ad1d-189">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="4ad1d-189">Az.DataFactory</span></span>
* <span data-ttu-id="4ad1d-190">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="4ad1d-190">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="4ad1d-191">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="4ad1d-191">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="4ad1d-192">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="4ad1d-192">Az.HDInsight</span></span>
* <span data-ttu-id="4ad1d-193">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="4ad1d-193">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="4ad1d-194">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="4ad1d-194">Az.IotHub</span></span>
* <span data-ttu-id="4ad1d-195">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-195">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="4ad1d-196">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-196">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="4ad1d-197">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-197">New cmdlets are:</span></span>
    - <span data-ttu-id="4ad1d-198">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="4ad1d-198">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="4ad1d-199">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="4ad1d-199">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="4ad1d-200">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="4ad1d-200">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="4ad1d-201">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="4ad1d-201">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="4ad1d-202">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="4ad1d-202">Az.Monitor</span></span>
* <span data-ttu-id="4ad1d-203">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="4ad1d-203">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="4ad1d-204">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-204">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="4ad1d-205">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-205">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="4ad1d-206">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-206">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="4ad1d-207">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-207">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="4ad1d-208">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-208">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="4ad1d-209">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-209">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="4ad1d-210">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-210">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="4ad1d-211">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-211">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="4ad1d-212">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-212">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="4ad1d-213">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-213">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="4ad1d-214">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-214">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="4ad1d-215">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="4ad1d-215">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="4ad1d-216">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="4ad1d-216">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="4ad1d-217">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="4ad1d-217">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="4ad1d-218">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="4ad1d-218">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="4ad1d-219">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="4ad1d-219">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="4ad1d-220">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="4ad1d-220">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="4ad1d-221">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-221">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="4ad1d-222">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="4ad1d-222">Overall improved help files</span></span>
* <span data-ttu-id="4ad1d-223">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-223">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-224">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-224">Az.Network</span></span>
* <span data-ttu-id="4ad1d-225">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-225">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="4ad1d-226">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="4ad1d-226">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="4ad1d-227">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="4ad1d-227">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="4ad1d-228">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-228">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="4ad1d-229">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="4ad1d-229">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="4ad1d-230">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="4ad1d-230">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="4ad1d-231">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="4ad1d-231">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="4ad1d-232">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="4ad1d-232">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="4ad1d-233">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ad1d-233">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="4ad1d-234">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="4ad1d-234">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="4ad1d-235">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="4ad1d-235">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="4ad1d-236">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="4ad1d-236">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="4ad1d-237">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="4ad1d-237">New cmdlets</span></span>
        - <span data-ttu-id="4ad1d-238">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="4ad1d-238">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="4ad1d-239">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-239">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="4ad1d-240">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-240">Updated cmdlet:</span></span>
        - <span data-ttu-id="4ad1d-241">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="4ad1d-241">New-VpnSite</span></span>
        - <span data-ttu-id="4ad1d-242">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="4ad1d-242">Update-VpnSite</span></span>
        - <span data-ttu-id="4ad1d-243">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-243">New-VpnConnection</span></span>
        - <span data-ttu-id="4ad1d-244">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-244">Update-VpnConnection</span></span>
* <span data-ttu-id="4ad1d-245">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="4ad1d-245">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="4ad1d-246">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-246">Az.RecoveryServices</span></span>
* <span data-ttu-id="4ad1d-247">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="4ad1d-247">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="4ad1d-248">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="4ad1d-248">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-249">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-249">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-250">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-250">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="4ad1d-251">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="4ad1d-251">Az.ServiceFabric</span></span>
* <span data-ttu-id="4ad1d-252">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-252">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="4ad1d-253">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-253">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="4ad1d-254">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="4ad1d-254">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="4ad1d-255">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="4ad1d-255">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="4ad1d-256">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="4ad1d-256">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="4ad1d-257">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="4ad1d-257">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="4ad1d-258">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="4ad1d-258">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="4ad1d-259">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="4ad1d-259">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="4ad1d-260">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="4ad1d-260">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="4ad1d-261">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="4ad1d-261">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="4ad1d-262">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="4ad1d-262">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="4ad1d-263">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="4ad1d-263">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="4ad1d-264">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="4ad1d-264">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="4ad1d-265">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="4ad1d-265">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="4ad1d-266">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="4ad1d-266">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="4ad1d-267">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-267">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="4ad1d-268">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="4ad1d-268">Az.SignalR</span></span>
* <span data-ttu-id="4ad1d-269">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-269">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-270">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-270">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-271">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-271">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="4ad1d-272">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="4ad1d-272">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="4ad1d-273">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="4ad1d-273">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="4ad1d-274">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-274">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="4ad1d-275">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="4ad1d-275">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="4ad1d-276">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-276">Az.Storage</span></span>
* <span data-ttu-id="4ad1d-277">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-277">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="4ad1d-278">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="4ad1d-278">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="4ad1d-279">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="4ad1d-279">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="4ad1d-280">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="4ad1d-280">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="4ad1d-281">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-281">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="4ad1d-282">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="4ad1d-282">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="4ad1d-283">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="4ad1d-283">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="4ad1d-284">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="4ad1d-284">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="4ad1d-285">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="4ad1d-285">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="4ad1d-286">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="4ad1d-286">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="4ad1d-287">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="4ad1d-287">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="4ad1d-288">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="4ad1d-288">Az.Websites</span></span>
* <span data-ttu-id="4ad1d-289">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="4ad1d-289">Fixing issue where webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="4ad1d-290">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="4ad1d-290">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="4ad1d-291">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-291">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="4ad1d-292">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-292">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="4ad1d-293">Geral</span><span class="sxs-lookup"><span data-stu-id="4ad1d-293">General</span></span>
* <span data-ttu-id="4ad1d-294">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-294">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="4ad1d-295">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-295">Az.Accounts</span></span>
* <span data-ttu-id="4ad1d-296">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="4ad1d-296">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="4ad1d-297">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="4ad1d-297">Az.Aks</span></span>
* <span data-ttu-id="4ad1d-298">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-298">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="4ad1d-299">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="4ad1d-299">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="4ad1d-300">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="4ad1d-300">Az.ApiManagement</span></span>
* <span data-ttu-id="4ad1d-301">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="4ad1d-301">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="4ad1d-302">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="4ad1d-302">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="4ad1d-303">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-303">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="4ad1d-304">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="4ad1d-304">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="4ad1d-305">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-305">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="4ad1d-306">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="4ad1d-306">Az.Batch</span></span>
* <span data-ttu-id="4ad1d-307">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="4ad1d-307">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="4ad1d-308">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="4ad1d-308">Az.Cdn</span></span>
* <span data-ttu-id="4ad1d-309">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="4ad1d-309">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-310">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-310">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-311">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-311">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="4ad1d-312">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="4ad1d-312">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="4ad1d-313">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="4ad1d-313">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="4ad1d-314">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="4ad1d-314">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="4ad1d-315">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="4ad1d-315">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="4ad1d-316">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="4ad1d-316">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="4ad1d-317">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="4ad1d-317">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="4ad1d-318">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-318">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="4ad1d-319">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="4ad1d-319">Az.DataFactory</span></span>
* <span data-ttu-id="4ad1d-320">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-320">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="4ad1d-321">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="4ad1d-321">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="4ad1d-322">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="4ad1d-322">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="4ad1d-323">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="4ad1d-323">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="4ad1d-324">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4ad1d-324">Az.DataLakeStore</span></span>
* <span data-ttu-id="4ad1d-325">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-325">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="4ad1d-326">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="4ad1d-326">Az.EventHub</span></span>
* <span data-ttu-id="4ad1d-327">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="4ad1d-327">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="4ad1d-328">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="4ad1d-328">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="4ad1d-329">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="4ad1d-329">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="4ad1d-330">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="4ad1d-330">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="4ad1d-331">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="4ad1d-331">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="4ad1d-332">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="4ad1d-332">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="4ad1d-333">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="4ad1d-333">Az.Monitor</span></span>
* <span data-ttu-id="4ad1d-334">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="4ad1d-334">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-335">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-335">Az.Network</span></span>
* <span data-ttu-id="4ad1d-336">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="4ad1d-336">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="4ad1d-337">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-337">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="4ad1d-338">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-338">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="4ad1d-339">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="4ad1d-339">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="4ad1d-340">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-340">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="4ad1d-341">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-341">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="4ad1d-342">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="4ad1d-342">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="4ad1d-343">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="4ad1d-343">Az.OperationalInsights</span></span>
* <span data-ttu-id="4ad1d-344">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-344">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="4ad1d-345">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="4ad1d-345">Added example</span></span>
    - <span data-ttu-id="4ad1d-346">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-346">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="4ad1d-347">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="4ad1d-347">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="4ad1d-348">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="4ad1d-348">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="4ad1d-349">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-349">Az.RecoveryServices</span></span>
* <span data-ttu-id="4ad1d-350">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-350">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-351">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-351">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-352">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="4ad1d-352">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="4ad1d-353">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="4ad1d-353">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="4ad1d-354">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="4ad1d-354">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="4ad1d-355">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="4ad1d-355">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="4ad1d-356">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="4ad1d-356">Az.ServiceBus</span></span>
* <span data-ttu-id="4ad1d-357">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="4ad1d-357">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="4ad1d-358">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="4ad1d-358">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="4ad1d-359">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="4ad1d-359">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="4ad1d-360">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="4ad1d-360">Az.ServiceFabric</span></span>
* <span data-ttu-id="4ad1d-361">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-361">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="4ad1d-362">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-362">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="4ad1d-363">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="4ad1d-363">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="4ad1d-364">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-364">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="4ad1d-365">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="4ad1d-365">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="4ad1d-366">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="4ad1d-366">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-367">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-367">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-368">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-368">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="4ad1d-369">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-369">Az.Storage</span></span>
* <span data-ttu-id="4ad1d-370">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="4ad1d-370">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="4ad1d-371">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="4ad1d-371">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="4ad1d-372">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="4ad1d-372">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="4ad1d-373">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="4ad1d-373">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="4ad1d-374">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="4ad1d-374">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="4ad1d-375">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="4ad1d-375">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="4ad1d-376">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="4ad1d-376">Az.Websites</span></span>
* <span data-ttu-id="4ad1d-377">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="4ad1d-377">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="4ad1d-378">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-378">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="4ad1d-379">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-379">Az.Accounts</span></span>
* <span data-ttu-id="4ad1d-380">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="4ad1d-380">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="4ad1d-381">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="4ad1d-381">Az.ApplicationInsights</span></span>
* <span data-ttu-id="4ad1d-382">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-382">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="4ad1d-383">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="4ad1d-383">Az.Automation</span></span>
* <span data-ttu-id="4ad1d-384">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-384">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="4ad1d-385">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-385">Az.CognitiveServices</span></span>
* <span data-ttu-id="4ad1d-386">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-386">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-387">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-387">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-388">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-388">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="4ad1d-389">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="4ad1d-389">Az.ContainerRegistry</span></span>
* <span data-ttu-id="4ad1d-390">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="4ad1d-390">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="4ad1d-391">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="4ad1d-391">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="4ad1d-392">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="4ad1d-392">Az.DataFactory</span></span>
* <span data-ttu-id="4ad1d-393">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="4ad1d-393">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="4ad1d-394">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-394">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="4ad1d-395">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="4ad1d-395">Az.EventHub</span></span>
* <span data-ttu-id="4ad1d-396">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="4ad1d-396">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="4ad1d-397">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="4ad1d-397">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="4ad1d-398">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="4ad1d-398">Az.KeyVault</span></span>
* <span data-ttu-id="4ad1d-399">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="4ad1d-399">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="4ad1d-400">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="4ad1d-400">Az.LogicApp</span></span>
* <span data-ttu-id="4ad1d-401">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="4ad1d-401">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="4ad1d-402">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="4ad1d-402">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="4ad1d-403">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-403">Az.ManagedServices</span></span>
* <span data-ttu-id="4ad1d-404">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="4ad1d-404">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-405">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-405">Az.Network</span></span>
* <span data-ttu-id="4ad1d-406">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="4ad1d-406">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="4ad1d-407">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="4ad1d-407">New cmdlets</span></span>
        - <span data-ttu-id="4ad1d-408">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="4ad1d-408">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="4ad1d-409">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="4ad1d-409">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="4ad1d-410">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-410">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="4ad1d-411">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-411">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="4ad1d-412">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-412">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="4ad1d-413">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-413">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="4ad1d-414">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="4ad1d-414">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="4ad1d-415">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="4ad1d-415">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="4ad1d-416">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="4ad1d-416">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="4ad1d-417">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-417">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="4ad1d-418">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-418">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="4ad1d-419">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-419">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="4ad1d-420">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="4ad1d-420">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="4ad1d-421">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="4ad1d-421">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="4ad1d-422">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="4ad1d-422">Updated cmdlets</span></span>
        - <span data-ttu-id="4ad1d-423">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-423">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="4ad1d-424">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-424">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="4ad1d-425">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-425">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="4ad1d-426">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-426">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="4ad1d-427">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ad1d-427">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="4ad1d-428">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-428">Updated cmdlet:</span></span>
        - <span data-ttu-id="4ad1d-429">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-429">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="4ad1d-430">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-430">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="4ad1d-431">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-431">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="4ad1d-432">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="4ad1d-432">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="4ad1d-433">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-433">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="4ad1d-434">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-434">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="4ad1d-435">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="4ad1d-435">Az.OperationalInsights</span></span>
* <span data-ttu-id="4ad1d-436">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-436">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="4ad1d-437">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="4ad1d-437">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="4ad1d-438">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-438">Az.RecoveryServices</span></span>
* <span data-ttu-id="4ad1d-439">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-439">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="4ad1d-440">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-440">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="4ad1d-441">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-441">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="4ad1d-442">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-442">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="4ad1d-443">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-443">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="4ad1d-444">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-444">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="4ad1d-445">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-445">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="4ad1d-446">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-446">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="4ad1d-447">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="4ad1d-447">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="4ad1d-448">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-448">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-449">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-449">Az.Resources</span></span>
- <span data-ttu-id="4ad1d-450">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-450">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="4ad1d-451">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="4ad1d-451">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="4ad1d-452">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="4ad1d-452">Az.ServiceBus</span></span>
* <span data-ttu-id="4ad1d-453">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="4ad1d-453">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="4ad1d-454">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="4ad1d-454">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-455">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-455">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-456">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="4ad1d-456">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="4ad1d-457">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="4ad1d-457">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="4ad1d-458">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-458">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="4ad1d-459">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-459">Az.Storage</span></span>
* <span data-ttu-id="4ad1d-460">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="4ad1d-460">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="4ad1d-461">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="4ad1d-461">Az.StorageSync</span></span>
* <span data-ttu-id="4ad1d-462">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-462">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="4ad1d-463">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="4ad1d-463">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="4ad1d-464">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="4ad1d-464">Az.Websites</span></span>
* <span data-ttu-id="4ad1d-465">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="4ad1d-465">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="4ad1d-466">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="4ad1d-466">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="4ad1d-467">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="4ad1d-467">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="4ad1d-468">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-468">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="4ad1d-469">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-469">Az.Accounts</span></span>
* <span data-ttu-id="4ad1d-470">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="4ad1d-470">Add support for profile cmdlets</span></span>
* <span data-ttu-id="4ad1d-471">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="4ad1d-471">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="4ad1d-472">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="4ad1d-472">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="4ad1d-473">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="4ad1d-473">Az.Advisor</span></span>
* <span data-ttu-id="4ad1d-474">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="4ad1d-474">GA release of Az.Advisor</span></span>
* <span data-ttu-id="4ad1d-475">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="4ad1d-475">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="4ad1d-476">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="4ad1d-476">Az.ApiManagement</span></span>
* <span data-ttu-id="4ad1d-477">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="4ad1d-477">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="4ad1d-478">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="4ad1d-478">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="4ad1d-479">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="4ad1d-479">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="4ad1d-480">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-480">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="4ad1d-481">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="4ad1d-481">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="4ad1d-482">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="4ad1d-482">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="4ad1d-483">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="4ad1d-483">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="4ad1d-484">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="4ad1d-484">Az.Automation</span></span>
* <span data-ttu-id="4ad1d-485">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="4ad1d-485">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-486">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-486">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-487">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-487">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="4ad1d-488">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="4ad1d-488">Az.DataFactory</span></span>
* <span data-ttu-id="4ad1d-489">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-489">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="4ad1d-490">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="4ad1d-490">Az.EventGrid</span></span>
* <span data-ttu-id="4ad1d-491">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-491">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="4ad1d-492">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="4ad1d-492">Az.IotHub</span></span>
* <span data-ttu-id="4ad1d-493">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-493">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-494">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-494">Az.Network</span></span>
* <span data-ttu-id="4ad1d-495">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="4ad1d-495">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="4ad1d-496">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-496">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="4ad1d-497">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="4ad1d-497">Az.PolicyInsights</span></span>
* <span data-ttu-id="4ad1d-498">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="4ad1d-498">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="4ad1d-499">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="4ad1d-499">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="4ad1d-500">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="4ad1d-500">Az.OperationalInsights</span></span>
* <span data-ttu-id="4ad1d-501">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="4ad1d-501">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="4ad1d-502">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-502">Az.RecoveryServices</span></span>
* <span data-ttu-id="4ad1d-503">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="4ad1d-503">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-504">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-504">Az.Resources</span></span>
    - <span data-ttu-id="4ad1d-505">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="4ad1d-505">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="4ad1d-506">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="4ad1d-506">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="4ad1d-507">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="4ad1d-507">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="4ad1d-508">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="4ad1d-508">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="4ad1d-509">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="4ad1d-509">Az.ServiceBus</span></span>
* <span data-ttu-id="4ad1d-510">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-510">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-511">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-511">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-512">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="4ad1d-512">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="4ad1d-513">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-513">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="4ad1d-514">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="4ad1d-514">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="4ad1d-515">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="4ad1d-515">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="4ad1d-516">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="4ad1d-516">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="4ad1d-517">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="4ad1d-517">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="4ad1d-518">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="4ad1d-518">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="4ad1d-519">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="4ad1d-519">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="4ad1d-520">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="4ad1d-520">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="4ad1d-521">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-521">Az.Storage</span></span>
* <span data-ttu-id="4ad1d-522">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-522">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="4ad1d-523">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="4ad1d-523">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="4ad1d-524">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="4ad1d-524">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="4ad1d-525">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="4ad1d-525">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="4ad1d-526">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="4ad1d-526">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="4ad1d-527">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="4ad1d-527">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="4ad1d-528">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="4ad1d-528">Set-AzStorageAccount</span></span>
* <span data-ttu-id="4ad1d-529">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="4ad1d-529">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="4ad1d-530">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="4ad1d-530">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="4ad1d-531">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="4ad1d-531">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="4ad1d-532">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="4ad1d-532">Az.StorageSync</span></span>
* <span data-ttu-id="4ad1d-533">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="4ad1d-533">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="4ad1d-534">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-534">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="4ad1d-535">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-535">Az.Accounts</span></span>
* <span data-ttu-id="4ad1d-536">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="4ad1d-536">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="4ad1d-537">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="4ad1d-537">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="4ad1d-538">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="4ad1d-538">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="4ad1d-539">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="4ad1d-539">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="4ad1d-540">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="4ad1d-540">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-541">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-541">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-542">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="4ad1d-542">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="4ad1d-543">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-543">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="4ad1d-544">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="4ad1d-544">Az.Dns</span></span>
* <span data-ttu-id="4ad1d-545">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="4ad1d-545">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="4ad1d-546">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="4ad1d-546">Az.EventGrid</span></span>
* <span data-ttu-id="4ad1d-547">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-547">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="4ad1d-548">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-548">New cmdlets:</span></span>
    - <span data-ttu-id="4ad1d-549">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="4ad1d-549">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="4ad1d-550">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-550">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="4ad1d-551">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="4ad1d-551">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="4ad1d-552">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-552">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="4ad1d-553">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="4ad1d-553">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="4ad1d-554">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-554">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="4ad1d-555">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="4ad1d-555">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="4ad1d-556">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-556">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="4ad1d-557">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="4ad1d-557">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="4ad1d-558">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-558">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="4ad1d-559">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-559">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="4ad1d-560">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-560">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="4ad1d-561">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="4ad1d-561">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="4ad1d-562">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="4ad1d-562">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="4ad1d-563">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-563">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="4ad1d-564">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-564">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="4ad1d-565">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-565">Updated cmdlets:</span></span>
    - <span data-ttu-id="4ad1d-566">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-566">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="4ad1d-567">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-567">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="4ad1d-568">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-568">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="4ad1d-569">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="4ad1d-569">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="4ad1d-570">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-570">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="4ad1d-571">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="4ad1d-571">Event subscription expiration date,</span></span>
            - <span data-ttu-id="4ad1d-572">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-572">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="4ad1d-573">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-573">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="4ad1d-574">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="4ad1d-574">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="4ad1d-575">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-575">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="4ad1d-576">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-576">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="4ad1d-577">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="4ad1d-577">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="4ad1d-578">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-578">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="4ad1d-579">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-579">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="4ad1d-580">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="4ad1d-580">Az.FrontDoor</span></span>
* <span data-ttu-id="4ad1d-581">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="4ad1d-581">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="4ad1d-582">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="4ad1d-582">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="4ad1d-583">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="4ad1d-583">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="4ad1d-584">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="4ad1d-584">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-585">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-585">Az.Network</span></span>
* <span data-ttu-id="4ad1d-586">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="4ad1d-586">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="4ad1d-587">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="4ad1d-587">New cmdlets</span></span>
        - <span data-ttu-id="4ad1d-588">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="4ad1d-588">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="4ad1d-589">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="4ad1d-589">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="4ad1d-590">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="4ad1d-590">New cmdlets</span></span> 
        - <span data-ttu-id="4ad1d-591">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="4ad1d-591">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="4ad1d-592">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="4ad1d-592">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="4ad1d-593">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="4ad1d-593">New cmdlets</span></span> 
        - <span data-ttu-id="4ad1d-594">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="4ad1d-594">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="4ad1d-595">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="4ad1d-595">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="4ad1d-596">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="4ad1d-596">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="4ad1d-597">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-597">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="4ad1d-598">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-598">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="4ad1d-599">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="4ad1d-599">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="4ad1d-600">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="4ad1d-600">New cmdlets</span></span>
        - <span data-ttu-id="4ad1d-601">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="4ad1d-601">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="4ad1d-602">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="4ad1d-602">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="4ad1d-603">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="4ad1d-603">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="4ad1d-604">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-604">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="4ad1d-605">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-605">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="4ad1d-606">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-606">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="4ad1d-607">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-607">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="4ad1d-608">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-608">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="4ad1d-609">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-609">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="4ad1d-610">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="4ad1d-610">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="4ad1d-611">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ad1d-611">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="4ad1d-612">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-612">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="4ad1d-613">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ad1d-613">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="4ad1d-614">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="4ad1d-614">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="4ad1d-615">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="4ad1d-615">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="4ad1d-616">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="4ad1d-616">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="4ad1d-617">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="4ad1d-617">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="4ad1d-618">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="4ad1d-618">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="4ad1d-619">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-619">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="4ad1d-620">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="4ad1d-620">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="4ad1d-621">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="4ad1d-621">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="4ad1d-622">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="4ad1d-622">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="4ad1d-623">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="4ad1d-623">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="4ad1d-624">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-624">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="4ad1d-625">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-625">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="4ad1d-626">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-626">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="4ad1d-627">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-627">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="4ad1d-628">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="4ad1d-628">Az.OperationalInsights</span></span>
* <span data-ttu-id="4ad1d-629">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-629">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-630">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-630">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-631">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="4ad1d-631">Support for additional Template Export options</span></span>
    - <span data-ttu-id="4ad1d-632">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="4ad1d-632">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="4ad1d-633">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="4ad1d-633">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="4ad1d-634">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="4ad1d-634">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="4ad1d-635">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="4ad1d-635">Az.ServiceFabric</span></span>
* <span data-ttu-id="4ad1d-636">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-636">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-637">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-637">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-638">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-638">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="4ad1d-639">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-639">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="4ad1d-640">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="4ad1d-640">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="4ad1d-641">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="4ad1d-641">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="4ad1d-642">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="4ad1d-642">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="4ad1d-643">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="4ad1d-643">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="4ad1d-644">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="4ad1d-644">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="4ad1d-645">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="4ad1d-645">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="4ad1d-646">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-646">Az.Storage</span></span>
* <span data-ttu-id="4ad1d-647">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="4ad1d-647">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="4ad1d-648">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="4ad1d-648">New-AzStorageAccount</span></span>
* <span data-ttu-id="4ad1d-649">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="4ad1d-649">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="4ad1d-650">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="4ad1d-650">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="4ad1d-651">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="4ad1d-651">Az.Websites</span></span>
* <span data-ttu-id="4ad1d-652">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="4ad1d-652">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="4ad1d-653">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="4ad1d-653">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="4ad1d-654">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-654">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="4ad1d-655">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="4ad1d-655">Az.Cdn</span></span>
* <span data-ttu-id="4ad1d-656">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-656">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-657">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-657">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-658">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-658">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="4ad1d-659">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="4ad1d-659">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="4ad1d-660">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="4ad1d-660">Az.EventHub</span></span>
* <span data-ttu-id="4ad1d-661">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="4ad1d-661">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="4ad1d-662">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="4ad1d-662">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-663">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-663">Az.Network</span></span>
* <span data-ttu-id="4ad1d-664">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="4ad1d-664">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="4ad1d-665">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="4ad1d-665">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="4ad1d-666">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="4ad1d-666">Az.PolicyInsights</span></span>
* <span data-ttu-id="4ad1d-667">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="4ad1d-667">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="4ad1d-668">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-668">Az.RecoveryServices</span></span>
* <span data-ttu-id="4ad1d-669">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="4ad1d-669">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="4ad1d-670">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="4ad1d-670">Az.ServiceBus</span></span>
* <span data-ttu-id="4ad1d-671">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="4ad1d-671">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="4ad1d-672">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="4ad1d-672">Az.ServiceFabric</span></span>
* <span data-ttu-id="4ad1d-673">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-673">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="4ad1d-674">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4ad1d-674">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-675">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-675">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-676">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-676">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="4ad1d-677">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="4ad1d-677">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="4ad1d-678">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-678">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="4ad1d-679">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-679">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="4ad1d-680">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="4ad1d-680">Az.Websites</span></span>
* <span data-ttu-id="4ad1d-681">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="4ad1d-681">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="4ad1d-682">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-682">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="4ad1d-683">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="4ad1d-683">Az.ApiManagement</span></span>
* <span data-ttu-id="4ad1d-684">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="4ad1d-684">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="4ad1d-685">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="4ad1d-685">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="4ad1d-686">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="4ad1d-686">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="4ad1d-687">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="4ad1d-687">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="4ad1d-688">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-688">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="4ad1d-689">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="4ad1d-689">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="4ad1d-690">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="4ad1d-690">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="4ad1d-691">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="4ad1d-691">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="4ad1d-692">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="4ad1d-692">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="4ad1d-693">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="4ad1d-693">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="4ad1d-694">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="4ad1d-694">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="4ad1d-695">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="4ad1d-695">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="4ad1d-696">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="4ad1d-696">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="4ad1d-697">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="4ad1d-697">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="4ad1d-698">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="4ad1d-698">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="4ad1d-699">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="4ad1d-699">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="4ad1d-700">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="4ad1d-700">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="4ad1d-701">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="4ad1d-701">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="4ad1d-702">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-702">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="4ad1d-703">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="4ad1d-703">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="4ad1d-704">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="4ad1d-704">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="4ad1d-705">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-705">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="4ad1d-706">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-706">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="4ad1d-707">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="4ad1d-707">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="4ad1d-708">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-708">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="4ad1d-709">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-709">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="4ad1d-710">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="4ad1d-710">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="4ad1d-711">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-711">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="4ad1d-712">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-712">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="4ad1d-713">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="4ad1d-713">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="4ad1d-714">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="4ad1d-714">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="4ad1d-715">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="4ad1d-715">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="4ad1d-716">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-716">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="4ad1d-717">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="4ad1d-717">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="4ad1d-718">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-718">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="4ad1d-719">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="4ad1d-719">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="4ad1d-720">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-720">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="4ad1d-721">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-721">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="4ad1d-722">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-722">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="4ad1d-723">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="4ad1d-723">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="4ad1d-724">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="4ad1d-724">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="4ad1d-725">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-725">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="4ad1d-726">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="4ad1d-726">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="4ad1d-727">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-727">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="4ad1d-728">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="4ad1d-728">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="4ad1d-729">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="4ad1d-729">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="4ad1d-730">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-730">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="4ad1d-731">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-731">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="4ad1d-732">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="4ad1d-732">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="4ad1d-733">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="4ad1d-733">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="4ad1d-734">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-734">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="4ad1d-735">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-735">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="4ad1d-736">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-736">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="4ad1d-737">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="4ad1d-737">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="4ad1d-738">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-738">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="4ad1d-739">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-739">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="4ad1d-740">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="4ad1d-740">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="4ad1d-741">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-741">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="4ad1d-742">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-742">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="4ad1d-743">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-743">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="4ad1d-744">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="4ad1d-744">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="4ad1d-745">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-745">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="4ad1d-746">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-746">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="4ad1d-747">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-747">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="4ad1d-748">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="4ad1d-748">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="4ad1d-749">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-749">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="4ad1d-750">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="4ad1d-750">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="4ad1d-751">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-751">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="4ad1d-752">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="4ad1d-752">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="4ad1d-753">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-753">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="4ad1d-754">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="4ad1d-754">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="4ad1d-755">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-755">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="4ad1d-756">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-756">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="4ad1d-757">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="4ad1d-757">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="4ad1d-758">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-758">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="4ad1d-759">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-759">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="4ad1d-760">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-760">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="4ad1d-761">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="4ad1d-761">Az.Automation</span></span>
* <span data-ttu-id="4ad1d-762">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-762">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="4ad1d-763">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="4ad1d-763">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="4ad1d-764">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="4ad1d-764">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="4ad1d-765">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-765">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="4ad1d-766">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="4ad1d-766">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="4ad1d-767">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-767">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="4ad1d-768">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-768">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-769">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-769">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-770">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-770">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="4ad1d-771">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="4ad1d-771">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="4ad1d-772">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4ad1d-772">Az.DataLakeStore</span></span>
* <span data-ttu-id="4ad1d-773">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="4ad1d-773">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="4ad1d-774">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="4ad1d-774">Az.Monitor</span></span>
* <span data-ttu-id="4ad1d-775">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="4ad1d-775">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-776">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-776">Az.Network</span></span>
* <span data-ttu-id="4ad1d-777">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="4ad1d-777">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="4ad1d-778">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-778">Updated cmdlet:</span></span>
        - <span data-ttu-id="4ad1d-779">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="4ad1d-779">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="4ad1d-780">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="4ad1d-780">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-781">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-781">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-782">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="4ad1d-782">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-783">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-783">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-784">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="4ad1d-784">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="4ad1d-785">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-785">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="4ad1d-786">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-786">Az.Accounts</span></span>
* <span data-ttu-id="4ad1d-787">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="4ad1d-787">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="4ad1d-788">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-788">Az.CognitiveServices</span></span>
* <span data-ttu-id="4ad1d-789">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-789">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="4ad1d-790">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-790">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-791">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-791">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-792">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-792">Proximity placement group feature.</span></span>
    - <span data-ttu-id="4ad1d-793">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="4ad1d-793">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="4ad1d-794">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-794">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="4ad1d-795">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-795">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="4ad1d-796">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-796">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="4ad1d-797">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="4ad1d-797">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="4ad1d-798">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="4ad1d-798">Breaking changes</span></span>
    - <span data-ttu-id="4ad1d-799">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-799">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="4ad1d-800">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-800">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="4ad1d-801">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="4ad1d-801">Az.DeploymentManager</span></span>
* <span data-ttu-id="4ad1d-802">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="4ad1d-802">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="4ad1d-803">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="4ad1d-803">Az.Dns</span></span>
* <span data-ttu-id="4ad1d-804">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="4ad1d-804">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="4ad1d-805">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-805">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="4ad1d-806">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-806">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="4ad1d-807">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="4ad1d-807">Az.FrontDoor</span></span>
* <span data-ttu-id="4ad1d-808">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="4ad1d-808">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="4ad1d-809">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-809">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="4ad1d-810">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="4ad1d-810">Az.HDInsight</span></span>
* <span data-ttu-id="4ad1d-811">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-811">Removed two cmdlets:</span></span>
    - <span data-ttu-id="4ad1d-812">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="4ad1d-812">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="4ad1d-813">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="4ad1d-813">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="4ad1d-814">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="4ad1d-814">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="4ad1d-815">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-815">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="4ad1d-816">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-816">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="4ad1d-817">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-817">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="4ad1d-818">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="4ad1d-818">Az.Monitor</span></span>
* <span data-ttu-id="4ad1d-819">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="4ad1d-819">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="4ad1d-820">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="4ad1d-820">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="4ad1d-821">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="4ad1d-821">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="4ad1d-822">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="4ad1d-822">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="4ad1d-823">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="4ad1d-823">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="4ad1d-824">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="4ad1d-824">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="4ad1d-825">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="4ad1d-825">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="4ad1d-826">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="4ad1d-826">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="4ad1d-827">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="4ad1d-827">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="4ad1d-828">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="4ad1d-828">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="4ad1d-829">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="4ad1d-829">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="4ad1d-830">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="4ad1d-830">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="4ad1d-831">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="4ad1d-831">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="4ad1d-832">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="4ad1d-832">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-833">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-833">Az.Network</span></span>
* <span data-ttu-id="4ad1d-834">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="4ad1d-834">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="4ad1d-835">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="4ad1d-835">New cmdlets</span></span>
        - <span data-ttu-id="4ad1d-836">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="4ad1d-836">New-AzNatGateway</span></span>
        - <span data-ttu-id="4ad1d-837">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="4ad1d-837">Get-AzNatGateway</span></span>
        - <span data-ttu-id="4ad1d-838">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="4ad1d-838">Set-AzNatGateway</span></span>
        - <span data-ttu-id="4ad1d-839">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="4ad1d-839">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="4ad1d-840">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="4ad1d-840">Updated cmdlets</span></span>
        - <span data-ttu-id="4ad1d-841">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="4ad1d-841">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="4ad1d-842">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="4ad1d-842">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="4ad1d-843">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-843">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="4ad1d-844">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-844">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="4ad1d-845">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-845">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="4ad1d-846">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="4ad1d-846">Az.PolicyInsights</span></span>
* <span data-ttu-id="4ad1d-847">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-847">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="4ad1d-848">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-848">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="4ad1d-849">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="4ad1d-849">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="4ad1d-850">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-850">Az.RecoveryServices</span></span>
* <span data-ttu-id="4ad1d-851">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-851">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="4ad1d-852">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-852">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="4ad1d-853">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-853">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="4ad1d-854">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-854">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="4ad1d-855">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-855">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="4ad1d-856">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-856">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="4ad1d-857">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="4ad1d-857">Az.Relay</span></span>
* <span data-ttu-id="4ad1d-858">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="4ad1d-858">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="4ad1d-859">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="4ad1d-859">Az.ServiceBus</span></span>
* <span data-ttu-id="4ad1d-860">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="4ad1d-860">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="4ad1d-861">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-861">Az.Storage</span></span>
* <span data-ttu-id="4ad1d-862">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="4ad1d-862">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="4ad1d-863">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-863">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="4ad1d-864">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-864">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="4ad1d-865">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="4ad1d-865">New-AzStorageAccount</span></span>
* <span data-ttu-id="4ad1d-866">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="4ad1d-866">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="4ad1d-867">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="4ad1d-867">New-AzStorageAccount</span></span>
    - <span data-ttu-id="4ad1d-868">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="4ad1d-868">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="4ad1d-869">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="4ad1d-869">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="4ad1d-870">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="4ad1d-870">Az.Websites</span></span>
* <span data-ttu-id="4ad1d-871">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="4ad1d-871">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="4ad1d-872">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="4ad1d-872">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="4ad1d-873">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-873">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="4ad1d-874">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="4ad1d-874">Highlights since the last major release</span></span>
* <span data-ttu-id="4ad1d-875">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="4ad1d-875">General availability of `Az` module</span></span>
* <span data-ttu-id="4ad1d-876">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="4ad1d-876">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="4ad1d-877">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="4ad1d-877">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="4ad1d-878">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-878">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="4ad1d-879">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="4ad1d-879">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="4ad1d-880">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="4ad1d-880">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="4ad1d-881">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="4ad1d-881">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="4ad1d-882">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-882">Az.Accounts</span></span>
* <span data-ttu-id="4ad1d-883">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="4ad1d-883">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="4ad1d-884">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="4ad1d-884">Az.Batch</span></span>
* <span data-ttu-id="4ad1d-885">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-885">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="4ad1d-886">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="4ad1d-886">Az.Cdn</span></span>
* <span data-ttu-id="4ad1d-887">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-887">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="4ad1d-888">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-888">Az.CognitiveServices</span></span>
* <span data-ttu-id="4ad1d-889">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-889">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-890">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-890">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-891">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="4ad1d-891">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="4ad1d-892">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-892">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="4ad1d-893">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="4ad1d-893">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="4ad1d-894">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="4ad1d-894">Az.DataFactory</span></span>
* <span data-ttu-id="4ad1d-895">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-895">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="4ad1d-896">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4ad1d-896">Az.DataLakeStore</span></span>
* <span data-ttu-id="4ad1d-897">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-897">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="4ad1d-898">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="4ad1d-898">Az.EventGrid</span></span>
* <span data-ttu-id="4ad1d-899">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-899">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="4ad1d-900">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="4ad1d-900">Az.EventHub</span></span>
* <span data-ttu-id="4ad1d-901">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="4ad1d-901">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="4ad1d-902">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="4ad1d-902">Az.HDInsight</span></span>
* <span data-ttu-id="4ad1d-903">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-903">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="4ad1d-904">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="4ad1d-904">Az.IotHub</span></span>
* <span data-ttu-id="4ad1d-905">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-905">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="4ad1d-906">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="4ad1d-906">Az.KeyVault</span></span>
* <span data-ttu-id="4ad1d-907">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-907">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="4ad1d-908">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="4ad1d-908">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="4ad1d-909">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="4ad1d-909">Az.MachineLearning</span></span>
* <span data-ttu-id="4ad1d-910">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-910">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="4ad1d-911">Az.Media</span><span class="sxs-lookup"><span data-stu-id="4ad1d-911">Az.Media</span></span>
* <span data-ttu-id="4ad1d-912">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-912">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="4ad1d-913">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="4ad1d-913">Az.Monitor</span></span>
  * <span data-ttu-id="4ad1d-914">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="4ad1d-914">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="4ad1d-915">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="4ad1d-915">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="4ad1d-916">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="4ad1d-916">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="4ad1d-917">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="4ad1d-917">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="4ad1d-918">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="4ad1d-918">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="4ad1d-919">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="4ad1d-919">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="4ad1d-920">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="4ad1d-920">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-921">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-921">Az.Network</span></span>
* <span data-ttu-id="4ad1d-922">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-922">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="4ad1d-923">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="4ad1d-923">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="4ad1d-924">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="4ad1d-924">Az.NotificationHubs</span></span>
* <span data-ttu-id="4ad1d-925">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-925">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="4ad1d-926">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="4ad1d-926">Az.OperationalInsights</span></span>
* <span data-ttu-id="4ad1d-927">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-927">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="4ad1d-928">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="4ad1d-928">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="4ad1d-929">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-929">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="4ad1d-930">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-930">Az.RecoveryServices</span></span>
* <span data-ttu-id="4ad1d-931">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-931">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="4ad1d-932">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="4ad1d-932">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="4ad1d-933">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="4ad1d-933">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="4ad1d-934">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="4ad1d-934">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="4ad1d-935">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="4ad1d-935">Az.RedisCache</span></span>
* <span data-ttu-id="4ad1d-936">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-936">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-937">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-937">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-938">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="4ad1d-938">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-939">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-939">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-940">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="4ad1d-940">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="4ad1d-941">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-941">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="4ad1d-942">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-942">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="4ad1d-943">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-943">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="4ad1d-944">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-944">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="4ad1d-945">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-945">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="4ad1d-946">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="4ad1d-946">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="4ad1d-947">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="4ad1d-947">Az.Websites</span></span>
* <span data-ttu-id="4ad1d-948">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="4ad1d-948">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="4ad1d-949">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-949">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="4ad1d-950">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-950">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="4ad1d-951">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-951">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="4ad1d-952">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-952">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="4ad1d-953">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="4ad1d-953">Highlights since the last major release</span></span>
* <span data-ttu-id="4ad1d-954">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="4ad1d-954">General availability of `Az` module</span></span>
* <span data-ttu-id="4ad1d-955">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="4ad1d-955">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="4ad1d-956">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="4ad1d-956">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="4ad1d-957">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-957">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="4ad1d-958">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="4ad1d-958">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="4ad1d-959">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="4ad1d-959">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="4ad1d-960">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="4ad1d-960">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="4ad1d-961">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-961">Az.Accounts</span></span>
* <span data-ttu-id="4ad1d-962">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="4ad1d-962">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="4ad1d-963">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-963">Az.AnalysisServices</span></span>
* <span data-ttu-id="4ad1d-964">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="4ad1d-964">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="4ad1d-965">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="4ad1d-965">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="4ad1d-966">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="4ad1d-966">Az.Automation</span></span>
* <span data-ttu-id="4ad1d-967">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-967">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="4ad1d-968">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-968">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="4ad1d-969">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="4ad1d-969">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-970">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-970">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-971">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-971">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="4ad1d-972">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-972">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="4ad1d-973">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="4ad1d-973">Az.ContainerInstance</span></span>
* <span data-ttu-id="4ad1d-974">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="4ad1d-974">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="4ad1d-975">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="4ad1d-975">Az.DataFactory</span></span>
* <span data-ttu-id="4ad1d-976">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="4ad1d-976">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="4ad1d-977">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-977">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-978">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-978">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-979">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-979">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="4ad1d-980">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-980">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="4ad1d-981">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="4ad1d-981">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="4ad1d-982">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="4ad1d-982">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="4ad1d-983">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="4ad1d-983">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="4ad1d-984">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="4ad1d-984">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-985">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-985">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-986">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-986">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="4ad1d-987">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-987">Az.Storage</span></span>
* <span data-ttu-id="4ad1d-988">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="4ad1d-988">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="4ad1d-989">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="4ad1d-989">New-AzStorageContext</span></span>
* <span data-ttu-id="4ad1d-990">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="4ad1d-990">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="4ad1d-991">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="4ad1d-991">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="4ad1d-992">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="4ad1d-992">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="4ad1d-993">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="4ad1d-993">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="4ad1d-994">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="4ad1d-994">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="4ad1d-995">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="4ad1d-995">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="4ad1d-996">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="4ad1d-996">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="4ad1d-997">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="4ad1d-997">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="4ad1d-998">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="4ad1d-998">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="4ad1d-999">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="4ad1d-999">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="4ad1d-1000">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1000">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="4ad1d-1001">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1001">Highlights since the last major release</span></span>
* <span data-ttu-id="4ad1d-1002">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1002">General availability of `Az` module</span></span>
* <span data-ttu-id="4ad1d-1003">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1003">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="4ad1d-1004">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1004">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="4ad1d-1005">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1005">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="4ad1d-1006">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1006">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="4ad1d-1007">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1007">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="4ad1d-1008">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1008">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="4ad1d-1009">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1009">Az.Automation</span></span>
* <span data-ttu-id="4ad1d-1010">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1010">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="4ad1d-1011">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1011">Dynamic grouping</span></span>
    * <span data-ttu-id="4ad1d-1012">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1012">Pre-Post script</span></span>
    * <span data-ttu-id="4ad1d-1013">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1013">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-1014">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1014">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-1015">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1015">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="4ad1d-1016">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1016">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="4ad1d-1017">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1017">Az.KeyVault</span></span>
* <span data-ttu-id="4ad1d-1018">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1018">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-1019">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1019">Az.Network</span></span>
* <span data-ttu-id="4ad1d-1020">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1020">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="4ad1d-1021">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1021">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="4ad1d-1022">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1022">Az.RecoveryServices</span></span>
* <span data-ttu-id="4ad1d-1023">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1023">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="4ad1d-1024">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1024">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-1025">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1025">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-1026">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1026">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="4ad1d-1027">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1027">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-1028">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1028">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-1029">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1029">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="4ad1d-1030">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1030">Az.Storage</span></span>
* <span data-ttu-id="4ad1d-1031">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1031">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="4ad1d-1032">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1032">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="4ad1d-1033">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1033">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="4ad1d-1034">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1034">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="4ad1d-1035">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1035">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="4ad1d-1036">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1036">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="4ad1d-1037">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1037">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="4ad1d-1038">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1038">Az.Websites</span></span>
* <span data-ttu-id="4ad1d-1039">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1039">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="4ad1d-1040">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1040">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="4ad1d-1041">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1041">Az.Accounts</span></span>
* <span data-ttu-id="4ad1d-1042">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1042">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="4ad1d-1043">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1043">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="4ad1d-1044">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1044">Az.Automation</span></span>
* <span data-ttu-id="4ad1d-1045">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1045">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="4ad1d-1046">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1046">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="4ad1d-1047">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1047">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="4ad1d-1048">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1048">Az.Cdn</span></span>
* <span data-ttu-id="4ad1d-1049">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1049">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-1050">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1050">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-1051">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1051">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="4ad1d-1052">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1052">Az.DataFactory</span></span>
* <span data-ttu-id="4ad1d-1053">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1053">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="4ad1d-1054">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1054">Az.LogicApp</span></span>
* <span data-ttu-id="4ad1d-1055">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1055">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-1056">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1056">Az.Network</span></span>
* <span data-ttu-id="4ad1d-1057">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1057">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="4ad1d-1058">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1058">Az.RecoveryServices</span></span>
* <span data-ttu-id="4ad1d-1059">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1059">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="4ad1d-1060">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1060">SDK Update</span></span>
* <span data-ttu-id="4ad1d-1061">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1061">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="4ad1d-1062">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1062">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-1063">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1063">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-1064">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1064">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="4ad1d-1065">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1065">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="4ad1d-1066">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1066">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="4ad1d-1067">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1067">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="4ad1d-1068">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1068">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="4ad1d-1069">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1069">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-1070">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1070">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-1071">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1071">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="4ad1d-1072">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1072">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="4ad1d-1073">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1073">Az.Storage</span></span>
* <span data-ttu-id="4ad1d-1074">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1074">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="4ad1d-1075">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1075">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="4ad1d-1076">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1076">Az.AnalysisServices</span></span>
* <span data-ttu-id="4ad1d-1077">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1077">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="4ad1d-1078">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1078">Az.Automation</span></span>
* <span data-ttu-id="4ad1d-1079">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1079">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="4ad1d-1080">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1080">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="4ad1d-1081">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1081">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="4ad1d-1082">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1082">Az.CognitiveServices</span></span>
* <span data-ttu-id="4ad1d-1083">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1083">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-1084">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1084">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-1085">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1085">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="4ad1d-1086">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1086">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="4ad1d-1087">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1087">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="4ad1d-1088">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1088">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="4ad1d-1089">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1089">Az.DataLakeStore</span></span>
* <span data-ttu-id="4ad1d-1090">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1090">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="4ad1d-1091">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1091">Az.EventHub</span></span>
* <span data-ttu-id="4ad1d-1092">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1092">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="4ad1d-1093">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1093">Az.KeyVault</span></span>
* <span data-ttu-id="4ad1d-1094">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1094">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="4ad1d-1095">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1095">Az.LogicApp</span></span>
* <span data-ttu-id="4ad1d-1096">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1096">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="4ad1d-1097">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1097">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="4ad1d-1098">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1098">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="4ad1d-1099">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1099">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="4ad1d-1100">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1100">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="4ad1d-1101">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1101">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="4ad1d-1102">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1102">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="4ad1d-1103">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1103">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="4ad1d-1104">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1104">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="4ad1d-1105">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1105">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="4ad1d-1106">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1106">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="4ad1d-1107">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1107">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="4ad1d-1108">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1108">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="4ad1d-1109">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1109">Az.Monitor</span></span>
* <span data-ttu-id="4ad1d-1110">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1110">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-1111">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1111">Az.Network</span></span>
* <span data-ttu-id="4ad1d-1112">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1112">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="4ad1d-1113">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1113">Az.OperationalInsights</span></span>
* <span data-ttu-id="4ad1d-1114">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1114">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="4ad1d-1115">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1115">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="4ad1d-1116">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1116">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="4ad1d-1117">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1117">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-1118">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1118">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="4ad1d-1119">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1119">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="4ad1d-1120">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1120">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="4ad1d-1121">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1121">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-1122">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1122">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-1123">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1123">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="4ad1d-1124">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1124">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="4ad1d-1125">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1125">Az.Websites</span></span>
* <span data-ttu-id="4ad1d-1126">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1126">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="4ad1d-1127">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1127">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="4ad1d-1128">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1128">Az.Accounts</span></span>
* <span data-ttu-id="4ad1d-1129">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1129">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="4ad1d-1130">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1130">Az.AnalysisServices</span></span>
<span data-ttu-id="4ad1d-1131">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1131">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-1132">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1132">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-1133">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1133">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="4ad1d-1134">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1134">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="4ad1d-1135">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1135">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="4ad1d-1136">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1136">Az.RecoveryServices</span></span>
<span data-ttu-id="4ad1d-1137">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1137">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-1138">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1138">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-1139">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1139">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="4ad1d-1140">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1140">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="4ad1d-1141">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1141">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="4ad1d-1142">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1142">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-1143">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1143">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-1144">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1144">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="4ad1d-1145">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1145">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="4ad1d-1146">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1146">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="4ad1d-1147">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1147">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="4ad1d-1148">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1148">Az.Accounts</span></span>
* <span data-ttu-id="4ad1d-1149">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1149">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="4ad1d-1150">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1150">Az.AnalysisServices</span></span>
* <span data-ttu-id="4ad1d-1151">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1151">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="4ad1d-1152">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1152">Az.RecoveryServices</span></span>
* <span data-ttu-id="4ad1d-1153">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1153">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="4ad1d-1154">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1154">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="4ad1d-1155">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1155">Az.Accounts</span></span>
* <span data-ttu-id="4ad1d-1156">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1156">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="4ad1d-1157">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1157">Update incorrect online help URLs</span></span>
* <span data-ttu-id="4ad1d-1158">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1158">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="4ad1d-1159">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1159">Az.Aks</span></span>
* <span data-ttu-id="4ad1d-1160">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1160">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="4ad1d-1161">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1161">Az.Automation</span></span>
* <span data-ttu-id="4ad1d-1162">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1162">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="4ad1d-1163">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1163">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="4ad1d-1164">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1164">Az.Cdn</span></span>
* <span data-ttu-id="4ad1d-1165">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1165">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-1166">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1166">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-1167">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1167">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="4ad1d-1168">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1168">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="4ad1d-1169">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1169">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="4ad1d-1170">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1170">Az.ContainerRegistry</span></span>
* <span data-ttu-id="4ad1d-1171">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1171">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="4ad1d-1172">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1172">Az.DataFactory</span></span>
* <span data-ttu-id="4ad1d-1173">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1173">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="4ad1d-1174">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1174">Az.DataLakeStore</span></span>
* <span data-ttu-id="4ad1d-1175">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1175">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="4ad1d-1176">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1176">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="4ad1d-1177">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1177">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="4ad1d-1178">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1178">Az.IotHub</span></span>
* <span data-ttu-id="4ad1d-1179">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1179">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="4ad1d-1180">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1180">Az.KeyVault</span></span>
* <span data-ttu-id="4ad1d-1181">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1181">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-1182">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1182">Az.Network</span></span>
* <span data-ttu-id="4ad1d-1183">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1183">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-1184">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1184">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-1185">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1185">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="4ad1d-1186">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1186">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="4ad1d-1187">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1187">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="4ad1d-1188">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1188">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="4ad1d-1189">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1189">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="4ad1d-1190">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1190">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="4ad1d-1191">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1191">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="4ad1d-1192">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1192">Az.ServiceFabric</span></span>
* <span data-ttu-id="4ad1d-1193">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1193">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="4ad1d-1194">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1194">Fix some error messages.</span></span>
* <span data-ttu-id="4ad1d-1195">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1195">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="4ad1d-1196">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1196">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="4ad1d-1197">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1197">Az.SignalR</span></span>
* <span data-ttu-id="4ad1d-1198">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1198">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-1199">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1199">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-1200">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1200">Update incorrect online help URLs</span></span>
* <span data-ttu-id="4ad1d-1201">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1201">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="4ad1d-1202">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1202">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="4ad1d-1203">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1203">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="4ad1d-1204">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1204">Az.Storage</span></span>
* <span data-ttu-id="4ad1d-1205">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1205">Update incorrect online help URLs</span></span>
* <span data-ttu-id="4ad1d-1206">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1206">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="4ad1d-1207">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1207">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="4ad1d-1208">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1208">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="4ad1d-1209">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1209">Az.TrafficManager</span></span>
* <span data-ttu-id="4ad1d-1210">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1210">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="4ad1d-1211">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1211">Az.Websites</span></span>
* <span data-ttu-id="4ad1d-1212">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1212">Update incorrect online help URLs</span></span>
* <span data-ttu-id="4ad1d-1213">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1213">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="4ad1d-1214">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1214">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="4ad1d-1215">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1215">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="4ad1d-1216">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1216">Az.Accounts</span></span>
* <span data-ttu-id="4ad1d-1217">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1217">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-1218">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1218">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-1219">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1219">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="4ad1d-1220">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1220">Updated the description of ID in help files</span></span>
* <span data-ttu-id="4ad1d-1221">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1221">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="4ad1d-1222">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1222">Az.DataLakeStore</span></span>
* <span data-ttu-id="4ad1d-1223">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1223">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="4ad1d-1224">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1224">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="4ad1d-1225">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1225">Az.EventGrid</span></span>
* <span data-ttu-id="4ad1d-1226">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1226">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="4ad1d-1227">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1227">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="4ad1d-1228">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1228">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="4ad1d-1229">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1229">Event Time-To-Live,</span></span>
        - <span data-ttu-id="4ad1d-1230">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1230">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="4ad1d-1231">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1231">Dead letter endpoint.</span></span>
    - <span data-ttu-id="4ad1d-1232">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1232">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="4ad1d-1233">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1233">Event Time-To-Live,</span></span>
        - <span data-ttu-id="4ad1d-1234">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1234">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="4ad1d-1235">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1235">Dead letter endpoint.</span></span>
* <span data-ttu-id="4ad1d-1236">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1236">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="4ad1d-1237">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1237">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="4ad1d-1238">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1238">Az.IotHub</span></span>
* <span data-ttu-id="4ad1d-1239">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1239">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="4ad1d-1240">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1240">Az.LogicApp</span></span>
* <span data-ttu-id="4ad1d-1241">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1241">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-1242">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1242">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-1243">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1243">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="4ad1d-1244">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1244">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="4ad1d-1245">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1245">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="4ad1d-1246">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1246">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="4ad1d-1247">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1247">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="4ad1d-1248">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1248">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="4ad1d-1249">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1249">Az.SignalR</span></span>
* <span data-ttu-id="4ad1d-1250">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1250">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-1251">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1251">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-1252">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1252">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="4ad1d-1253">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1253">Az.Storage</span></span>
* <span data-ttu-id="4ad1d-1254">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1254">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="4ad1d-1255">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1255">New-AzStorageContext</span></span>
* <span data-ttu-id="4ad1d-1256">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1256">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="4ad1d-1257">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1257">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="4ad1d-1258">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1258">Az.Websites</span></span>
* <span data-ttu-id="4ad1d-1259">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1259">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="4ad1d-1260">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1260">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="4ad1d-1261">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1261">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="4ad1d-1262">Geral</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1262">General</span></span>

- <span data-ttu-id="4ad1d-1263">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1263">General Availability of Az Module</span></span>
- <span data-ttu-id="4ad1d-1264">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1264">Online help for each module</span></span>
- <span data-ttu-id="4ad1d-1265">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1265">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="4ad1d-1266">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1266">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="4ad1d-1267">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1267">Az.Accounts</span></span>
- <span data-ttu-id="4ad1d-1268">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1268">Changed from Az.Profile</span></span>
- <span data-ttu-id="4ad1d-1269">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1269">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="4ad1d-1270">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1270">Az.ApiManagement</span></span>
- <span data-ttu-id="4ad1d-1271">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1271">Fixes for #7002</span></span>
- <span data-ttu-id="4ad1d-1272">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1272">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="4ad1d-1273">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1273">Az.Batch</span></span>
- <span data-ttu-id="4ad1d-1274">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1274">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="4ad1d-1275">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1275">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="4ad1d-1276">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1276">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="4ad1d-1277">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1277">Az.Billing</span></span>
- <span data-ttu-id="4ad1d-1278">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1278">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="4ad1d-1279">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1279">Az.CognitivServices</span></span>
- <span data-ttu-id="4ad1d-1280">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1280">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="4ad1d-1281">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1281">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="4ad1d-1282">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1282">Az.ContainerInstance</span></span>
- <span data-ttu-id="4ad1d-1283">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1283">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="4ad1d-1284">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1284">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="4ad1d-1285">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1285">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="4ad1d-1286">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1286">Az.DataLakeStore</span></span>
- <span data-ttu-id="4ad1d-1287">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1287">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="4ad1d-1288">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1288">Az.Monitor</span></span>
- <span data-ttu-id="4ad1d-1289">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1289">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="4ad1d-1290">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1290">Az.KeyVault</span></span>
- <span data-ttu-id="4ad1d-1291">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1291">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="4ad1d-1292">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1292">Az.MachineLearning</span></span>
- <span data-ttu-id="4ad1d-1293">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1293">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="4ad1d-1294">Az.Media</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1294">Az.Media</span></span>
- <span data-ttu-id="4ad1d-1295">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1295">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="4ad1d-1296">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1296">Az.Network</span></span>
<span data-ttu-id="4ad1d-1297">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1297">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="4ad1d-1298">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1298">New cmdlets added:</span></span>
        - <span data-ttu-id="4ad1d-1299">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1299">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="4ad1d-1300">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1300">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="4ad1d-1301">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1301">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="4ad1d-1302">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1302">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="4ad1d-1303">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1303">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="4ad1d-1304">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1304">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="4ad1d-1305">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1305">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="4ad1d-1306">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1306">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="4ad1d-1307">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1307">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="4ad1d-1308">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1308">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="4ad1d-1309">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1309">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="4ad1d-1310">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1310">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="4ad1d-1311">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1311">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="4ad1d-1312">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1312">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="4ad1d-1313">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1313">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="4ad1d-1314">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1314">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="4ad1d-1315">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1315">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="4ad1d-1316">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1316">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="4ad1d-1317">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1317">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="4ad1d-1318">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1318">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="4ad1d-1319">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1319">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="4ad1d-1320">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1320">Az.OperationalInsights</span></span>
- <span data-ttu-id="4ad1d-1321">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1321">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="4ad1d-1322">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1322">Az.Profile</span></span>
- <span data-ttu-id="4ad1d-1323">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1323">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="4ad1d-1324">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1324">Az.RecoveryServices</span></span>
- <span data-ttu-id="4ad1d-1325">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1325">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="4ad1d-1326">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1326">Az.Resources</span></span>
- <span data-ttu-id="4ad1d-1327">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1327">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="4ad1d-1328">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1328">Az.ServiceFabric</span></span>
- <span data-ttu-id="4ad1d-1329">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1329">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="4ad1d-1330">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1330">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="4ad1d-1331">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1331">Az.SIgnalR</span></span>
- <span data-ttu-id="4ad1d-1332">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1332">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="4ad1d-1333">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1333">Az.Sql</span></span>
- <span data-ttu-id="4ad1d-1334">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1334">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="4ad1d-1335">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1335">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="4ad1d-1336">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1336">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="4ad1d-1337">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1337">Az.Storage</span></span>
- <span data-ttu-id="4ad1d-1338">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1338">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="4ad1d-1339">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1339">Az.Websites</span></span>
- <span data-ttu-id="4ad1d-1340">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1340">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="4ad1d-1341">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1341">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="4ad1d-1342">Geral</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1342">General</span></span>

* <span data-ttu-id="4ad1d-1343">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1343">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="4ad1d-1344">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1344">Az.Compute</span></span>

* <span data-ttu-id="4ad1d-1345">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1345">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="4ad1d-1346">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1346">Az.DataLakeStore</span></span>

* <span data-ttu-id="4ad1d-1347">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1347">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="4ad1d-1348">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1348">Az.FrontDoor</span></span>

* <span data-ttu-id="4ad1d-1349">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1349">Fixed some broken links</span></span>
    - <span data-ttu-id="4ad1d-1350">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1350">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="4ad1d-1351">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1351">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="4ad1d-1352">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1352">Az.RecoveryServices</span></span>

* <span data-ttu-id="4ad1d-1353">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1353">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="4ad1d-1354">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1354">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="4ad1d-1355">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1355">Az.Resources</span></span>

* <span data-ttu-id="4ad1d-1356">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1356">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="4ad1d-1357">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1357">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="4ad1d-1358">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1358">Az.Sql</span></span>

* <span data-ttu-id="4ad1d-1359">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1359">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="4ad1d-1360">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1360">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="4ad1d-1361">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1361">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="4ad1d-1362">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1362">Az.Storage</span></span>

* <span data-ttu-id="4ad1d-1363">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1363">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="4ad1d-1364">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1364">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="4ad1d-1365">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1365">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="4ad1d-1366">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1366">Support Static Website configuration</span></span>
    - <span data-ttu-id="4ad1d-1367">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1367">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="4ad1d-1368">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1368">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="4ad1d-1369">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1369">Az.Websites</span></span>

* <span data-ttu-id="4ad1d-1370">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1370">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="4ad1d-1371">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1371">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="4ad1d-1372">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1372">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="4ad1d-1373">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1373">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="4ad1d-1374">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1374">Az.ApiManagement</span></span>
* <span data-ttu-id="4ad1d-1375">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1375">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="4ad1d-1376">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1376">Az.Automation</span></span>
* <span data-ttu-id="4ad1d-1377">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1377">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="4ad1d-1378">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1378">Added Update Management cmdlets</span></span>
* <span data-ttu-id="4ad1d-1379">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1379">Added Source Control cmdlets</span></span>
* <span data-ttu-id="4ad1d-1380">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1380">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="4ad1d-1381">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1381">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="4ad1d-1382">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1382">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-1383">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1383">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="4ad1d-1384">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1384">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="4ad1d-1385">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1385">Az.ContainerInstance</span></span>
* <span data-ttu-id="4ad1d-1386">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1386">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="4ad1d-1387">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1387">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="4ad1d-1388">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1388">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="4ad1d-1389">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1389">Az.Network</span></span>
* <span data-ttu-id="4ad1d-1390">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1390">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="4ad1d-1391">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1391">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="4ad1d-1392">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1392">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="4ad1d-1393">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1393">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="4ad1d-1394">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1394">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="4ad1d-1395">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1395">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="4ad1d-1396">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1396">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="4ad1d-1397">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1397">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="4ad1d-1398">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1398">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="4ad1d-1399">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1399">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="4ad1d-1400">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1400">Az.Relay</span></span>
* <span data-ttu-id="4ad1d-1401">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1401">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="4ad1d-1402">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1402">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-1403">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1403">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="4ad1d-1404">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1404">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="4ad1d-1405">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1405">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="4ad1d-1406">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1406">Az.ServiceFabric</span></span>
* <span data-ttu-id="4ad1d-1407">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1407">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="4ad1d-1408">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1408">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-1409">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1409">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="4ad1d-1410">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1410">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="4ad1d-1411">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1411">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="4ad1d-1412">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1412">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="4ad1d-1413">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1413">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="4ad1d-1414">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1414">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="4ad1d-1415">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1415">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="4ad1d-1416">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1416">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="4ad1d-1417">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1417">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="4ad1d-1418">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1418">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="4ad1d-1419">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1419">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="4ad1d-1420">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1420">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="4ad1d-1421">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1421">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="4ad1d-1422">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1422">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="4ad1d-1423">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1423">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="4ad1d-1424">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1424">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="4ad1d-1425">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1425">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="4ad1d-1426">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1426">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="4ad1d-1427">Geral</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1427">General</span></span>
* <span data-ttu-id="4ad1d-1428">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1428">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="4ad1d-1429">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1429">Az.Profile</span></span>
* <span data-ttu-id="4ad1d-1430">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1430">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="4ad1d-1431">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1431">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="4ad1d-1432">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1432">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="4ad1d-1433">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1433">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="4ad1d-1434">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1434">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="4ad1d-1435">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1435">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="4ad1d-1436">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1436">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="4ad1d-1437">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1437">Az.CognitiveServices</span></span>
* <span data-ttu-id="4ad1d-1438">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1438">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-1439">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1439">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-1440">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1440">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="4ad1d-1441">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1441">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="4ad1d-1442">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1442">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="4ad1d-1443">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1443">Az.DataLakeStore</span></span>
* <span data-ttu-id="4ad1d-1444">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1444">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="4ad1d-1445">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1445">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="4ad1d-1446">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1446">Az.Insights</span></span>
* <span data-ttu-id="4ad1d-1447">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1447">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="4ad1d-1448">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1448">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="4ad1d-1449">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1449">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="4ad1d-1450">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1450">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-1451">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1451">Az.Network</span></span>
* <span data-ttu-id="4ad1d-1452">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1452">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="4ad1d-1453">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1453">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="4ad1d-1454">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1454">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="4ad1d-1455">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1455">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="4ad1d-1456">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1456">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="4ad1d-1457">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1457">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="4ad1d-1458">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1458">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="4ad1d-1459">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1459">Az.PolicyInsights</span></span>
* <span data-ttu-id="4ad1d-1460">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1460">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-1461">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1461">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-1462">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1462">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="4ad1d-1463">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1463">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="4ad1d-1464">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1464">Az.ServiceBus</span></span>
* <span data-ttu-id="4ad1d-1465">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1465">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="4ad1d-1466">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1466">Az.ServiceFabric</span></span>
* <span data-ttu-id="4ad1d-1467">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1467">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="4ad1d-1468">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1468">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="4ad1d-1469">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1469">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="4ad1d-1470">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1470">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="4ad1d-1471">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1471">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="4ad1d-1472">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1472">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="4ad1d-1473">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1473">Az.Profile</span></span>
* <span data-ttu-id="4ad1d-1474">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1474">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="4ad1d-1475">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1475">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-1476">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1476">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-1477">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1477">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="4ad1d-1478">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1478">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="4ad1d-1479">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1479">Az.DataLakeStore</span></span>
* <span data-ttu-id="4ad1d-1480">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1480">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="4ad1d-1481">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1481">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="4ad1d-1482">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1482">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="4ad1d-1483">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1483">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="4ad1d-1484">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1484">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-1485">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1485">Az.Network</span></span>
* <span data-ttu-id="4ad1d-1486">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1486">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="4ad1d-1487">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1487">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-1488">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1488">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-1489">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1489">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="4ad1d-1490">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1490">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="4ad1d-1491">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1491">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="4ad1d-1492">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1492">Azure.Storage</span></span>
* <span data-ttu-id="4ad1d-1493">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1493">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="4ad1d-1494">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1494">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="4ad1d-1495">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1495">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="4ad1d-1496">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1496">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="4ad1d-1497">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1497">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="4ad1d-1498">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1498">Az.CognitiveServices</span></span>
* <span data-ttu-id="4ad1d-1499">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1499">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="4ad1d-1500">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1500">Az.Compute</span></span>
* <span data-ttu-id="4ad1d-1501">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1501">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="4ad1d-1502">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1502">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="4ad1d-1503">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1503">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="4ad1d-1504">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1504">Az.DataFactoryV2</span></span>
* <span data-ttu-id="4ad1d-1505">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1505">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="4ad1d-1506">Az.Network</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1506">Az.Network</span></span>
* <span data-ttu-id="4ad1d-1507">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1507">Added NetworkProfile functionality.</span></span> <span data-ttu-id="4ad1d-1508">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1508">new cmdlets added</span></span>
    - <span data-ttu-id="4ad1d-1509">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1509">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="4ad1d-1510">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1510">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="4ad1d-1511">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1511">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="4ad1d-1512">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1512">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="4ad1d-1513">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1513">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="4ad1d-1514">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1514">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="4ad1d-1515">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1515">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="4ad1d-1516">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1516">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="4ad1d-1517">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1517">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="4ad1d-1518">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1518">Az.RedisCache</span></span>
* <span data-ttu-id="4ad1d-1519">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1519">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="4ad1d-1520">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1520">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="4ad1d-1521">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1521">Az.Resources</span></span>
* <span data-ttu-id="4ad1d-1522">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1522">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="4ad1d-1523">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1523">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="4ad1d-1524">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1524">Az.Sql</span></span>
* <span data-ttu-id="4ad1d-1525">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1525">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="4ad1d-1526">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1526">Az.Websites</span></span>
* <span data-ttu-id="4ad1d-1527">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1527">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="4ad1d-1528">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1528">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="4ad1d-1529">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1529">0.2.0 - September 2018</span></span>
 <span data-ttu-id="4ad1d-1530">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="4ad1d-1530">Initial Release</span></span>
