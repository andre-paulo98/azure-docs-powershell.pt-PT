---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/15/2019
ms.openlocfilehash: bcbb78809c2db63d665dc0c3d05e0614acce6045
ms.sourcegitcommit: 9f5c7d231b069ad501729bf015a829f3fe89bc6a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/28/2020
ms.locfileid: "84122162"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="32ae3-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="32ae3-103">Azure PowerShell release notes</span></span>
## <a name="280---october-2019"></a><span data-ttu-id="32ae3-104">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-104">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="32ae3-105">Geral</span><span class="sxs-lookup"><span data-stu-id="32ae3-105">General</span></span>
* <span data-ttu-id="32ae3-106">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="32ae3-106">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="32ae3-107">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-107">Az.Accounts</span></span>
* <span data-ttu-id="32ae3-108">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="32ae3-108">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="32ae3-109">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="32ae3-109">Az.ApiManagement</span></span>
* <span data-ttu-id="32ae3-110">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="32ae3-110">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="32ae3-111">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="32ae3-111">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="32ae3-112">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="32ae3-112">Az.Automation</span></span>
* <span data-ttu-id="32ae3-113">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="32ae3-113">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="32ae3-114">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="32ae3-114">Az.Batch</span></span>
* <span data-ttu-id="32ae3-115">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="32ae3-115">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-116">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-116">Az.Compute</span></span>
* <span data-ttu-id="32ae3-117">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="32ae3-117">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="32ae3-118">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="32ae3-118">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="32ae3-119">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="32ae3-119">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="32ae3-120">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="32ae3-120">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="32ae3-121">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="32ae3-121">Az.DataFactory</span></span>
* <span data-ttu-id="32ae3-122">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="32ae3-122">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="32ae3-123">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="32ae3-123">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="32ae3-124">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="32ae3-124">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="32ae3-125">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="32ae3-125">Az.DataLakeStore</span></span>
* <span data-ttu-id="32ae3-126">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="32ae3-126">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="32ae3-127">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="32ae3-127">Az.HealthcareApis</span></span>
* <span data-ttu-id="32ae3-128">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="32ae3-128">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="32ae3-129">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="32ae3-129">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="32ae3-130">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="32ae3-130">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="32ae3-131">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="32ae3-131">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="32ae3-132">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="32ae3-132">Az.IotHub</span></span>
* <span data-ttu-id="32ae3-133">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="32ae3-133">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="32ae3-134">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="32ae3-134">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="32ae3-135">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="32ae3-135">Az.Monitor</span></span>
* <span data-ttu-id="32ae3-136">Foram adicionados novos recetores de grupos de ações para New-AzActionGroupReceiver:   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="32ae3-136">New action group receivers added for New-AzActionGroupReceiver:   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="32ae3-137">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="32ae3-137">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="32ae3-138">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="32ae3-138">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="32ae3-139">Os webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="32ae3-139">Webhooks now supports Azure active directory authentication.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-140">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-140">Az.Network</span></span>
* <span data-ttu-id="32ae3-141">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="32ae3-141">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="32ae3-142">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="32ae3-142">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="32ae3-143">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="32ae3-143">New cmdlets added:</span></span>
        - <span data-ttu-id="32ae3-144">New-AzIpsecTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="32ae3-144">New-AzIpsecTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="32ae3-145">Foram atualizados cmdlets com o parâmetro opcional -TrafficSelectorPolicies</span><span class="sxs-lookup"><span data-stu-id="32ae3-145">Cmdlets updated with optional parameter -TrafficSelectorPolicies</span></span>
        - <span data-ttu-id="32ae3-146">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="32ae3-146">New-AzVirtualNetworkGatewayConnection</span></span>
        - <span data-ttu-id="32ae3-147">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="32ae3-147">Set-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="32ae3-148">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="32ae3-148">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="32ae3-149">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="32ae3-149">Updated cmdlets:</span></span>
        - <span data-ttu-id="32ae3-150">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-150">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="32ae3-151">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-151">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="32ae3-152">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-152">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="32ae3-153">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="32ae3-153">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="32ae3-154">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="32ae3-154">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="32ae3-155">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="32ae3-155">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="32ae3-156">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="32ae3-156">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="32ae3-157">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="32ae3-157">Az.RedisCache</span></span>
* <span data-ttu-id="32ae3-158">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="32ae3-158">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-159">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-159">Az.Sql</span></span>
* <span data-ttu-id="32ae3-160">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="32ae3-160">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="32ae3-161">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="32ae3-161">Az.Storage</span></span>
* <span data-ttu-id="32ae3-162">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="32ae3-162">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="32ae3-163">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="32ae3-163">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="32ae3-164">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="32ae3-164">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="32ae3-165">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="32ae3-165">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="32ae3-166">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="32ae3-166">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="32ae3-167">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="32ae3-167">Az.StorageSync</span></span>
* <span data-ttu-id="32ae3-168">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="32ae3-168">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="32ae3-169">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="32ae3-169">Az.Websites</span></span>
* <span data-ttu-id="32ae3-170">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="32ae3-170">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="32ae3-171">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-171">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="32ae3-172">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="32ae3-172">Az.ApiManagement</span></span>
* <span data-ttu-id="32ae3-173">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="32ae3-173">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="32ae3-174">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="32ae3-174">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="32ae3-175">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="32ae3-175">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="32ae3-176">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="32ae3-176">Az.Automation</span></span>
* <span data-ttu-id="32ae3-177">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="32ae3-177">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="32ae3-178">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="32ae3-178">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="32ae3-179">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="32ae3-179">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-180">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-180">Az.Compute</span></span>
* <span data-ttu-id="32ae3-181">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-181">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="32ae3-182">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-182">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="32ae3-183">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="32ae3-183">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="32ae3-184">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="32ae3-184">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="32ae3-185">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="32ae3-185">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="32ae3-186">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="32ae3-186">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="32ae3-187">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="32ae3-187">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="32ae3-188">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="32ae3-188">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="32ae3-189">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="32ae3-189">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="32ae3-190">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="32ae3-190">Az.DataFactory</span></span>
* <span data-ttu-id="32ae3-191">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="32ae3-191">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="32ae3-192">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="32ae3-192">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="32ae3-193">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="32ae3-193">Az.HDInsight</span></span>
* <span data-ttu-id="32ae3-194">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="32ae3-194">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="32ae3-195">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="32ae3-195">Az.IotHub</span></span>
* <span data-ttu-id="32ae3-196">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="32ae3-196">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="32ae3-197">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="32ae3-197">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="32ae3-198">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="32ae3-198">New cmdlets are:</span></span>
    - <span data-ttu-id="32ae3-199">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="32ae3-199">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="32ae3-200">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="32ae3-200">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="32ae3-201">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="32ae3-201">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="32ae3-202">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="32ae3-202">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="32ae3-203">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="32ae3-203">Az.Monitor</span></span>
* <span data-ttu-id="32ae3-204">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="32ae3-204">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="32ae3-205">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="32ae3-205">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="32ae3-206">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="32ae3-206">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="32ae3-207">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="32ae3-207">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="32ae3-208">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="32ae3-208">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="32ae3-209">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="32ae3-209">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="32ae3-210">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="32ae3-210">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="32ae3-211">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="32ae3-211">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="32ae3-212">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="32ae3-212">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="32ae3-213">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="32ae3-213">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="32ae3-214">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="32ae3-214">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="32ae3-215">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="32ae3-215">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="32ae3-216">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="32ae3-216">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="32ae3-217">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="32ae3-217">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="32ae3-218">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="32ae3-218">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="32ae3-219">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="32ae3-219">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="32ae3-220">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="32ae3-220">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="32ae3-221">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="32ae3-221">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="32ae3-222">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="32ae3-222">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="32ae3-223">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="32ae3-223">Overall improved help files</span></span>
* <span data-ttu-id="32ae3-224">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="32ae3-224">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-225">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-225">Az.Network</span></span>
* <span data-ttu-id="32ae3-226">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="32ae3-226">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="32ae3-227">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="32ae3-227">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="32ae3-228">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="32ae3-228">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="32ae3-229">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="32ae3-229">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="32ae3-230">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="32ae3-230">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="32ae3-231">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="32ae3-231">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="32ae3-232">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="32ae3-232">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="32ae3-233">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="32ae3-233">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="32ae3-234">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="32ae3-234">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="32ae3-235">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="32ae3-235">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="32ae3-236">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="32ae3-236">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="32ae3-237">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="32ae3-237">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="32ae3-238">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="32ae3-238">New cmdlets</span></span>
        - <span data-ttu-id="32ae3-239">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="32ae3-239">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="32ae3-240">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="32ae3-240">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="32ae3-241">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="32ae3-241">Updated cmdlet:</span></span>
        - <span data-ttu-id="32ae3-242">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="32ae3-242">New-VpnSite</span></span>
        - <span data-ttu-id="32ae3-243">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="32ae3-243">Update-VpnSite</span></span>
        - <span data-ttu-id="32ae3-244">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="32ae3-244">New-VpnConnection</span></span>
        - <span data-ttu-id="32ae3-245">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="32ae3-245">Update-VpnConnection</span></span>
* <span data-ttu-id="32ae3-246">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="32ae3-246">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="32ae3-247">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-247">Az.RecoveryServices</span></span>
* <span data-ttu-id="32ae3-248">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="32ae3-248">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="32ae3-249">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="32ae3-249">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-250">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-250">Az.Resources</span></span>
* <span data-ttu-id="32ae3-251">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="32ae3-251">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="32ae3-252">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="32ae3-252">Az.ServiceFabric</span></span>
* <span data-ttu-id="32ae3-253">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="32ae3-253">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="32ae3-254">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="32ae3-254">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="32ae3-255">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="32ae3-255">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="32ae3-256">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="32ae3-256">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="32ae3-257">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="32ae3-257">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="32ae3-258">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="32ae3-258">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="32ae3-259">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="32ae3-259">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="32ae3-260">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="32ae3-260">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="32ae3-261">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="32ae3-261">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="32ae3-262">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="32ae3-262">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="32ae3-263">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="32ae3-263">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="32ae3-264">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="32ae3-264">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="32ae3-265">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="32ae3-265">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="32ae3-266">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="32ae3-266">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="32ae3-267">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="32ae3-267">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="32ae3-268">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="32ae3-268">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="32ae3-269">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="32ae3-269">Az.SignalR</span></span>
* <span data-ttu-id="32ae3-270">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="32ae3-270">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-271">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-271">Az.Sql</span></span>
* <span data-ttu-id="32ae3-272">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="32ae3-272">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="32ae3-273">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="32ae3-273">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="32ae3-274">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="32ae3-274">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="32ae3-275">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="32ae3-275">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="32ae3-276">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="32ae3-276">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="32ae3-277">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="32ae3-277">Az.Storage</span></span>
* <span data-ttu-id="32ae3-278">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="32ae3-278">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="32ae3-279">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="32ae3-279">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="32ae3-280">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="32ae3-280">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="32ae3-281">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="32ae3-281">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="32ae3-282">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="32ae3-282">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="32ae3-283">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="32ae3-283">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="32ae3-284">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="32ae3-284">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="32ae3-285">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="32ae3-285">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="32ae3-286">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="32ae3-286">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="32ae3-287">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="32ae3-287">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="32ae3-288">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="32ae3-288">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="32ae3-289">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="32ae3-289">Az.Websites</span></span>
* <span data-ttu-id="32ae3-290">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="32ae3-290">Fixing issue where webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="32ae3-291">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="32ae3-291">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="32ae3-292">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="32ae3-292">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="32ae3-293">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-293">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="32ae3-294">Geral</span><span class="sxs-lookup"><span data-stu-id="32ae3-294">General</span></span>
* <span data-ttu-id="32ae3-295">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="32ae3-295">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="32ae3-296">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-296">Az.Accounts</span></span>
* <span data-ttu-id="32ae3-297">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="32ae3-297">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="32ae3-298">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="32ae3-298">Az.Aks</span></span>
* <span data-ttu-id="32ae3-299">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="32ae3-299">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="32ae3-300">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="32ae3-300">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="32ae3-301">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="32ae3-301">Az.ApiManagement</span></span>
* <span data-ttu-id="32ae3-302">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="32ae3-302">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="32ae3-303">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="32ae3-303">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="32ae3-304">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="32ae3-304">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="32ae3-305">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="32ae3-305">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="32ae3-306">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="32ae3-306">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="32ae3-307">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="32ae3-307">Az.Batch</span></span>
* <span data-ttu-id="32ae3-308">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="32ae3-308">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="32ae3-309">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="32ae3-309">Az.Cdn</span></span>
* <span data-ttu-id="32ae3-310">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="32ae3-310">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-311">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-311">Az.Compute</span></span>
* <span data-ttu-id="32ae3-312">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-312">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="32ae3-313">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="32ae3-313">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="32ae3-314">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="32ae3-314">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="32ae3-315">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="32ae3-315">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="32ae3-316">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="32ae3-316">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="32ae3-317">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="32ae3-317">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="32ae3-318">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="32ae3-318">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="32ae3-319">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="32ae3-319">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="32ae3-320">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="32ae3-320">Az.DataFactory</span></span>
* <span data-ttu-id="32ae3-321">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="32ae3-321">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="32ae3-322">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="32ae3-322">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="32ae3-323">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="32ae3-323">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="32ae3-324">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="32ae3-324">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="32ae3-325">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="32ae3-325">Az.DataLakeStore</span></span>
* <span data-ttu-id="32ae3-326">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="32ae3-326">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="32ae3-327">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="32ae3-327">Az.EventHub</span></span>
* <span data-ttu-id="32ae3-328">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="32ae3-328">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="32ae3-329">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="32ae3-329">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="32ae3-330">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="32ae3-330">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="32ae3-331">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="32ae3-331">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="32ae3-332">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="32ae3-332">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="32ae3-333">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="32ae3-333">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="32ae3-334">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="32ae3-334">Az.Monitor</span></span>
* <span data-ttu-id="32ae3-335">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="32ae3-335">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-336">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-336">Az.Network</span></span>
* <span data-ttu-id="32ae3-337">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="32ae3-337">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="32ae3-338">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="32ae3-338">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="32ae3-339">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="32ae3-339">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="32ae3-340">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="32ae3-340">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="32ae3-341">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="32ae3-341">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="32ae3-342">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="32ae3-342">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="32ae3-343">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="32ae3-343">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="32ae3-344">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="32ae3-344">Az.OperationalInsights</span></span>
* <span data-ttu-id="32ae3-345">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="32ae3-345">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="32ae3-346">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="32ae3-346">Added example</span></span>
    - <span data-ttu-id="32ae3-347">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="32ae3-347">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="32ae3-348">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="32ae3-348">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="32ae3-349">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="32ae3-349">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="32ae3-350">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-350">Az.RecoveryServices</span></span>
* <span data-ttu-id="32ae3-351">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="32ae3-351">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-352">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-352">Az.Resources</span></span>
* <span data-ttu-id="32ae3-353">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="32ae3-353">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="32ae3-354">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="32ae3-354">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="32ae3-355">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="32ae3-355">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="32ae3-356">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="32ae3-356">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="32ae3-357">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="32ae3-357">Az.ServiceBus</span></span>
* <span data-ttu-id="32ae3-358">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="32ae3-358">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="32ae3-359">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="32ae3-359">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="32ae3-360">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="32ae3-360">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="32ae3-361">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="32ae3-361">Az.ServiceFabric</span></span>
* <span data-ttu-id="32ae3-362">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="32ae3-362">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="32ae3-363">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="32ae3-363">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="32ae3-364">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="32ae3-364">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="32ae3-365">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="32ae3-365">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="32ae3-366">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="32ae3-366">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="32ae3-367">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="32ae3-367">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-368">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-368">Az.Sql</span></span>
* <span data-ttu-id="32ae3-369">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="32ae3-369">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="32ae3-370">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="32ae3-370">Az.Storage</span></span>
* <span data-ttu-id="32ae3-371">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="32ae3-371">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="32ae3-372">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="32ae3-372">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="32ae3-373">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="32ae3-373">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="32ae3-374">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="32ae3-374">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="32ae3-375">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="32ae3-375">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="32ae3-376">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="32ae3-376">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="32ae3-377">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="32ae3-377">Az.Websites</span></span>
* <span data-ttu-id="32ae3-378">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="32ae3-378">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="32ae3-379">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-379">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="32ae3-380">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-380">Az.Accounts</span></span>
* <span data-ttu-id="32ae3-381">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="32ae3-381">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="32ae3-382">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="32ae3-382">Az.ApplicationInsights</span></span>
* <span data-ttu-id="32ae3-383">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="32ae3-383">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="32ae3-384">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="32ae3-384">Az.Automation</span></span>
* <span data-ttu-id="32ae3-385">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="32ae3-385">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="32ae3-386">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-386">Az.CognitiveServices</span></span>
* <span data-ttu-id="32ae3-387">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="32ae3-387">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-388">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-388">Az.Compute</span></span>
* <span data-ttu-id="32ae3-389">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="32ae3-389">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="32ae3-390">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="32ae3-390">Az.ContainerRegistry</span></span>
* <span data-ttu-id="32ae3-391">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="32ae3-391">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="32ae3-392">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="32ae3-392">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="32ae3-393">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="32ae3-393">Az.DataFactory</span></span>
* <span data-ttu-id="32ae3-394">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="32ae3-394">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="32ae3-395">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="32ae3-395">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="32ae3-396">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="32ae3-396">Az.EventHub</span></span>
* <span data-ttu-id="32ae3-397">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="32ae3-397">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="32ae3-398">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="32ae3-398">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="32ae3-399">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="32ae3-399">Az.KeyVault</span></span>
* <span data-ttu-id="32ae3-400">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="32ae3-400">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="32ae3-401">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="32ae3-401">Az.LogicApp</span></span>
* <span data-ttu-id="32ae3-402">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="32ae3-402">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="32ae3-403">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="32ae3-403">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="32ae3-404">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-404">Az.ManagedServices</span></span>
* <span data-ttu-id="32ae3-405">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="32ae3-405">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-406">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-406">Az.Network</span></span>
* <span data-ttu-id="32ae3-407">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="32ae3-407">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="32ae3-408">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="32ae3-408">New cmdlets</span></span>
        - <span data-ttu-id="32ae3-409">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="32ae3-409">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="32ae3-410">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="32ae3-410">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="32ae3-411">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="32ae3-411">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="32ae3-412">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="32ae3-412">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="32ae3-413">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="32ae3-413">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="32ae3-414">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="32ae3-414">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="32ae3-415">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="32ae3-415">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="32ae3-416">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="32ae3-416">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="32ae3-417">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="32ae3-417">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="32ae3-418">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-418">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="32ae3-419">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="32ae3-419">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="32ae3-420">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="32ae3-420">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="32ae3-421">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="32ae3-421">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="32ae3-422">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="32ae3-422">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="32ae3-423">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="32ae3-423">Updated cmdlets</span></span>
        - <span data-ttu-id="32ae3-424">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-424">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="32ae3-425">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-425">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="32ae3-426">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-426">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="32ae3-427">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="32ae3-427">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="32ae3-428">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="32ae3-428">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="32ae3-429">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="32ae3-429">Updated cmdlet:</span></span>
        - <span data-ttu-id="32ae3-430">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-430">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="32ae3-431">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-431">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="32ae3-432">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-432">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="32ae3-433">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="32ae3-433">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="32ae3-434">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="32ae3-434">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="32ae3-435">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="32ae3-435">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="32ae3-436">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="32ae3-436">Az.OperationalInsights</span></span>
* <span data-ttu-id="32ae3-437">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="32ae3-437">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="32ae3-438">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="32ae3-438">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="32ae3-439">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-439">Az.RecoveryServices</span></span>
* <span data-ttu-id="32ae3-440">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="32ae3-440">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="32ae3-441">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="32ae3-441">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="32ae3-442">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="32ae3-442">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="32ae3-443">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="32ae3-443">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="32ae3-444">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="32ae3-444">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="32ae3-445">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="32ae3-445">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="32ae3-446">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="32ae3-446">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="32ae3-447">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="32ae3-447">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="32ae3-448">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="32ae3-448">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="32ae3-449">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="32ae3-449">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-450">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-450">Az.Resources</span></span>
- <span data-ttu-id="32ae3-451">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="32ae3-451">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="32ae3-452">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="32ae3-452">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="32ae3-453">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="32ae3-453">Az.ServiceBus</span></span>
* <span data-ttu-id="32ae3-454">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="32ae3-454">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="32ae3-455">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="32ae3-455">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-456">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-456">Az.Sql</span></span>
* <span data-ttu-id="32ae3-457">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="32ae3-457">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="32ae3-458">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="32ae3-458">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="32ae3-459">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="32ae3-459">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="32ae3-460">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="32ae3-460">Az.Storage</span></span>
* <span data-ttu-id="32ae3-461">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="32ae3-461">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="32ae3-462">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="32ae3-462">Az.StorageSync</span></span>
* <span data-ttu-id="32ae3-463">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="32ae3-463">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="32ae3-464">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="32ae3-464">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="32ae3-465">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="32ae3-465">Az.Websites</span></span>
* <span data-ttu-id="32ae3-466">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="32ae3-466">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="32ae3-467">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="32ae3-467">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="32ae3-468">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="32ae3-468">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="32ae3-469">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-469">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="32ae3-470">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-470">Az.Accounts</span></span>
* <span data-ttu-id="32ae3-471">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="32ae3-471">Add support for profile cmdlets</span></span>
* <span data-ttu-id="32ae3-472">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="32ae3-472">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="32ae3-473">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="32ae3-473">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="32ae3-474">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="32ae3-474">Az.Advisor</span></span>
* <span data-ttu-id="32ae3-475">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="32ae3-475">GA release of Az.Advisor</span></span>
* <span data-ttu-id="32ae3-476">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="32ae3-476">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="32ae3-477">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="32ae3-477">Az.ApiManagement</span></span>
* <span data-ttu-id="32ae3-478">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="32ae3-478">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="32ae3-479">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="32ae3-479">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="32ae3-480">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="32ae3-480">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="32ae3-481">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="32ae3-481">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="32ae3-482">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="32ae3-482">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="32ae3-483">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="32ae3-483">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="32ae3-484">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="32ae3-484">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="32ae3-485">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="32ae3-485">Az.Automation</span></span>
* <span data-ttu-id="32ae3-486">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="32ae3-486">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-487">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-487">Az.Compute</span></span>
* <span data-ttu-id="32ae3-488">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-488">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="32ae3-489">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="32ae3-489">Az.DataFactory</span></span>
* <span data-ttu-id="32ae3-490">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="32ae3-490">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="32ae3-491">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="32ae3-491">Az.EventGrid</span></span>
* <span data-ttu-id="32ae3-492">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="32ae3-492">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="32ae3-493">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="32ae3-493">Az.IotHub</span></span>
* <span data-ttu-id="32ae3-494">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="32ae3-494">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-495">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-495">Az.Network</span></span>
* <span data-ttu-id="32ae3-496">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="32ae3-496">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="32ae3-497">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="32ae3-497">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="32ae3-498">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="32ae3-498">Az.PolicyInsights</span></span>
* <span data-ttu-id="32ae3-499">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="32ae3-499">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="32ae3-500">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="32ae3-500">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="32ae3-501">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="32ae3-501">Az.OperationalInsights</span></span>
* <span data-ttu-id="32ae3-502">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="32ae3-502">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="32ae3-503">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-503">Az.RecoveryServices</span></span>
* <span data-ttu-id="32ae3-504">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="32ae3-504">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-505">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-505">Az.Resources</span></span>
    - <span data-ttu-id="32ae3-506">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="32ae3-506">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="32ae3-507">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="32ae3-507">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="32ae3-508">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="32ae3-508">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="32ae3-509">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="32ae3-509">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="32ae3-510">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="32ae3-510">Az.ServiceBus</span></span>
* <span data-ttu-id="32ae3-511">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="32ae3-511">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-512">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-512">Az.Sql</span></span>
* <span data-ttu-id="32ae3-513">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="32ae3-513">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="32ae3-514">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="32ae3-514">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="32ae3-515">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="32ae3-515">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="32ae3-516">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="32ae3-516">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="32ae3-517">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="32ae3-517">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="32ae3-518">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="32ae3-518">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="32ae3-519">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="32ae3-519">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="32ae3-520">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="32ae3-520">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="32ae3-521">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="32ae3-521">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="32ae3-522">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="32ae3-522">Az.Storage</span></span>
* <span data-ttu-id="32ae3-523">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="32ae3-523">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="32ae3-524">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="32ae3-524">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="32ae3-525">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="32ae3-525">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="32ae3-526">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="32ae3-526">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="32ae3-527">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="32ae3-527">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="32ae3-528">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="32ae3-528">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="32ae3-529">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="32ae3-529">Set-AzStorageAccount</span></span>
* <span data-ttu-id="32ae3-530">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="32ae3-530">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="32ae3-531">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="32ae3-531">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="32ae3-532">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="32ae3-532">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="32ae3-533">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="32ae3-533">Az.StorageSync</span></span>
* <span data-ttu-id="32ae3-534">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="32ae3-534">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="32ae3-535">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-535">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="32ae3-536">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-536">Az.Accounts</span></span>
* <span data-ttu-id="32ae3-537">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="32ae3-537">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="32ae3-538">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="32ae3-538">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="32ae3-539">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="32ae3-539">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="32ae3-540">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="32ae3-540">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="32ae3-541">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="32ae3-541">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-542">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-542">Az.Compute</span></span>
* <span data-ttu-id="32ae3-543">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="32ae3-543">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="32ae3-544">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="32ae3-544">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="32ae3-545">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="32ae3-545">Az.Dns</span></span>
* <span data-ttu-id="32ae3-546">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="32ae3-546">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="32ae3-547">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="32ae3-547">Az.EventGrid</span></span>
* <span data-ttu-id="32ae3-548">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="32ae3-548">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="32ae3-549">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="32ae3-549">New cmdlets:</span></span>
    - <span data-ttu-id="32ae3-550">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="32ae3-550">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="32ae3-551">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="32ae3-551">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="32ae3-552">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="32ae3-552">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="32ae3-553">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="32ae3-553">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="32ae3-554">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="32ae3-554">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="32ae3-555">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="32ae3-555">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="32ae3-556">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="32ae3-556">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="32ae3-557">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="32ae3-557">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="32ae3-558">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="32ae3-558">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="32ae3-559">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="32ae3-559">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="32ae3-560">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="32ae3-560">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="32ae3-561">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="32ae3-561">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="32ae3-562">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="32ae3-562">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="32ae3-563">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="32ae3-563">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="32ae3-564">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="32ae3-564">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="32ae3-565">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="32ae3-565">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="32ae3-566">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="32ae3-566">Updated cmdlets:</span></span>
    - <span data-ttu-id="32ae3-567">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="32ae3-567">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="32ae3-568">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="32ae3-568">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="32ae3-569">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="32ae3-569">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="32ae3-570">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="32ae3-570">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="32ae3-571">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="32ae3-571">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="32ae3-572">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="32ae3-572">Event subscription expiration date,</span></span>
            - <span data-ttu-id="32ae3-573">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="32ae3-573">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="32ae3-574">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="32ae3-574">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="32ae3-575">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="32ae3-575">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="32ae3-576">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="32ae3-576">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="32ae3-577">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="32ae3-577">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="32ae3-578">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="32ae3-578">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="32ae3-579">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="32ae3-579">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="32ae3-580">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="32ae3-580">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="32ae3-581">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="32ae3-581">Az.FrontDoor</span></span>
* <span data-ttu-id="32ae3-582">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="32ae3-582">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="32ae3-583">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="32ae3-583">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="32ae3-584">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="32ae3-584">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="32ae3-585">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="32ae3-585">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-586">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-586">Az.Network</span></span>
* <span data-ttu-id="32ae3-587">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="32ae3-587">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="32ae3-588">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="32ae3-588">New cmdlets</span></span>
        - <span data-ttu-id="32ae3-589">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="32ae3-589">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="32ae3-590">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="32ae3-590">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="32ae3-591">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="32ae3-591">New cmdlets</span></span>
        - <span data-ttu-id="32ae3-592">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="32ae3-592">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="32ae3-593">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="32ae3-593">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="32ae3-594">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="32ae3-594">New cmdlets</span></span>
        - <span data-ttu-id="32ae3-595">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="32ae3-595">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="32ae3-596">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="32ae3-596">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="32ae3-597">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="32ae3-597">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="32ae3-598">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-598">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="32ae3-599">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="32ae3-599">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="32ae3-600">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="32ae3-600">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="32ae3-601">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="32ae3-601">New cmdlets</span></span>
        - <span data-ttu-id="32ae3-602">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="32ae3-602">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="32ae3-603">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="32ae3-603">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="32ae3-604">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="32ae3-604">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="32ae3-605">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="32ae3-605">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="32ae3-606">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="32ae3-606">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="32ae3-607">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="32ae3-607">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="32ae3-608">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="32ae3-608">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="32ae3-609">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="32ae3-609">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="32ae3-610">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="32ae3-610">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="32ae3-611">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="32ae3-611">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="32ae3-612">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="32ae3-612">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="32ae3-613">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="32ae3-613">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="32ae3-614">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="32ae3-614">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="32ae3-615">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="32ae3-615">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="32ae3-616">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="32ae3-616">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="32ae3-617">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="32ae3-617">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="32ae3-618">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="32ae3-618">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="32ae3-619">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="32ae3-619">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="32ae3-620">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="32ae3-620">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="32ae3-621">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="32ae3-621">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="32ae3-622">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="32ae3-622">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="32ae3-623">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="32ae3-623">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="32ae3-624">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="32ae3-624">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="32ae3-625">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="32ae3-625">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="32ae3-626">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="32ae3-626">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="32ae3-627">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="32ae3-627">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="32ae3-628">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="32ae3-628">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="32ae3-629">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="32ae3-629">Az.OperationalInsights</span></span>
* <span data-ttu-id="32ae3-630">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="32ae3-630">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-631">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-631">Az.Resources</span></span>
* <span data-ttu-id="32ae3-632">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="32ae3-632">Support for additional Template Export options</span></span>
    - <span data-ttu-id="32ae3-633">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="32ae3-633">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="32ae3-634">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="32ae3-634">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="32ae3-635">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="32ae3-635">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="32ae3-636">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="32ae3-636">Az.ServiceFabric</span></span>
* <span data-ttu-id="32ae3-637">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="32ae3-637">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-638">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-638">Az.Sql</span></span>
* <span data-ttu-id="32ae3-639">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="32ae3-639">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="32ae3-640">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="32ae3-640">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="32ae3-641">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="32ae3-641">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="32ae3-642">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="32ae3-642">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="32ae3-643">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="32ae3-643">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="32ae3-644">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="32ae3-644">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="32ae3-645">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="32ae3-645">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="32ae3-646">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="32ae3-646">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="32ae3-647">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="32ae3-647">Az.Storage</span></span>
* <span data-ttu-id="32ae3-648">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="32ae3-648">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="32ae3-649">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="32ae3-649">New-AzStorageAccount</span></span>
* <span data-ttu-id="32ae3-650">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="32ae3-650">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="32ae3-651">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="32ae3-651">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="32ae3-652">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="32ae3-652">Az.Websites</span></span>
* <span data-ttu-id="32ae3-653">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="32ae3-653">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="32ae3-654">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="32ae3-654">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="32ae3-655">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-655">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="32ae3-656">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="32ae3-656">Az.Cdn</span></span>
* <span data-ttu-id="32ae3-657">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="32ae3-657">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-658">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-658">Az.Compute</span></span>
* <span data-ttu-id="32ae3-659">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="32ae3-659">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="32ae3-660">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="32ae3-660">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="32ae3-661">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="32ae3-661">Az.EventHub</span></span>
* <span data-ttu-id="32ae3-662">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="32ae3-662">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="32ae3-663">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="32ae3-663">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-664">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-664">Az.Network</span></span>
* <span data-ttu-id="32ae3-665">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="32ae3-665">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="32ae3-666">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="32ae3-666">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="32ae3-667">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="32ae3-667">Az.PolicyInsights</span></span>
* <span data-ttu-id="32ae3-668">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="32ae3-668">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="32ae3-669">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-669">Az.RecoveryServices</span></span>
* <span data-ttu-id="32ae3-670">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="32ae3-670">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="32ae3-671">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="32ae3-671">Az.ServiceBus</span></span>
* <span data-ttu-id="32ae3-672">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="32ae3-672">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="32ae3-673">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="32ae3-673">Az.ServiceFabric</span></span>
* <span data-ttu-id="32ae3-674">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="32ae3-674">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="32ae3-675">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="32ae3-675">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-676">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-676">Az.Sql</span></span>
* <span data-ttu-id="32ae3-677">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="32ae3-677">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="32ae3-678">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="32ae3-678">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="32ae3-679">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="32ae3-679">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="32ae3-680">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="32ae3-680">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="32ae3-681">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="32ae3-681">Az.Websites</span></span>
* <span data-ttu-id="32ae3-682">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="32ae3-682">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="32ae3-683">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-683">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="32ae3-684">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="32ae3-684">Az.ApiManagement</span></span>
* <span data-ttu-id="32ae3-685">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="32ae3-685">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="32ae3-686">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="32ae3-686">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="32ae3-687">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="32ae3-687">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="32ae3-688">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="32ae3-688">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="32ae3-689">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="32ae3-689">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="32ae3-690">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="32ae3-690">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="32ae3-691">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="32ae3-691">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="32ae3-692">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="32ae3-692">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="32ae3-693">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="32ae3-693">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="32ae3-694">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="32ae3-694">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="32ae3-695">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="32ae3-695">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="32ae3-696">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="32ae3-696">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="32ae3-697">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="32ae3-697">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="32ae3-698">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="32ae3-698">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="32ae3-699">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="32ae3-699">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="32ae3-700">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="32ae3-700">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="32ae3-701">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="32ae3-701">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="32ae3-702">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="32ae3-702">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="32ae3-703">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="32ae3-703">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="32ae3-704">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="32ae3-704">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="32ae3-705">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="32ae3-705">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="32ae3-706">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="32ae3-706">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="32ae3-707">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="32ae3-707">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="32ae3-708">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="32ae3-708">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="32ae3-709">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="32ae3-709">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="32ae3-710">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="32ae3-710">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="32ae3-711">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="32ae3-711">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="32ae3-712">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="32ae3-712">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="32ae3-713">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="32ae3-713">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="32ae3-714">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="32ae3-714">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="32ae3-715">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="32ae3-715">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="32ae3-716">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="32ae3-716">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="32ae3-717">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="32ae3-717">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="32ae3-718">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="32ae3-718">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="32ae3-719">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="32ae3-719">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="32ae3-720">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="32ae3-720">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="32ae3-721">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="32ae3-721">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="32ae3-722">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="32ae3-722">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="32ae3-723">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="32ae3-723">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="32ae3-724">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="32ae3-724">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="32ae3-725">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="32ae3-725">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="32ae3-726">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="32ae3-726">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="32ae3-727">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="32ae3-727">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="32ae3-728">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="32ae3-728">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="32ae3-729">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="32ae3-729">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="32ae3-730">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="32ae3-730">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="32ae3-731">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="32ae3-731">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="32ae3-732">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="32ae3-732">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="32ae3-733">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="32ae3-733">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="32ae3-734">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="32ae3-734">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="32ae3-735">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="32ae3-735">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="32ae3-736">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="32ae3-736">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="32ae3-737">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="32ae3-737">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="32ae3-738">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="32ae3-738">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="32ae3-739">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="32ae3-739">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="32ae3-740">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="32ae3-740">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="32ae3-741">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="32ae3-741">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="32ae3-742">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="32ae3-742">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="32ae3-743">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="32ae3-743">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="32ae3-744">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="32ae3-744">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="32ae3-745">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="32ae3-745">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="32ae3-746">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="32ae3-746">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="32ae3-747">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="32ae3-747">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="32ae3-748">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="32ae3-748">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="32ae3-749">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="32ae3-749">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="32ae3-750">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="32ae3-750">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="32ae3-751">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="32ae3-751">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="32ae3-752">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="32ae3-752">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="32ae3-753">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="32ae3-753">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="32ae3-754">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="32ae3-754">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="32ae3-755">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="32ae3-755">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="32ae3-756">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="32ae3-756">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="32ae3-757">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="32ae3-757">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="32ae3-758">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="32ae3-758">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="32ae3-759">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="32ae3-759">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="32ae3-760">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="32ae3-760">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="32ae3-761">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="32ae3-761">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="32ae3-762">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="32ae3-762">Az.Automation</span></span>
* <span data-ttu-id="32ae3-763">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="32ae3-763">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="32ae3-764">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="32ae3-764">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="32ae3-765">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="32ae3-765">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="32ae3-766">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="32ae3-766">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="32ae3-767">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="32ae3-767">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="32ae3-768">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="32ae3-768">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="32ae3-769">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="32ae3-769">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-770">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-770">Az.Compute</span></span>
* <span data-ttu-id="32ae3-771">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="32ae3-771">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="32ae3-772">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="32ae3-772">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="32ae3-773">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="32ae3-773">Az.DataLakeStore</span></span>
* <span data-ttu-id="32ae3-774">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="32ae3-774">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="32ae3-775">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="32ae3-775">Az.Monitor</span></span>
* <span data-ttu-id="32ae3-776">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="32ae3-776">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-777">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-777">Az.Network</span></span>
* <span data-ttu-id="32ae3-778">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="32ae3-778">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="32ae3-779">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="32ae3-779">Updated cmdlet:</span></span>
        - <span data-ttu-id="32ae3-780">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="32ae3-780">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="32ae3-781">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="32ae3-781">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-782">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-782">Az.Resources</span></span>
* <span data-ttu-id="32ae3-783">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="32ae3-783">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-784">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-784">Az.Sql</span></span>
* <span data-ttu-id="32ae3-785">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="32ae3-785">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="32ae3-786">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-786">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="32ae3-787">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-787">Az.Accounts</span></span>
* <span data-ttu-id="32ae3-788">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="32ae3-788">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="32ae3-789">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-789">Az.CognitiveServices</span></span>
* <span data-ttu-id="32ae3-790">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="32ae3-790">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="32ae3-791">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="32ae3-791">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-792">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-792">Az.Compute</span></span>
* <span data-ttu-id="32ae3-793">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="32ae3-793">Proximity placement group feature.</span></span>
    - <span data-ttu-id="32ae3-794">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="32ae3-794">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="32ae3-795">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-795">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="32ae3-796">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="32ae3-796">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="32ae3-797">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="32ae3-797">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="32ae3-798">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="32ae3-798">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="32ae3-799">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="32ae3-799">Breaking changes</span></span>
    - <span data-ttu-id="32ae3-800">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="32ae3-800">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="32ae3-801">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="32ae3-801">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="32ae3-802">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="32ae3-802">Az.DeploymentManager</span></span>
* <span data-ttu-id="32ae3-803">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="32ae3-803">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="32ae3-804">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="32ae3-804">Az.Dns</span></span>
* <span data-ttu-id="32ae3-805">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="32ae3-805">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="32ae3-806">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="32ae3-806">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="32ae3-807">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="32ae3-807">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="32ae3-808">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="32ae3-808">Az.FrontDoor</span></span>
* <span data-ttu-id="32ae3-809">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="32ae3-809">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="32ae3-810">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="32ae3-810">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="32ae3-811">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="32ae3-811">Az.HDInsight</span></span>
* <span data-ttu-id="32ae3-812">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="32ae3-812">Removed two cmdlets:</span></span>
    - <span data-ttu-id="32ae3-813">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="32ae3-813">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="32ae3-814">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="32ae3-814">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="32ae3-815">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="32ae3-815">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="32ae3-816">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="32ae3-816">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="32ae3-817">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="32ae3-817">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="32ae3-818">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="32ae3-818">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="32ae3-819">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="32ae3-819">Az.Monitor</span></span>
* <span data-ttu-id="32ae3-820">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="32ae3-820">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="32ae3-821">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="32ae3-821">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="32ae3-822">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="32ae3-822">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="32ae3-823">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="32ae3-823">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="32ae3-824">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="32ae3-824">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="32ae3-825">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="32ae3-825">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="32ae3-826">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="32ae3-826">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="32ae3-827">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="32ae3-827">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="32ae3-828">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="32ae3-828">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="32ae3-829">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="32ae3-829">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="32ae3-830">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="32ae3-830">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="32ae3-831">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="32ae3-831">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="32ae3-832">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="32ae3-832">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="32ae3-833">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="32ae3-833">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-834">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-834">Az.Network</span></span>
* <span data-ttu-id="32ae3-835">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="32ae3-835">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="32ae3-836">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="32ae3-836">New cmdlets</span></span>
        - <span data-ttu-id="32ae3-837">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="32ae3-837">New-AzNatGateway</span></span>
        - <span data-ttu-id="32ae3-838">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="32ae3-838">Get-AzNatGateway</span></span>
        - <span data-ttu-id="32ae3-839">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="32ae3-839">Set-AzNatGateway</span></span>
        - <span data-ttu-id="32ae3-840">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="32ae3-840">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="32ae3-841">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="32ae3-841">Updated cmdlets</span></span>
        - <span data-ttu-id="32ae3-842">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="32ae3-842">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="32ae3-843">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="32ae3-843">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="32ae3-844">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="32ae3-844">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="32ae3-845">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="32ae3-845">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="32ae3-846">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="32ae3-846">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="32ae3-847">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="32ae3-847">Az.PolicyInsights</span></span>
* <span data-ttu-id="32ae3-848">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="32ae3-848">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="32ae3-849">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="32ae3-849">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="32ae3-850">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="32ae3-850">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="32ae3-851">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-851">Az.RecoveryServices</span></span>
* <span data-ttu-id="32ae3-852">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="32ae3-852">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="32ae3-853">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="32ae3-853">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="32ae3-854">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="32ae3-854">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="32ae3-855">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="32ae3-855">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="32ae3-856">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="32ae3-856">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="32ae3-857">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="32ae3-857">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="32ae3-858">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="32ae3-858">Az.Relay</span></span>
* <span data-ttu-id="32ae3-859">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="32ae3-859">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="32ae3-860">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="32ae3-860">Az.ServiceBus</span></span>
* <span data-ttu-id="32ae3-861">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="32ae3-861">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="32ae3-862">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="32ae3-862">Az.Storage</span></span>
* <span data-ttu-id="32ae3-863">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="32ae3-863">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="32ae3-864">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="32ae3-864">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="32ae3-865">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="32ae3-865">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="32ae3-866">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="32ae3-866">New-AzStorageAccount</span></span>
* <span data-ttu-id="32ae3-867">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="32ae3-867">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="32ae3-868">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="32ae3-868">New-AzStorageAccount</span></span>
    - <span data-ttu-id="32ae3-869">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="32ae3-869">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="32ae3-870">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="32ae3-870">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="32ae3-871">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="32ae3-871">Az.Websites</span></span>
* <span data-ttu-id="32ae3-872">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="32ae3-872">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="32ae3-873">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="32ae3-873">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="32ae3-874">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-874">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="32ae3-875">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="32ae3-875">Highlights since the last major release</span></span>
* <span data-ttu-id="32ae3-876">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="32ae3-876">General availability of `Az` module</span></span>
* <span data-ttu-id="32ae3-877">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="32ae3-877">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="32ae3-878">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="32ae3-878">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="32ae3-879">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-879">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="32ae3-880">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="32ae3-880">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="32ae3-881">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="32ae3-881">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="32ae3-882">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="32ae3-882">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="32ae3-883">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-883">Az.Accounts</span></span>
* <span data-ttu-id="32ae3-884">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="32ae3-884">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="32ae3-885">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="32ae3-885">Az.Batch</span></span>
* <span data-ttu-id="32ae3-886">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-886">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="32ae3-887">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="32ae3-887">Az.Cdn</span></span>
* <span data-ttu-id="32ae3-888">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-888">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="32ae3-889">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-889">Az.CognitiveServices</span></span>
* <span data-ttu-id="32ae3-890">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-890">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-891">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-891">Az.Compute</span></span>
* <span data-ttu-id="32ae3-892">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="32ae3-892">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="32ae3-893">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-893">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="32ae3-894">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="32ae3-894">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="32ae3-895">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="32ae3-895">Az.DataFactory</span></span>
* <span data-ttu-id="32ae3-896">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="32ae3-896">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="32ae3-897">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="32ae3-897">Az.DataLakeStore</span></span>
* <span data-ttu-id="32ae3-898">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-898">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="32ae3-899">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="32ae3-899">Az.EventGrid</span></span>
* <span data-ttu-id="32ae3-900">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="32ae3-900">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="32ae3-901">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="32ae3-901">Az.EventHub</span></span>
* <span data-ttu-id="32ae3-902">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="32ae3-902">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="32ae3-903">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="32ae3-903">Az.HDInsight</span></span>
* <span data-ttu-id="32ae3-904">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-904">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="32ae3-905">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="32ae3-905">Az.IotHub</span></span>
* <span data-ttu-id="32ae3-906">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-906">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="32ae3-907">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="32ae3-907">Az.KeyVault</span></span>
* <span data-ttu-id="32ae3-908">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-908">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="32ae3-909">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="32ae3-909">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="32ae3-910">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="32ae3-910">Az.MachineLearning</span></span>
* <span data-ttu-id="32ae3-911">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-911">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="32ae3-912">Az.Media</span><span class="sxs-lookup"><span data-stu-id="32ae3-912">Az.Media</span></span>
* <span data-ttu-id="32ae3-913">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-913">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="32ae3-914">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="32ae3-914">Az.Monitor</span></span>
  * <span data-ttu-id="32ae3-915">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="32ae3-915">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="32ae3-916">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="32ae3-916">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="32ae3-917">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="32ae3-917">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="32ae3-918">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="32ae3-918">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="32ae3-919">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="32ae3-919">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="32ae3-920">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="32ae3-920">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="32ae3-921">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="32ae3-921">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-922">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-922">Az.Network</span></span>
* <span data-ttu-id="32ae3-923">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-923">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="32ae3-924">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="32ae3-924">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="32ae3-925">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="32ae3-925">Az.NotificationHubs</span></span>
* <span data-ttu-id="32ae3-926">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-926">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="32ae3-927">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="32ae3-927">Az.OperationalInsights</span></span>
* <span data-ttu-id="32ae3-928">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-928">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="32ae3-929">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="32ae3-929">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="32ae3-930">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-930">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="32ae3-931">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-931">Az.RecoveryServices</span></span>
* <span data-ttu-id="32ae3-932">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-932">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="32ae3-933">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="32ae3-933">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="32ae3-934">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="32ae3-934">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="32ae3-935">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="32ae3-935">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="32ae3-936">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="32ae3-936">Az.RedisCache</span></span>
* <span data-ttu-id="32ae3-937">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-937">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-938">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-938">Az.Resources</span></span>
* <span data-ttu-id="32ae3-939">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="32ae3-939">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-940">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-940">Az.Sql</span></span>
* <span data-ttu-id="32ae3-941">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="32ae3-941">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="32ae3-942">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-942">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="32ae3-943">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="32ae3-943">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="32ae3-944">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="32ae3-944">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="32ae3-945">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="32ae3-945">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="32ae3-946">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="32ae3-946">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="32ae3-947">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="32ae3-947">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="32ae3-948">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="32ae3-948">Az.Websites</span></span>
* <span data-ttu-id="32ae3-949">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="32ae3-949">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="32ae3-950">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="32ae3-950">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="32ae3-951">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="32ae3-951">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="32ae3-952">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="32ae3-952">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="32ae3-953">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-953">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="32ae3-954">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="32ae3-954">Highlights since the last major release</span></span>
* <span data-ttu-id="32ae3-955">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="32ae3-955">General availability of `Az` module</span></span>
* <span data-ttu-id="32ae3-956">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="32ae3-956">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="32ae3-957">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="32ae3-957">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="32ae3-958">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-958">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="32ae3-959">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="32ae3-959">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="32ae3-960">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="32ae3-960">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="32ae3-961">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="32ae3-961">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="32ae3-962">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-962">Az.Accounts</span></span>
* <span data-ttu-id="32ae3-963">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="32ae3-963">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="32ae3-964">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-964">Az.AnalysisServices</span></span>
* <span data-ttu-id="32ae3-965">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="32ae3-965">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="32ae3-966">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="32ae3-966">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="32ae3-967">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="32ae3-967">Az.Automation</span></span>
* <span data-ttu-id="32ae3-968">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="32ae3-968">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="32ae3-969">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="32ae3-969">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="32ae3-970">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="32ae3-970">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-971">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-971">Az.Compute</span></span>
* <span data-ttu-id="32ae3-972">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-972">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="32ae3-973">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="32ae3-973">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="32ae3-974">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="32ae3-974">Az.ContainerInstance</span></span>
* <span data-ttu-id="32ae3-975">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="32ae3-975">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="32ae3-976">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="32ae3-976">Az.DataFactory</span></span>
* <span data-ttu-id="32ae3-977">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="32ae3-977">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="32ae3-978">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="32ae3-978">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-979">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-979">Az.Resources</span></span>
* <span data-ttu-id="32ae3-980">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="32ae3-980">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="32ae3-981">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="32ae3-981">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="32ae3-982">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="32ae3-982">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="32ae3-983">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="32ae3-983">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="32ae3-984">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="32ae3-984">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="32ae3-985">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="32ae3-985">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-986">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-986">Az.Sql</span></span>
* <span data-ttu-id="32ae3-987">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="32ae3-987">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="32ae3-988">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="32ae3-988">Az.Storage</span></span>
* <span data-ttu-id="32ae3-989">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="32ae3-989">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="32ae3-990">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="32ae3-990">New-AzStorageContext</span></span>
* <span data-ttu-id="32ae3-991">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="32ae3-991">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="32ae3-992">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="32ae3-992">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="32ae3-993">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="32ae3-993">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="32ae3-994">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="32ae3-994">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="32ae3-995">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="32ae3-995">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="32ae3-996">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="32ae3-996">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="32ae3-997">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="32ae3-997">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="32ae3-998">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="32ae3-998">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="32ae3-999">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="32ae3-999">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="32ae3-1000">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="32ae3-1000">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="32ae3-1001">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-1001">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="32ae3-1002">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="32ae3-1002">Highlights since the last major release</span></span>
* <span data-ttu-id="32ae3-1003">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="32ae3-1003">General availability of `Az` module</span></span>
* <span data-ttu-id="32ae3-1004">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="32ae3-1004">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="32ae3-1005">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="32ae3-1005">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="32ae3-1006">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-1006">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="32ae3-1007">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="32ae3-1007">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="32ae3-1008">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="32ae3-1008">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="32ae3-1009">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="32ae3-1009">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="32ae3-1010">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="32ae3-1010">Az.Automation</span></span>
* <span data-ttu-id="32ae3-1011">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="32ae3-1011">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="32ae3-1012">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="32ae3-1012">Dynamic grouping</span></span>
    * <span data-ttu-id="32ae3-1013">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="32ae3-1013">Pre-Post script</span></span>
    * <span data-ttu-id="32ae3-1014">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="32ae3-1014">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-1015">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-1015">Az.Compute</span></span>
* <span data-ttu-id="32ae3-1016">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="32ae3-1016">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="32ae3-1017">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1017">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="32ae3-1018">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="32ae3-1018">Az.KeyVault</span></span>
* <span data-ttu-id="32ae3-1019">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="32ae3-1019">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-1020">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-1020">Az.Network</span></span>
* <span data-ttu-id="32ae3-1021">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="32ae3-1021">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="32ae3-1022">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="32ae3-1022">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="32ae3-1023">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-1023">Az.RecoveryServices</span></span>
* <span data-ttu-id="32ae3-1024">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="32ae3-1024">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="32ae3-1025">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="32ae3-1025">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-1026">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-1026">Az.Resources</span></span>
* <span data-ttu-id="32ae3-1027">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="32ae3-1027">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="32ae3-1028">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="32ae3-1028">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-1029">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-1029">Az.Sql</span></span>
* <span data-ttu-id="32ae3-1030">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1030">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="32ae3-1031">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="32ae3-1031">Az.Storage</span></span>
* <span data-ttu-id="32ae3-1032">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="32ae3-1032">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="32ae3-1033">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="32ae3-1033">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="32ae3-1034">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="32ae3-1034">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="32ae3-1035">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="32ae3-1035">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="32ae3-1036">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="32ae3-1036">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="32ae3-1037">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="32ae3-1037">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="32ae3-1038">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="32ae3-1038">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="32ae3-1039">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="32ae3-1039">Az.Websites</span></span>
* <span data-ttu-id="32ae3-1040">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="32ae3-1040">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="32ae3-1041">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-1041">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="32ae3-1042">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-1042">Az.Accounts</span></span>
* <span data-ttu-id="32ae3-1043">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="32ae3-1043">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="32ae3-1044">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="32ae3-1044">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="32ae3-1045">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="32ae3-1045">Az.Automation</span></span>
* <span data-ttu-id="32ae3-1046">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="32ae3-1046">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="32ae3-1047">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1047">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="32ae3-1048">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="32ae3-1048">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="32ae3-1049">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="32ae3-1049">Az.Cdn</span></span>
* <span data-ttu-id="32ae3-1050">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1050">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-1051">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-1051">Az.Compute</span></span>
* <span data-ttu-id="32ae3-1052">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="32ae3-1052">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="32ae3-1053">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="32ae3-1053">Az.DataFactory</span></span>
* <span data-ttu-id="32ae3-1054">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="32ae3-1054">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="32ae3-1055">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="32ae3-1055">Az.LogicApp</span></span>
* <span data-ttu-id="32ae3-1056">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="32ae3-1056">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-1057">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-1057">Az.Network</span></span>
* <span data-ttu-id="32ae3-1058">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-1058">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="32ae3-1059">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-1059">Az.RecoveryServices</span></span>
* <span data-ttu-id="32ae3-1060">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="32ae3-1060">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="32ae3-1061">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="32ae3-1061">SDK Update</span></span>
* <span data-ttu-id="32ae3-1062">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="32ae3-1062">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="32ae3-1063">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="32ae3-1063">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-1064">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-1064">Az.Resources</span></span>
* <span data-ttu-id="32ae3-1065">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="32ae3-1065">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="32ae3-1066">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="32ae3-1066">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="32ae3-1067">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="32ae3-1067">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="32ae3-1068">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="32ae3-1068">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="32ae3-1069">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="32ae3-1069">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="32ae3-1070">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="32ae3-1070">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-1071">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-1071">Az.Sql</span></span>
* <span data-ttu-id="32ae3-1072">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1072">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="32ae3-1073">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1073">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="32ae3-1074">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="32ae3-1074">Az.Storage</span></span>
* <span data-ttu-id="32ae3-1075">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="32ae3-1075">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="32ae3-1076">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-1076">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="32ae3-1077">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-1077">Az.AnalysisServices</span></span>
* <span data-ttu-id="32ae3-1078">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="32ae3-1078">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="32ae3-1079">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="32ae3-1079">Az.Automation</span></span>
* <span data-ttu-id="32ae3-1080">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="32ae3-1080">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="32ae3-1081">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="32ae3-1081">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="32ae3-1082">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="32ae3-1082">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="32ae3-1083">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-1083">Az.CognitiveServices</span></span>
* <span data-ttu-id="32ae3-1084">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1084">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-1085">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-1085">Az.Compute</span></span>
* <span data-ttu-id="32ae3-1086">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="32ae3-1086">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="32ae3-1087">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="32ae3-1087">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="32ae3-1088">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="32ae3-1088">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="32ae3-1089">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1089">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="32ae3-1090">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="32ae3-1090">Az.DataLakeStore</span></span>
* <span data-ttu-id="32ae3-1091">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="32ae3-1091">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="32ae3-1092">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="32ae3-1092">Az.EventHub</span></span>
* <span data-ttu-id="32ae3-1093">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="32ae3-1093">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="32ae3-1094">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="32ae3-1094">Az.KeyVault</span></span>
* <span data-ttu-id="32ae3-1095">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="32ae3-1095">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="32ae3-1096">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="32ae3-1096">Az.LogicApp</span></span>
* <span data-ttu-id="32ae3-1097">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="32ae3-1097">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="32ae3-1098">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1098">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="32ae3-1099">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="32ae3-1099">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="32ae3-1100">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="32ae3-1100">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="32ae3-1101">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="32ae3-1101">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="32ae3-1102">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="32ae3-1102">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="32ae3-1103">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="32ae3-1103">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="32ae3-1104">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="32ae3-1104">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="32ae3-1105">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="32ae3-1105">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="32ae3-1106">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="32ae3-1106">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="32ae3-1107">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="32ae3-1107">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="32ae3-1108">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="32ae3-1108">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="32ae3-1109">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="32ae3-1109">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="32ae3-1110">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="32ae3-1110">Az.Monitor</span></span>
* <span data-ttu-id="32ae3-1111">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="32ae3-1111">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-1112">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-1112">Az.Network</span></span>
* <span data-ttu-id="32ae3-1113">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="32ae3-1113">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="32ae3-1114">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="32ae3-1114">Az.OperationalInsights</span></span>
* <span data-ttu-id="32ae3-1115">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1115">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="32ae3-1116">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1116">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="32ae3-1117">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1117">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-1118">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-1118">Az.Resources</span></span>
* <span data-ttu-id="32ae3-1119">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="32ae3-1119">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="32ae3-1120">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="32ae3-1120">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="32ae3-1121">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="32ae3-1121">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="32ae3-1122">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="32ae3-1122">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-1123">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-1123">Az.Sql</span></span>
* <span data-ttu-id="32ae3-1124">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="32ae3-1124">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="32ae3-1125">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="32ae3-1125">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="32ae3-1126">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="32ae3-1126">Az.Websites</span></span>
* <span data-ttu-id="32ae3-1127">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="32ae3-1127">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="32ae3-1128">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-1128">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="32ae3-1129">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-1129">Az.Accounts</span></span>
* <span data-ttu-id="32ae3-1130">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="32ae3-1130">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="32ae3-1131">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-1131">Az.AnalysisServices</span></span>
<span data-ttu-id="32ae3-1132">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1132">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-1133">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-1133">Az.Compute</span></span>
* <span data-ttu-id="32ae3-1134">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="32ae3-1134">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="32ae3-1135">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="32ae3-1135">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="32ae3-1136">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="32ae3-1136">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="32ae3-1137">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-1137">Az.RecoveryServices</span></span>
<span data-ttu-id="32ae3-1138">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1138">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-1139">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-1139">Az.Resources</span></span>
* <span data-ttu-id="32ae3-1140">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="32ae3-1140">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="32ae3-1141">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="32ae3-1141">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="32ae3-1142">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="32ae3-1142">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="32ae3-1143">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="32ae3-1143">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-1144">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-1144">Az.Sql</span></span>
* <span data-ttu-id="32ae3-1145">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="32ae3-1145">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="32ae3-1146">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="32ae3-1146">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="32ae3-1147">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="32ae3-1147">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="32ae3-1148">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-1148">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="32ae3-1149">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-1149">Az.Accounts</span></span>
* <span data-ttu-id="32ae3-1150">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="32ae3-1150">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="32ae3-1151">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-1151">Az.AnalysisServices</span></span>
* <span data-ttu-id="32ae3-1152">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="32ae3-1152">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="32ae3-1153">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-1153">Az.RecoveryServices</span></span>
* <span data-ttu-id="32ae3-1154">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="32ae3-1154">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="32ae3-1155">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-1155">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="32ae3-1156">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-1156">Az.Accounts</span></span>
* <span data-ttu-id="32ae3-1157">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="32ae3-1157">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="32ae3-1158">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1158">Update incorrect online help URLs</span></span>
* <span data-ttu-id="32ae3-1159">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="32ae3-1159">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="32ae3-1160">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="32ae3-1160">Az.Aks</span></span>
* <span data-ttu-id="32ae3-1161">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1161">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="32ae3-1162">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="32ae3-1162">Az.Automation</span></span>
* <span data-ttu-id="32ae3-1163">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="32ae3-1163">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="32ae3-1164">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1164">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="32ae3-1165">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="32ae3-1165">Az.Cdn</span></span>
* <span data-ttu-id="32ae3-1166">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1166">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-1167">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-1167">Az.Compute</span></span>
* <span data-ttu-id="32ae3-1168">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="32ae3-1168">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="32ae3-1169">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="32ae3-1169">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="32ae3-1170">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="32ae3-1170">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="32ae3-1171">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="32ae3-1171">Az.ContainerRegistry</span></span>
* <span data-ttu-id="32ae3-1172">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1172">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="32ae3-1173">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="32ae3-1173">Az.DataFactory</span></span>
* <span data-ttu-id="32ae3-1174">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="32ae3-1174">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="32ae3-1175">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="32ae3-1175">Az.DataLakeStore</span></span>
* <span data-ttu-id="32ae3-1176">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="32ae3-1176">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="32ae3-1177">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="32ae3-1177">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="32ae3-1178">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1178">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="32ae3-1179">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="32ae3-1179">Az.IotHub</span></span>
* <span data-ttu-id="32ae3-1180">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1180">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="32ae3-1181">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="32ae3-1181">Az.KeyVault</span></span>
* <span data-ttu-id="32ae3-1182">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1182">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-1183">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-1183">Az.Network</span></span>
* <span data-ttu-id="32ae3-1184">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1184">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-1185">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-1185">Az.Resources</span></span>
* <span data-ttu-id="32ae3-1186">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="32ae3-1186">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="32ae3-1187">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1187">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="32ae3-1188">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="32ae3-1188">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="32ae3-1189">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="32ae3-1189">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="32ae3-1190">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="32ae3-1190">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="32ae3-1191">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="32ae3-1191">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="32ae3-1192">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="32ae3-1192">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="32ae3-1193">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="32ae3-1193">Az.ServiceFabric</span></span>
* <span data-ttu-id="32ae3-1194">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="32ae3-1194">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="32ae3-1195">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1195">Fix some error messages.</span></span>
* <span data-ttu-id="32ae3-1196">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1196">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="32ae3-1197">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1197">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="32ae3-1198">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="32ae3-1198">Az.SignalR</span></span>
* <span data-ttu-id="32ae3-1199">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1199">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-1200">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-1200">Az.Sql</span></span>
* <span data-ttu-id="32ae3-1201">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1201">Update incorrect online help URLs</span></span>
* <span data-ttu-id="32ae3-1202">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="32ae3-1202">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="32ae3-1203">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="32ae3-1203">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="32ae3-1204">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="32ae3-1204">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="32ae3-1205">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="32ae3-1205">Az.Storage</span></span>
* <span data-ttu-id="32ae3-1206">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1206">Update incorrect online help URLs</span></span>
* <span data-ttu-id="32ae3-1207">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1207">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="32ae3-1208">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="32ae3-1208">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="32ae3-1209">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="32ae3-1209">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="32ae3-1210">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="32ae3-1210">Az.TrafficManager</span></span>
* <span data-ttu-id="32ae3-1211">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1211">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="32ae3-1212">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="32ae3-1212">Az.Websites</span></span>
* <span data-ttu-id="32ae3-1213">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1213">Update incorrect online help URLs</span></span>
* <span data-ttu-id="32ae3-1214">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1214">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="32ae3-1215">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="32ae3-1215">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="32ae3-1216">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="32ae3-1216">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="32ae3-1217">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-1217">Az.Accounts</span></span>
* <span data-ttu-id="32ae3-1218">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="32ae3-1218">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-1219">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-1219">Az.Compute</span></span>
* <span data-ttu-id="32ae3-1220">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="32ae3-1220">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="32ae3-1221">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="32ae3-1221">Updated the description of ID in help files</span></span>
* <span data-ttu-id="32ae3-1222">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-1222">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="32ae3-1223">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="32ae3-1223">Az.DataLakeStore</span></span>
* <span data-ttu-id="32ae3-1224">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1224">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="32ae3-1225">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="32ae3-1225">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="32ae3-1226">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="32ae3-1226">Az.EventGrid</span></span>
* <span data-ttu-id="32ae3-1227">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1227">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="32ae3-1228">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="32ae3-1228">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="32ae3-1229">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="32ae3-1229">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="32ae3-1230">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="32ae3-1230">Event Time-To-Live,</span></span>
        - <span data-ttu-id="32ae3-1231">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="32ae3-1231">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="32ae3-1232">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1232">Dead letter endpoint.</span></span>
    - <span data-ttu-id="32ae3-1233">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="32ae3-1233">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="32ae3-1234">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="32ae3-1234">Event Time-To-Live,</span></span>
        - <span data-ttu-id="32ae3-1235">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="32ae3-1235">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="32ae3-1236">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1236">Dead letter endpoint.</span></span>
* <span data-ttu-id="32ae3-1237">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1237">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="32ae3-1238">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1238">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="32ae3-1239">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="32ae3-1239">Az.IotHub</span></span>
* <span data-ttu-id="32ae3-1240">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="32ae3-1240">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="32ae3-1241">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="32ae3-1241">Az.LogicApp</span></span>
* <span data-ttu-id="32ae3-1242">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="32ae3-1242">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-1243">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-1243">Az.Resources</span></span>
* <span data-ttu-id="32ae3-1244">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="32ae3-1244">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="32ae3-1245">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="32ae3-1245">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="32ae3-1246">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="32ae3-1246">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="32ae3-1247">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="32ae3-1247">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="32ae3-1248">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="32ae3-1248">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="32ae3-1249">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="32ae3-1249">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="32ae3-1250">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="32ae3-1250">Az.SignalR</span></span>
* <span data-ttu-id="32ae3-1251">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-1251">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-1252">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-1252">Az.Sql</span></span>
* <span data-ttu-id="32ae3-1253">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1253">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="32ae3-1254">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="32ae3-1254">Az.Storage</span></span>
* <span data-ttu-id="32ae3-1255">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="32ae3-1255">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="32ae3-1256">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="32ae3-1256">New-AzStorageContext</span></span>
* <span data-ttu-id="32ae3-1257">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="32ae3-1257">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="32ae3-1258">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="32ae3-1258">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="32ae3-1259">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="32ae3-1259">Az.Websites</span></span>
* <span data-ttu-id="32ae3-1260">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="32ae3-1260">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="32ae3-1261">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-1261">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="32ae3-1262">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="32ae3-1262">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="32ae3-1263">Geral</span><span class="sxs-lookup"><span data-stu-id="32ae3-1263">General</span></span>

- <span data-ttu-id="32ae3-1264">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="32ae3-1264">General Availability of Az Module</span></span>
- <span data-ttu-id="32ae3-1265">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="32ae3-1265">Online help for each module</span></span>
- <span data-ttu-id="32ae3-1266">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="32ae3-1266">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="32ae3-1267">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="32ae3-1267">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="32ae3-1268">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-1268">Az.Accounts</span></span>
- <span data-ttu-id="32ae3-1269">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="32ae3-1269">Changed from Az.Profile</span></span>
- <span data-ttu-id="32ae3-1270">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="32ae3-1270">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="32ae3-1271">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="32ae3-1271">Az.ApiManagement</span></span>
- <span data-ttu-id="32ae3-1272">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="32ae3-1272">Fixes for #7002</span></span>
- <span data-ttu-id="32ae3-1273">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="32ae3-1273">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="32ae3-1274">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="32ae3-1274">Az.Batch</span></span>
- <span data-ttu-id="32ae3-1275">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1275">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="32ae3-1276">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1276">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="32ae3-1277">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="32ae3-1277">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="32ae3-1278">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="32ae3-1278">Az.Billing</span></span>
- <span data-ttu-id="32ae3-1279">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="32ae3-1279">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="32ae3-1280">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-1280">Az.CognitivServices</span></span>
- <span data-ttu-id="32ae3-1281">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="32ae3-1281">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="32ae3-1282">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="32ae3-1282">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="32ae3-1283">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="32ae3-1283">Az.ContainerInstance</span></span>
- <span data-ttu-id="32ae3-1284">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="32ae3-1284">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="32ae3-1285">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="32ae3-1285">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="32ae3-1286">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="32ae3-1286">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="32ae3-1287">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="32ae3-1287">Az.DataLakeStore</span></span>
- <span data-ttu-id="32ae3-1288">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="32ae3-1288">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="32ae3-1289">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="32ae3-1289">Az.Monitor</span></span>
- <span data-ttu-id="32ae3-1290">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="32ae3-1290">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="32ae3-1291">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="32ae3-1291">Az.KeyVault</span></span>
- <span data-ttu-id="32ae3-1292">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="32ae3-1292">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="32ae3-1293">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="32ae3-1293">Az.MachineLearning</span></span>
- <span data-ttu-id="32ae3-1294">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="32ae3-1294">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="32ae3-1295">Az.Media</span><span class="sxs-lookup"><span data-stu-id="32ae3-1295">Az.Media</span></span>
- <span data-ttu-id="32ae3-1296">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="32ae3-1296">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="32ae3-1297">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-1297">Az.Network</span></span>
<span data-ttu-id="32ae3-1298">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="32ae3-1298">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="32ae3-1299">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="32ae3-1299">New cmdlets added:</span></span>
        - <span data-ttu-id="32ae3-1300">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="32ae3-1300">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="32ae3-1301">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="32ae3-1301">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="32ae3-1302">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="32ae3-1302">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="32ae3-1303">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="32ae3-1303">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="32ae3-1304">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="32ae3-1304">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="32ae3-1305">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="32ae3-1305">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="32ae3-1306">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="32ae3-1306">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="32ae3-1307">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="32ae3-1307">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="32ae3-1308">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="32ae3-1308">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="32ae3-1309">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="32ae3-1309">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="32ae3-1310">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="32ae3-1310">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="32ae3-1311">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="32ae3-1311">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="32ae3-1312">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-1312">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="32ae3-1313">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-1313">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="32ae3-1314">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1314">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="32ae3-1315">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="32ae3-1315">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="32ae3-1316">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="32ae3-1316">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="32ae3-1317">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="32ae3-1317">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="32ae3-1318">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="32ae3-1318">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="32ae3-1319">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="32ae3-1319">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="32ae3-1320">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="32ae3-1320">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="32ae3-1321">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="32ae3-1321">Az.OperationalInsights</span></span>
- <span data-ttu-id="32ae3-1322">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="32ae3-1322">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="32ae3-1323">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="32ae3-1323">Az.Profile</span></span>
- <span data-ttu-id="32ae3-1324">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="32ae3-1324">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="32ae3-1325">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-1325">Az.RecoveryServices</span></span>
- <span data-ttu-id="32ae3-1326">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="32ae3-1326">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="32ae3-1327">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-1327">Az.Resources</span></span>
- <span data-ttu-id="32ae3-1328">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="32ae3-1328">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="32ae3-1329">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="32ae3-1329">Az.ServiceFabric</span></span>
- <span data-ttu-id="32ae3-1330">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="32ae3-1330">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="32ae3-1331">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="32ae3-1331">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="32ae3-1332">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="32ae3-1332">Az.SIgnalR</span></span>
- <span data-ttu-id="32ae3-1333">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="32ae3-1333">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="32ae3-1334">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-1334">Az.Sql</span></span>
- <span data-ttu-id="32ae3-1335">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="32ae3-1335">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="32ae3-1336">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="32ae3-1336">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="32ae3-1337">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="32ae3-1337">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="32ae3-1338">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="32ae3-1338">Az.Storage</span></span>
- <span data-ttu-id="32ae3-1339">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="32ae3-1339">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="32ae3-1340">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="32ae3-1340">Az.Websites</span></span>
- <span data-ttu-id="32ae3-1341">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="32ae3-1341">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="32ae3-1342">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="32ae3-1342">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="32ae3-1343">Geral</span><span class="sxs-lookup"><span data-stu-id="32ae3-1343">General</span></span>

* <span data-ttu-id="32ae3-1344">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="32ae3-1344">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="32ae3-1345">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-1345">Az.Compute</span></span>

* <span data-ttu-id="32ae3-1346">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1346">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="32ae3-1347">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="32ae3-1347">Az.DataLakeStore</span></span>

* <span data-ttu-id="32ae3-1348">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="32ae3-1348">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="32ae3-1349">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="32ae3-1349">Az.FrontDoor</span></span>

* <span data-ttu-id="32ae3-1350">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="32ae3-1350">Fixed some broken links</span></span>
    - <span data-ttu-id="32ae3-1351">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1351">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="32ae3-1352">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1352">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="32ae3-1353">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-1353">Az.RecoveryServices</span></span>

* <span data-ttu-id="32ae3-1354">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1354">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="32ae3-1355">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1355">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="32ae3-1356">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-1356">Az.Resources</span></span>

* <span data-ttu-id="32ae3-1357">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="32ae3-1357">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="32ae3-1358">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1358">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="32ae3-1359">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-1359">Az.Sql</span></span>

* <span data-ttu-id="32ae3-1360">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="32ae3-1360">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="32ae3-1361">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="32ae3-1361">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="32ae3-1362">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1362">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="32ae3-1363">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="32ae3-1363">Az.Storage</span></span>

* <span data-ttu-id="32ae3-1364">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="32ae3-1364">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="32ae3-1365">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="32ae3-1365">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="32ae3-1366">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="32ae3-1366">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="32ae3-1367">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="32ae3-1367">Support Static Website configuration</span></span>
    - <span data-ttu-id="32ae3-1368">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="32ae3-1368">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="32ae3-1369">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="32ae3-1369">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="32ae3-1370">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="32ae3-1370">Az.Websites</span></span>

* <span data-ttu-id="32ae3-1371">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="32ae3-1371">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="32ae3-1372">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1372">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="32ae3-1373">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1373">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="32ae3-1374">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="32ae3-1374">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="32ae3-1375">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="32ae3-1375">Az.ApiManagement</span></span>
* <span data-ttu-id="32ae3-1376">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1376">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="32ae3-1377">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="32ae3-1377">Az.Automation</span></span>
* <span data-ttu-id="32ae3-1378">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="32ae3-1378">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="32ae3-1379">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="32ae3-1379">Added Update Management cmdlets</span></span>
* <span data-ttu-id="32ae3-1380">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="32ae3-1380">Added Source Control cmdlets</span></span>
* <span data-ttu-id="32ae3-1381">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="32ae3-1381">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="32ae3-1382">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="32ae3-1382">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="32ae3-1383">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-1383">Az.Compute</span></span>
* <span data-ttu-id="32ae3-1384">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="32ae3-1384">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="32ae3-1385">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1385">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="32ae3-1386">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="32ae3-1386">Az.ContainerInstance</span></span>
* <span data-ttu-id="32ae3-1387">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1387">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="32ae3-1388">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="32ae3-1388">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="32ae3-1389">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="32ae3-1389">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="32ae3-1390">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-1390">Az.Network</span></span>
* <span data-ttu-id="32ae3-1391">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="32ae3-1391">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="32ae3-1392">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="32ae3-1392">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="32ae3-1393">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1393">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="32ae3-1394">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="32ae3-1394">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="32ae3-1395">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="32ae3-1395">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="32ae3-1396">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1396">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="32ae3-1397">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1397">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="32ae3-1398">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="32ae3-1398">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="32ae3-1399">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="32ae3-1399">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="32ae3-1400">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="32ae3-1400">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="32ae3-1401">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="32ae3-1401">Az.Relay</span></span>
* <span data-ttu-id="32ae3-1402">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1402">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="32ae3-1403">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-1403">Az.Resources</span></span>
* <span data-ttu-id="32ae3-1404">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="32ae3-1404">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="32ae3-1405">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="32ae3-1405">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="32ae3-1406">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="32ae3-1406">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="32ae3-1407">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="32ae3-1407">Az.ServiceFabric</span></span>
* <span data-ttu-id="32ae3-1408">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="32ae3-1408">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="32ae3-1409">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-1409">Az.Sql</span></span>
* <span data-ttu-id="32ae3-1410">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="32ae3-1410">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="32ae3-1411">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="32ae3-1411">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="32ae3-1412">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="32ae3-1412">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="32ae3-1413">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="32ae3-1413">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="32ae3-1414">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="32ae3-1414">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="32ae3-1415">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="32ae3-1415">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="32ae3-1416">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="32ae3-1416">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="32ae3-1417">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="32ae3-1417">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="32ae3-1418">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="32ae3-1418">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="32ae3-1419">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1419">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="32ae3-1420">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1420">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="32ae3-1421">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1421">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="32ae3-1422">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1422">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="32ae3-1423">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1423">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="32ae3-1424">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1424">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="32ae3-1425">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1425">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="32ae3-1426">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="32ae3-1426">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="32ae3-1427">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="32ae3-1427">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="32ae3-1428">Geral</span><span class="sxs-lookup"><span data-stu-id="32ae3-1428">General</span></span>
* <span data-ttu-id="32ae3-1429">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="32ae3-1429">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="32ae3-1430">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="32ae3-1430">Az.Profile</span></span>
* <span data-ttu-id="32ae3-1431">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="32ae3-1431">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="32ae3-1432">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="32ae3-1432">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="32ae3-1433">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="32ae3-1433">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="32ae3-1434">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="32ae3-1434">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="32ae3-1435">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="32ae3-1435">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="32ae3-1436">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="32ae3-1436">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="32ae3-1437">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="32ae3-1437">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="32ae3-1438">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-1438">Az.CognitiveServices</span></span>
* <span data-ttu-id="32ae3-1439">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1439">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-1440">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-1440">Az.Compute</span></span>
* <span data-ttu-id="32ae3-1441">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="32ae3-1441">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="32ae3-1442">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="32ae3-1442">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="32ae3-1443">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1443">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="32ae3-1444">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="32ae3-1444">Az.DataLakeStore</span></span>
* <span data-ttu-id="32ae3-1445">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1445">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="32ae3-1446">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1446">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="32ae3-1447">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="32ae3-1447">Az.Insights</span></span>
* <span data-ttu-id="32ae3-1448">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="32ae3-1448">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="32ae3-1449">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="32ae3-1449">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="32ae3-1450">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="32ae3-1450">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="32ae3-1451">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="32ae3-1451">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-1452">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-1452">Az.Network</span></span>
* <span data-ttu-id="32ae3-1453">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="32ae3-1453">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="32ae3-1454">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="32ae3-1454">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="32ae3-1455">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="32ae3-1455">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="32ae3-1456">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="32ae3-1456">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="32ae3-1457">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="32ae3-1457">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="32ae3-1458">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="32ae3-1458">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="32ae3-1459">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="32ae3-1459">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="32ae3-1460">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="32ae3-1460">Az.PolicyInsights</span></span>
* <span data-ttu-id="32ae3-1461">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="32ae3-1461">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-1462">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-1462">Az.Resources</span></span>
* <span data-ttu-id="32ae3-1463">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="32ae3-1463">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="32ae3-1464">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="32ae3-1464">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="32ae3-1465">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="32ae3-1465">Az.ServiceBus</span></span>
* <span data-ttu-id="32ae3-1466">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1466">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="32ae3-1467">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="32ae3-1467">Az.ServiceFabric</span></span>
* <span data-ttu-id="32ae3-1468">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1468">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="32ae3-1469">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="32ae3-1469">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="32ae3-1470">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="32ae3-1470">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="32ae3-1471">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="32ae3-1471">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="32ae3-1472">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1472">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="32ae3-1473">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="32ae3-1473">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="32ae3-1474">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="32ae3-1474">Az.Profile</span></span>
* <span data-ttu-id="32ae3-1475">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="32ae3-1475">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="32ae3-1476">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="32ae3-1476">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-1477">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-1477">Az.Compute</span></span>
* <span data-ttu-id="32ae3-1478">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="32ae3-1478">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="32ae3-1479">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1479">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="32ae3-1480">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="32ae3-1480">Az.DataLakeStore</span></span>
* <span data-ttu-id="32ae3-1481">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="32ae3-1481">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="32ae3-1482">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1482">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="32ae3-1483">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1483">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="32ae3-1484">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1484">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="32ae3-1485">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1485">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-1486">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-1486">Az.Network</span></span>
* <span data-ttu-id="32ae3-1487">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1487">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="32ae3-1488">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1488">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-1489">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-1489">Az.Resources</span></span>
* <span data-ttu-id="32ae3-1490">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1490">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="32ae3-1491">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="32ae3-1491">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="32ae3-1492">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="32ae3-1492">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="32ae3-1493">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="32ae3-1493">Azure.Storage</span></span>
* <span data-ttu-id="32ae3-1494">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="32ae3-1494">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="32ae3-1495">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="32ae3-1495">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="32ae3-1496">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="32ae3-1496">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="32ae3-1497">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1497">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="32ae3-1498">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="32ae3-1498">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="32ae3-1499">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="32ae3-1499">Az.CognitiveServices</span></span>
* <span data-ttu-id="32ae3-1500">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1500">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="32ae3-1501">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="32ae3-1501">Az.Compute</span></span>
* <span data-ttu-id="32ae3-1502">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="32ae3-1502">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="32ae3-1503">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1503">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="32ae3-1504">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="32ae3-1504">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="32ae3-1505">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="32ae3-1505">Az.DataFactoryV2</span></span>
* <span data-ttu-id="32ae3-1506">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1506">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="32ae3-1507">Az.Network</span><span class="sxs-lookup"><span data-stu-id="32ae3-1507">Az.Network</span></span>
* <span data-ttu-id="32ae3-1508">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1508">Added NetworkProfile functionality.</span></span> <span data-ttu-id="32ae3-1509">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="32ae3-1509">new cmdlets added</span></span>
    - <span data-ttu-id="32ae3-1510">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="32ae3-1510">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="32ae3-1511">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="32ae3-1511">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="32ae3-1512">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="32ae3-1512">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="32ae3-1513">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="32ae3-1513">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="32ae3-1514">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-1514">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="32ae3-1515">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-1515">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="32ae3-1516">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="32ae3-1516">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="32ae3-1517">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="32ae3-1517">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="32ae3-1518">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="32ae3-1518">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="32ae3-1519">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="32ae3-1519">Az.RedisCache</span></span>
* <span data-ttu-id="32ae3-1520">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="32ae3-1520">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="32ae3-1521">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="32ae3-1521">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="32ae3-1522">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="32ae3-1522">Az.Resources</span></span>
* <span data-ttu-id="32ae3-1523">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="32ae3-1523">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="32ae3-1524">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="32ae3-1524">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="32ae3-1525">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="32ae3-1525">Az.Sql</span></span>
* <span data-ttu-id="32ae3-1526">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="32ae3-1526">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="32ae3-1527">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="32ae3-1527">Az.Websites</span></span>
* <span data-ttu-id="32ae3-1528">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="32ae3-1528">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="32ae3-1529">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="32ae3-1529">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="32ae3-1530">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="32ae3-1530">0.2.0 - September 2018</span></span>
 <span data-ttu-id="32ae3-1531">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="32ae3-1531">Initial Release</span></span>
