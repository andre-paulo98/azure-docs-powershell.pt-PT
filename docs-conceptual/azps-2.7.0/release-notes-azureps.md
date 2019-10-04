---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/25/2019
ms.openlocfilehash: b879d970d3237098e481dba0419ee65efa8d51cd
ms.sourcegitcommit: f0f09eee03ef9dd7fe07432252a3dc8ca93e3a7b
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2019
ms.locfileid: "71319319"
---
## <a name="270---september-2019"></a><span data-ttu-id="20a83-103">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-103">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="20a83-104">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="20a83-104">Az.ApiManagement</span></span>
* <span data-ttu-id="20a83-105">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="20a83-105">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="20a83-106">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="20a83-106">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="20a83-107">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="20a83-107">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="20a83-108">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="20a83-108">Az.Automation</span></span>
* <span data-ttu-id="20a83-109">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="20a83-109">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="20a83-110">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="20a83-110">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="20a83-111">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="20a83-111">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-112">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-112">Az.Compute</span></span>
* <span data-ttu-id="20a83-113">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-113">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="20a83-114">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-114">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="20a83-115">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="20a83-115">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="20a83-116">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="20a83-116">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="20a83-117">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="20a83-117">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="20a83-118">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="20a83-118">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="20a83-119">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="20a83-119">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="20a83-120">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="20a83-120">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="20a83-121">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="20a83-121">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="20a83-122">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="20a83-122">Az.DataFactory</span></span>
* <span data-ttu-id="20a83-123">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="20a83-123">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="20a83-124">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="20a83-124">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="20a83-125">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="20a83-125">Az.HDInsight</span></span>
* <span data-ttu-id="20a83-126">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="20a83-126">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="20a83-127">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="20a83-127">Az.IotHub</span></span>
* <span data-ttu-id="20a83-128">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="20a83-128">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="20a83-129">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="20a83-129">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="20a83-130">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="20a83-130">New cmdlets are:</span></span>
    - <span data-ttu-id="20a83-131">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="20a83-131">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="20a83-132">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="20a83-132">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="20a83-133">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="20a83-133">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="20a83-134">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="20a83-134">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="20a83-135">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="20a83-135">Az.Monitor</span></span>
* <span data-ttu-id="20a83-136">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="20a83-136">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="20a83-137">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="20a83-137">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="20a83-138">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="20a83-138">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="20a83-139">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="20a83-139">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="20a83-140">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="20a83-140">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="20a83-141">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="20a83-141">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="20a83-142">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="20a83-142">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="20a83-143">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="20a83-143">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="20a83-144">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="20a83-144">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="20a83-145">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="20a83-145">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="20a83-146">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="20a83-146">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="20a83-147">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="20a83-147">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="20a83-148">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="20a83-148">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="20a83-149">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="20a83-149">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="20a83-150">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="20a83-150">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="20a83-151">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="20a83-151">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="20a83-152">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="20a83-152">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="20a83-153">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="20a83-153">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="20a83-154">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="20a83-154">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="20a83-155">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="20a83-155">Overall improved help files</span></span>
* <span data-ttu-id="20a83-156">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="20a83-156">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-157">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-157">Az.Network</span></span>
* <span data-ttu-id="20a83-158">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="20a83-158">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="20a83-159">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="20a83-159">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="20a83-160">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="20a83-160">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="20a83-161">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="20a83-161">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="20a83-162">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="20a83-162">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="20a83-163">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="20a83-163">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="20a83-164">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="20a83-164">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="20a83-165">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="20a83-165">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="20a83-166">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="20a83-166">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="20a83-167">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="20a83-167">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="20a83-168">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="20a83-168">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="20a83-169">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="20a83-169">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="20a83-170">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="20a83-170">New cmdlets</span></span>
        - <span data-ttu-id="20a83-171">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="20a83-171">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="20a83-172">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="20a83-172">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="20a83-173">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="20a83-173">Updated cmdlet:</span></span>
        - <span data-ttu-id="20a83-174">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="20a83-174">New-VpnSite</span></span>
        - <span data-ttu-id="20a83-175">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="20a83-175">Update-VpnSite</span></span>
        - <span data-ttu-id="20a83-176">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="20a83-176">New-VpnConnection</span></span>
        - <span data-ttu-id="20a83-177">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="20a83-177">Update-VpnConnection</span></span>
* <span data-ttu-id="20a83-178">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="20a83-178">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="20a83-179">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="20a83-179">Az.RecoveryServices</span></span>
* <span data-ttu-id="20a83-180">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="20a83-180">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="20a83-181">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="20a83-181">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-182">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-182">Az.Resources</span></span>
* <span data-ttu-id="20a83-183">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="20a83-183">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="20a83-184">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="20a83-184">Az.ServiceFabric</span></span>
* <span data-ttu-id="20a83-185">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="20a83-185">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="20a83-186">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="20a83-186">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="20a83-187">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="20a83-187">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="20a83-188">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="20a83-188">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="20a83-189">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="20a83-189">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="20a83-190">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="20a83-190">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="20a83-191">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="20a83-191">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="20a83-192">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="20a83-192">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="20a83-193">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="20a83-193">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="20a83-194">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="20a83-194">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="20a83-195">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="20a83-195">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="20a83-196">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="20a83-196">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="20a83-197">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="20a83-197">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="20a83-198">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="20a83-198">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="20a83-199">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="20a83-199">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="20a83-200">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="20a83-200">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="20a83-201">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="20a83-201">Az.SignalR</span></span>
* <span data-ttu-id="20a83-202">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="20a83-202">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-203">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-203">Az.Sql</span></span>
* <span data-ttu-id="20a83-204">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="20a83-204">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="20a83-205">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="20a83-205">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="20a83-206">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="20a83-206">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="20a83-207">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="20a83-207">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="20a83-208">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="20a83-208">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="20a83-209">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="20a83-209">Az.Storage</span></span>
* <span data-ttu-id="20a83-210">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="20a83-210">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="20a83-211">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="20a83-211">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="20a83-212">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="20a83-212">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="20a83-213">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="20a83-213">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="20a83-214">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="20a83-214">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="20a83-215">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="20a83-215">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="20a83-216">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="20a83-216">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="20a83-217">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="20a83-217">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="20a83-218">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="20a83-218">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="20a83-219">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="20a83-219">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="20a83-220">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="20a83-220">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="20a83-221">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="20a83-221">Az.Websites</span></span>
* <span data-ttu-id="20a83-222">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="20a83-222">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="20a83-223">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="20a83-223">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="20a83-224">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="20a83-224">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="20a83-225">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-225">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="20a83-226">Geral</span><span class="sxs-lookup"><span data-stu-id="20a83-226">General</span></span>
* <span data-ttu-id="20a83-227">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="20a83-227">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="20a83-228">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-228">Az.Accounts</span></span>
* <span data-ttu-id="20a83-229">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="20a83-229">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="20a83-230">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="20a83-230">Az.Aks</span></span>
* <span data-ttu-id="20a83-231">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="20a83-231">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="20a83-232">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="20a83-232">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="20a83-233">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="20a83-233">Az.ApiManagement</span></span>
* <span data-ttu-id="20a83-234">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="20a83-234">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="20a83-235">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="20a83-235">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="20a83-236">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="20a83-236">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="20a83-237">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="20a83-237">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="20a83-238">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="20a83-238">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="20a83-239">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="20a83-239">Az.Batch</span></span>
* <span data-ttu-id="20a83-240">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="20a83-240">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="20a83-241">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="20a83-241">Az.Cdn</span></span>
* <span data-ttu-id="20a83-242">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="20a83-242">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-243">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-243">Az.Compute</span></span>
* <span data-ttu-id="20a83-244">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-244">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="20a83-245">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="20a83-245">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="20a83-246">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="20a83-246">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="20a83-247">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="20a83-247">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="20a83-248">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="20a83-248">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="20a83-249">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="20a83-249">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="20a83-250">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="20a83-250">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="20a83-251">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="20a83-251">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="20a83-252">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="20a83-252">Az.DataFactory</span></span>
* <span data-ttu-id="20a83-253">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="20a83-253">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="20a83-254">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="20a83-254">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="20a83-255">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="20a83-255">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="20a83-256">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="20a83-256">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="20a83-257">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="20a83-257">Az.DataLakeStore</span></span>
* <span data-ttu-id="20a83-258">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="20a83-258">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="20a83-259">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="20a83-259">Az.EventHub</span></span>
* <span data-ttu-id="20a83-260">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="20a83-260">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="20a83-261">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="20a83-261">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="20a83-262">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="20a83-262">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="20a83-263">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="20a83-263">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="20a83-264">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="20a83-264">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="20a83-265">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="20a83-265">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="20a83-266">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="20a83-266">Az.Monitor</span></span>
* <span data-ttu-id="20a83-267">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="20a83-267">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-268">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-268">Az.Network</span></span>
* <span data-ttu-id="20a83-269">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="20a83-269">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="20a83-270">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="20a83-270">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="20a83-271">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="20a83-271">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="20a83-272">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="20a83-272">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="20a83-273">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="20a83-273">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="20a83-274">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="20a83-274">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="20a83-275">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="20a83-275">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="20a83-276">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="20a83-276">Az.OperationalInsights</span></span>
* <span data-ttu-id="20a83-277">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="20a83-277">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="20a83-278">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="20a83-278">Added example</span></span>
    - <span data-ttu-id="20a83-279">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="20a83-279">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="20a83-280">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="20a83-280">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="20a83-281">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="20a83-281">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="20a83-282">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="20a83-282">Az.RecoveryServices</span></span>
* <span data-ttu-id="20a83-283">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="20a83-283">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-284">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-284">Az.Resources</span></span>
* <span data-ttu-id="20a83-285">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="20a83-285">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="20a83-286">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="20a83-286">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="20a83-287">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="20a83-287">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="20a83-288">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="20a83-288">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="20a83-289">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="20a83-289">Az.ServiceBus</span></span>
* <span data-ttu-id="20a83-290">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="20a83-290">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="20a83-291">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="20a83-291">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="20a83-292">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="20a83-292">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="20a83-293">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="20a83-293">Az.ServiceFabric</span></span>
* <span data-ttu-id="20a83-294">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="20a83-294">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="20a83-295">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="20a83-295">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="20a83-296">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="20a83-296">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="20a83-297">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="20a83-297">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="20a83-298">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="20a83-298">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="20a83-299">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="20a83-299">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-300">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-300">Az.Sql</span></span>
* <span data-ttu-id="20a83-301">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="20a83-301">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="20a83-302">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="20a83-302">Az.Storage</span></span>
* <span data-ttu-id="20a83-303">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="20a83-303">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="20a83-304">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="20a83-304">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="20a83-305">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="20a83-305">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="20a83-306">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="20a83-306">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="20a83-307">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="20a83-307">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="20a83-308">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="20a83-308">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="20a83-309">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="20a83-309">Az.Websites</span></span>
* <span data-ttu-id="20a83-310">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="20a83-310">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="20a83-311">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-311">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="20a83-312">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-312">Az.Accounts</span></span>
* <span data-ttu-id="20a83-313">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="20a83-313">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="20a83-314">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="20a83-314">Az.ApplicationInsights</span></span>
* <span data-ttu-id="20a83-315">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="20a83-315">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="20a83-316">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="20a83-316">Az.Automation</span></span>
* <span data-ttu-id="20a83-317">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="20a83-317">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="20a83-318">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="20a83-318">Az.CognitiveServices</span></span>
* <span data-ttu-id="20a83-319">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="20a83-319">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-320">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-320">Az.Compute</span></span>
* <span data-ttu-id="20a83-321">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="20a83-321">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="20a83-322">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="20a83-322">Az.ContainerRegistry</span></span>
* <span data-ttu-id="20a83-323">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="20a83-323">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="20a83-324">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="20a83-324">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="20a83-325">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="20a83-325">Az.DataFactory</span></span>
* <span data-ttu-id="20a83-326">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="20a83-326">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="20a83-327">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="20a83-327">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="20a83-328">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="20a83-328">Az.EventHub</span></span>
* <span data-ttu-id="20a83-329">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="20a83-329">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="20a83-330">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="20a83-330">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="20a83-331">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="20a83-331">Az.KeyVault</span></span>
* <span data-ttu-id="20a83-332">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="20a83-332">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="20a83-333">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="20a83-333">Az.LogicApp</span></span>
* <span data-ttu-id="20a83-334">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="20a83-334">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="20a83-335">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="20a83-335">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="20a83-336">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="20a83-336">Az.ManagedServices</span></span>
* <span data-ttu-id="20a83-337">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="20a83-337">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-338">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-338">Az.Network</span></span>
* <span data-ttu-id="20a83-339">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="20a83-339">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="20a83-340">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="20a83-340">New cmdlets</span></span>
        - <span data-ttu-id="20a83-341">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="20a83-341">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="20a83-342">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="20a83-342">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="20a83-343">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="20a83-343">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="20a83-344">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="20a83-344">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="20a83-345">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="20a83-345">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="20a83-346">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="20a83-346">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="20a83-347">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="20a83-347">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="20a83-348">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="20a83-348">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="20a83-349">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="20a83-349">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="20a83-350">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-350">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="20a83-351">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="20a83-351">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="20a83-352">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="20a83-352">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="20a83-353">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="20a83-353">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="20a83-354">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="20a83-354">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="20a83-355">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="20a83-355">Updated cmdlets</span></span>
        - <span data-ttu-id="20a83-356">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-356">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="20a83-357">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-357">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="20a83-358">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-358">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="20a83-359">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="20a83-359">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="20a83-360">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="20a83-360">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="20a83-361">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="20a83-361">Updated cmdlet:</span></span>
        - <span data-ttu-id="20a83-362">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-362">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="20a83-363">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-363">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="20a83-364">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-364">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="20a83-365">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="20a83-365">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="20a83-366">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="20a83-366">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="20a83-367">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="20a83-367">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="20a83-368">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="20a83-368">Az.OperationalInsights</span></span>
* <span data-ttu-id="20a83-369">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="20a83-369">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="20a83-370">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="20a83-370">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="20a83-371">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="20a83-371">Az.RecoveryServices</span></span>
* <span data-ttu-id="20a83-372">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="20a83-372">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="20a83-373">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="20a83-373">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="20a83-374">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="20a83-374">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="20a83-375">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="20a83-375">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="20a83-376">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="20a83-376">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="20a83-377">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="20a83-377">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="20a83-378">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="20a83-378">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="20a83-379">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="20a83-379">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="20a83-380">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="20a83-380">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="20a83-381">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="20a83-381">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-382">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-382">Az.Resources</span></span>
- <span data-ttu-id="20a83-383">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="20a83-383">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="20a83-384">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="20a83-384">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="20a83-385">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="20a83-385">Az.ServiceBus</span></span>
* <span data-ttu-id="20a83-386">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="20a83-386">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="20a83-387">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="20a83-387">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-388">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-388">Az.Sql</span></span>
* <span data-ttu-id="20a83-389">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="20a83-389">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="20a83-390">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="20a83-390">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="20a83-391">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="20a83-391">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="20a83-392">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="20a83-392">Az.Storage</span></span>
* <span data-ttu-id="20a83-393">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="20a83-393">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="20a83-394">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="20a83-394">Az.StorageSync</span></span>
* <span data-ttu-id="20a83-395">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="20a83-395">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="20a83-396">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="20a83-396">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="20a83-397">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="20a83-397">Az.Websites</span></span>
* <span data-ttu-id="20a83-398">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="20a83-398">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="20a83-399">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="20a83-399">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="20a83-400">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="20a83-400">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="20a83-401">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-401">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="20a83-402">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-402">Az.Accounts</span></span>
* <span data-ttu-id="20a83-403">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="20a83-403">Add support for profile cmdlets</span></span>
* <span data-ttu-id="20a83-404">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="20a83-404">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="20a83-405">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="20a83-405">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="20a83-406">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="20a83-406">Az.Advisor</span></span>
* <span data-ttu-id="20a83-407">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="20a83-407">GA release of Az.Advisor</span></span>
* <span data-ttu-id="20a83-408">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="20a83-408">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="20a83-409">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="20a83-409">Az.ApiManagement</span></span>
* <span data-ttu-id="20a83-410">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="20a83-410">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="20a83-411">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="20a83-411">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="20a83-412">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="20a83-412">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="20a83-413">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="20a83-413">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="20a83-414">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="20a83-414">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="20a83-415">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="20a83-415">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="20a83-416">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="20a83-416">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="20a83-417">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="20a83-417">Az.Automation</span></span>
* <span data-ttu-id="20a83-418">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="20a83-418">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-419">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-419">Az.Compute</span></span>
* <span data-ttu-id="20a83-420">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-420">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="20a83-421">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="20a83-421">Az.DataFactory</span></span>
* <span data-ttu-id="20a83-422">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="20a83-422">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="20a83-423">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="20a83-423">Az.EventGrid</span></span>
* <span data-ttu-id="20a83-424">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="20a83-424">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="20a83-425">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="20a83-425">Az.IotHub</span></span>
* <span data-ttu-id="20a83-426">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="20a83-426">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-427">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-427">Az.Network</span></span>
* <span data-ttu-id="20a83-428">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="20a83-428">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="20a83-429">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="20a83-429">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="20a83-430">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="20a83-430">Az.PolicyInsights</span></span>
* <span data-ttu-id="20a83-431">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="20a83-431">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="20a83-432">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="20a83-432">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="20a83-433">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="20a83-433">Az.OperationalInsights</span></span>
* <span data-ttu-id="20a83-434">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="20a83-434">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="20a83-435">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="20a83-435">Az.RecoveryServices</span></span>
* <span data-ttu-id="20a83-436">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="20a83-436">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-437">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-437">Az.Resources</span></span>
    - <span data-ttu-id="20a83-438">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="20a83-438">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="20a83-439">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="20a83-439">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="20a83-440">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="20a83-440">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="20a83-441">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="20a83-441">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="20a83-442">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="20a83-442">Az.ServiceBus</span></span>
* <span data-ttu-id="20a83-443">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="20a83-443">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-444">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-444">Az.Sql</span></span>
* <span data-ttu-id="20a83-445">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="20a83-445">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="20a83-446">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="20a83-446">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="20a83-447">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="20a83-447">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="20a83-448">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="20a83-448">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="20a83-449">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="20a83-449">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="20a83-450">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="20a83-450">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="20a83-451">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="20a83-451">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="20a83-452">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="20a83-452">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="20a83-453">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="20a83-453">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="20a83-454">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="20a83-454">Az.Storage</span></span>
* <span data-ttu-id="20a83-455">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="20a83-455">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="20a83-456">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="20a83-456">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="20a83-457">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="20a83-457">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="20a83-458">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="20a83-458">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="20a83-459">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="20a83-459">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="20a83-460">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="20a83-460">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="20a83-461">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="20a83-461">Set-AzStorageAccount</span></span>
* <span data-ttu-id="20a83-462">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="20a83-462">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="20a83-463">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="20a83-463">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="20a83-464">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="20a83-464">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="20a83-465">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="20a83-465">Az.StorageSync</span></span>
* <span data-ttu-id="20a83-466">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="20a83-466">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="20a83-467">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-467">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="20a83-468">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-468">Az.Accounts</span></span>
* <span data-ttu-id="20a83-469">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="20a83-469">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="20a83-470">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="20a83-470">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="20a83-471">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="20a83-471">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="20a83-472">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="20a83-472">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="20a83-473">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="20a83-473">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-474">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-474">Az.Compute</span></span>
* <span data-ttu-id="20a83-475">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="20a83-475">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="20a83-476">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="20a83-476">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="20a83-477">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="20a83-477">Az.Dns</span></span>
* <span data-ttu-id="20a83-478">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="20a83-478">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="20a83-479">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="20a83-479">Az.EventGrid</span></span>
* <span data-ttu-id="20a83-480">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="20a83-480">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="20a83-481">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="20a83-481">New cmdlets:</span></span>
    - <span data-ttu-id="20a83-482">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="20a83-482">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="20a83-483">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="20a83-483">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="20a83-484">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="20a83-484">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="20a83-485">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="20a83-485">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="20a83-486">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="20a83-486">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="20a83-487">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="20a83-487">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="20a83-488">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="20a83-488">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="20a83-489">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="20a83-489">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="20a83-490">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="20a83-490">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="20a83-491">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="20a83-491">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="20a83-492">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="20a83-492">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="20a83-493">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="20a83-493">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="20a83-494">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="20a83-494">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="20a83-495">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="20a83-495">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="20a83-496">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="20a83-496">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="20a83-497">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="20a83-497">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="20a83-498">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="20a83-498">Updated cmdlets:</span></span>
    - <span data-ttu-id="20a83-499">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="20a83-499">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="20a83-500">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="20a83-500">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="20a83-501">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="20a83-501">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="20a83-502">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="20a83-502">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="20a83-503">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="20a83-503">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="20a83-504">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="20a83-504">Event subscription expiration date,</span></span>
            - <span data-ttu-id="20a83-505">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="20a83-505">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="20a83-506">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="20a83-506">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="20a83-507">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="20a83-507">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="20a83-508">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="20a83-508">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="20a83-509">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="20a83-509">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="20a83-510">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="20a83-510">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="20a83-511">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="20a83-511">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="20a83-512">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="20a83-512">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="20a83-513">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="20a83-513">Az.FrontDoor</span></span>
* <span data-ttu-id="20a83-514">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="20a83-514">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="20a83-515">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="20a83-515">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="20a83-516">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="20a83-516">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="20a83-517">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="20a83-517">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-518">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-518">Az.Network</span></span>
* <span data-ttu-id="20a83-519">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="20a83-519">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="20a83-520">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="20a83-520">New cmdlets</span></span>
        - <span data-ttu-id="20a83-521">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="20a83-521">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="20a83-522">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="20a83-522">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="20a83-523">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="20a83-523">New cmdlets</span></span> 
        - <span data-ttu-id="20a83-524">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="20a83-524">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="20a83-525">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="20a83-525">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="20a83-526">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="20a83-526">New cmdlets</span></span> 
        - <span data-ttu-id="20a83-527">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="20a83-527">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="20a83-528">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="20a83-528">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="20a83-529">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="20a83-529">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="20a83-530">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-530">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="20a83-531">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="20a83-531">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="20a83-532">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="20a83-532">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="20a83-533">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="20a83-533">New cmdlets</span></span>
        - <span data-ttu-id="20a83-534">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="20a83-534">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="20a83-535">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="20a83-535">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="20a83-536">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="20a83-536">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="20a83-537">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="20a83-537">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="20a83-538">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="20a83-538">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="20a83-539">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="20a83-539">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="20a83-540">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="20a83-540">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="20a83-541">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="20a83-541">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="20a83-542">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="20a83-542">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="20a83-543">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="20a83-543">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="20a83-544">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="20a83-544">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="20a83-545">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="20a83-545">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="20a83-546">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="20a83-546">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="20a83-547">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="20a83-547">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="20a83-548">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="20a83-548">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="20a83-549">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="20a83-549">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="20a83-550">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="20a83-550">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="20a83-551">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="20a83-551">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="20a83-552">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="20a83-552">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="20a83-553">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="20a83-553">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="20a83-554">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="20a83-554">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="20a83-555">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="20a83-555">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="20a83-556">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="20a83-556">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="20a83-557">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="20a83-557">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="20a83-558">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="20a83-558">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="20a83-559">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="20a83-559">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="20a83-560">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="20a83-560">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="20a83-561">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="20a83-561">Az.OperationalInsights</span></span>
* <span data-ttu-id="20a83-562">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="20a83-562">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-563">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-563">Az.Resources</span></span>
* <span data-ttu-id="20a83-564">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="20a83-564">Support for additional Template Export options</span></span>
    - <span data-ttu-id="20a83-565">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="20a83-565">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="20a83-566">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="20a83-566">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="20a83-567">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="20a83-567">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="20a83-568">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="20a83-568">Az.ServiceFabric</span></span>
* <span data-ttu-id="20a83-569">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="20a83-569">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-570">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-570">Az.Sql</span></span>
* <span data-ttu-id="20a83-571">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="20a83-571">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="20a83-572">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="20a83-572">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="20a83-573">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="20a83-573">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="20a83-574">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="20a83-574">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="20a83-575">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="20a83-575">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="20a83-576">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="20a83-576">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="20a83-577">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="20a83-577">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="20a83-578">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="20a83-578">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="20a83-579">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="20a83-579">Az.Storage</span></span>
* <span data-ttu-id="20a83-580">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="20a83-580">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="20a83-581">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="20a83-581">New-AzStorageAccount</span></span>
* <span data-ttu-id="20a83-582">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="20a83-582">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="20a83-583">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="20a83-583">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="20a83-584">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="20a83-584">Az.Websites</span></span>
* <span data-ttu-id="20a83-585">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="20a83-585">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="20a83-586">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="20a83-586">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="20a83-587">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-587">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="20a83-588">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="20a83-588">Az.Cdn</span></span>
* <span data-ttu-id="20a83-589">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="20a83-589">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-590">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-590">Az.Compute</span></span>
* <span data-ttu-id="20a83-591">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="20a83-591">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="20a83-592">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="20a83-592">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="20a83-593">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="20a83-593">Az.EventHub</span></span>
* <span data-ttu-id="20a83-594">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="20a83-594">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="20a83-595">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="20a83-595">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-596">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-596">Az.Network</span></span>
* <span data-ttu-id="20a83-597">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="20a83-597">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="20a83-598">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="20a83-598">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="20a83-599">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="20a83-599">Az.PolicyInsights</span></span>
* <span data-ttu-id="20a83-600">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="20a83-600">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="20a83-601">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="20a83-601">Az.RecoveryServices</span></span>
* <span data-ttu-id="20a83-602">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="20a83-602">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="20a83-603">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="20a83-603">Az.ServiceBus</span></span>
* <span data-ttu-id="20a83-604">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="20a83-604">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="20a83-605">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="20a83-605">Az.ServiceFabric</span></span>
* <span data-ttu-id="20a83-606">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="20a83-606">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="20a83-607">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="20a83-607">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-608">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-608">Az.Sql</span></span>
* <span data-ttu-id="20a83-609">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="20a83-609">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="20a83-610">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="20a83-610">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="20a83-611">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="20a83-611">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="20a83-612">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="20a83-612">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="20a83-613">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="20a83-613">Az.Websites</span></span>
* <span data-ttu-id="20a83-614">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="20a83-614">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="20a83-615">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-615">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="20a83-616">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="20a83-616">Az.ApiManagement</span></span>
* <span data-ttu-id="20a83-617">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="20a83-617">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="20a83-618">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="20a83-618">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="20a83-619">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="20a83-619">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="20a83-620">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="20a83-620">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="20a83-621">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="20a83-621">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="20a83-622">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="20a83-622">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="20a83-623">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="20a83-623">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="20a83-624">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="20a83-624">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="20a83-625">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="20a83-625">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="20a83-626">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="20a83-626">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="20a83-627">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="20a83-627">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="20a83-628">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="20a83-628">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="20a83-629">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="20a83-629">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="20a83-630">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="20a83-630">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="20a83-631">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="20a83-631">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="20a83-632">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="20a83-632">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="20a83-633">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="20a83-633">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="20a83-634">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="20a83-634">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="20a83-635">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="20a83-635">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="20a83-636">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="20a83-636">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="20a83-637">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="20a83-637">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="20a83-638">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="20a83-638">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="20a83-639">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="20a83-639">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="20a83-640">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="20a83-640">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="20a83-641">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="20a83-641">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="20a83-642">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="20a83-642">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="20a83-643">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="20a83-643">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="20a83-644">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="20a83-644">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="20a83-645">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="20a83-645">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="20a83-646">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="20a83-646">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="20a83-647">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="20a83-647">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="20a83-648">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="20a83-648">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="20a83-649">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="20a83-649">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="20a83-650">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="20a83-650">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="20a83-651">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="20a83-651">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="20a83-652">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="20a83-652">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="20a83-653">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="20a83-653">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="20a83-654">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="20a83-654">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="20a83-655">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="20a83-655">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="20a83-656">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="20a83-656">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="20a83-657">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="20a83-657">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="20a83-658">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="20a83-658">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="20a83-659">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="20a83-659">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="20a83-660">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="20a83-660">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="20a83-661">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="20a83-661">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="20a83-662">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="20a83-662">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="20a83-663">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="20a83-663">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="20a83-664">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="20a83-664">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="20a83-665">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="20a83-665">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="20a83-666">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="20a83-666">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="20a83-667">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="20a83-667">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="20a83-668">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="20a83-668">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="20a83-669">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="20a83-669">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="20a83-670">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="20a83-670">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="20a83-671">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="20a83-671">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="20a83-672">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="20a83-672">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="20a83-673">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="20a83-673">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="20a83-674">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="20a83-674">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="20a83-675">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="20a83-675">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="20a83-676">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="20a83-676">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="20a83-677">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="20a83-677">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="20a83-678">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="20a83-678">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="20a83-679">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="20a83-679">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="20a83-680">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="20a83-680">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="20a83-681">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="20a83-681">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="20a83-682">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="20a83-682">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="20a83-683">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="20a83-683">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="20a83-684">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="20a83-684">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="20a83-685">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="20a83-685">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="20a83-686">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="20a83-686">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="20a83-687">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="20a83-687">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="20a83-688">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="20a83-688">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="20a83-689">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="20a83-689">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="20a83-690">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="20a83-690">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="20a83-691">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="20a83-691">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="20a83-692">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="20a83-692">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="20a83-693">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="20a83-693">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="20a83-694">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="20a83-694">Az.Automation</span></span>
* <span data-ttu-id="20a83-695">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="20a83-695">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="20a83-696">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="20a83-696">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="20a83-697">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="20a83-697">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="20a83-698">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="20a83-698">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="20a83-699">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="20a83-699">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="20a83-700">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="20a83-700">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="20a83-701">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="20a83-701">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-702">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-702">Az.Compute</span></span>
* <span data-ttu-id="20a83-703">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="20a83-703">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="20a83-704">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="20a83-704">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="20a83-705">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="20a83-705">Az.DataLakeStore</span></span>
* <span data-ttu-id="20a83-706">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="20a83-706">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="20a83-707">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="20a83-707">Az.Monitor</span></span>
* <span data-ttu-id="20a83-708">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="20a83-708">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-709">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-709">Az.Network</span></span>
* <span data-ttu-id="20a83-710">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="20a83-710">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="20a83-711">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="20a83-711">Updated cmdlet:</span></span>
        - <span data-ttu-id="20a83-712">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="20a83-712">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="20a83-713">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="20a83-713">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-714">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-714">Az.Resources</span></span>
* <span data-ttu-id="20a83-715">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="20a83-715">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-716">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-716">Az.Sql</span></span>
* <span data-ttu-id="20a83-717">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="20a83-717">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="20a83-718">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-718">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="20a83-719">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-719">Az.Accounts</span></span>
* <span data-ttu-id="20a83-720">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="20a83-720">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="20a83-721">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="20a83-721">Az.CognitiveServices</span></span>
* <span data-ttu-id="20a83-722">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="20a83-722">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="20a83-723">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="20a83-723">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-724">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-724">Az.Compute</span></span>
* <span data-ttu-id="20a83-725">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="20a83-725">Proximity placement group feature.</span></span>
    - <span data-ttu-id="20a83-726">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="20a83-726">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="20a83-727">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-727">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="20a83-728">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="20a83-728">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="20a83-729">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="20a83-729">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="20a83-730">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="20a83-730">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="20a83-731">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="20a83-731">Breaking changes</span></span>
    - <span data-ttu-id="20a83-732">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="20a83-732">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="20a83-733">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="20a83-733">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="20a83-734">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="20a83-734">Az.DeploymentManager</span></span>
* <span data-ttu-id="20a83-735">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="20a83-735">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="20a83-736">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="20a83-736">Az.Dns</span></span>
* <span data-ttu-id="20a83-737">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="20a83-737">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="20a83-738">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="20a83-738">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="20a83-739">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="20a83-739">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="20a83-740">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="20a83-740">Az.FrontDoor</span></span>
* <span data-ttu-id="20a83-741">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="20a83-741">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="20a83-742">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="20a83-742">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="20a83-743">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="20a83-743">Az.HDInsight</span></span>
* <span data-ttu-id="20a83-744">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="20a83-744">Removed two cmdlets:</span></span>
    - <span data-ttu-id="20a83-745">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="20a83-745">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="20a83-746">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="20a83-746">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="20a83-747">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="20a83-747">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="20a83-748">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="20a83-748">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="20a83-749">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="20a83-749">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="20a83-750">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="20a83-750">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="20a83-751">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="20a83-751">Az.Monitor</span></span>
* <span data-ttu-id="20a83-752">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="20a83-752">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="20a83-753">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="20a83-753">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="20a83-754">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="20a83-754">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="20a83-755">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="20a83-755">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="20a83-756">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="20a83-756">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="20a83-757">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="20a83-757">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="20a83-758">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="20a83-758">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="20a83-759">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="20a83-759">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="20a83-760">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="20a83-760">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="20a83-761">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="20a83-761">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="20a83-762">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="20a83-762">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="20a83-763">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="20a83-763">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="20a83-764">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="20a83-764">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="20a83-765">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="20a83-765">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-766">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-766">Az.Network</span></span>
* <span data-ttu-id="20a83-767">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="20a83-767">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="20a83-768">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="20a83-768">New cmdlets</span></span>
        - <span data-ttu-id="20a83-769">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="20a83-769">New-AzNatGateway</span></span>
        - <span data-ttu-id="20a83-770">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="20a83-770">Get-AzNatGateway</span></span>
        - <span data-ttu-id="20a83-771">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="20a83-771">Set-AzNatGateway</span></span>
        - <span data-ttu-id="20a83-772">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="20a83-772">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="20a83-773">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="20a83-773">Updated cmdlets</span></span>
        - <span data-ttu-id="20a83-774">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="20a83-774">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="20a83-775">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="20a83-775">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="20a83-776">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="20a83-776">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="20a83-777">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="20a83-777">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="20a83-778">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="20a83-778">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="20a83-779">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="20a83-779">Az.PolicyInsights</span></span>
* <span data-ttu-id="20a83-780">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="20a83-780">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="20a83-781">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="20a83-781">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="20a83-782">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="20a83-782">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="20a83-783">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="20a83-783">Az.RecoveryServices</span></span>
* <span data-ttu-id="20a83-784">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="20a83-784">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="20a83-785">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="20a83-785">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="20a83-786">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="20a83-786">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="20a83-787">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="20a83-787">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="20a83-788">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="20a83-788">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="20a83-789">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="20a83-789">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="20a83-790">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="20a83-790">Az.Relay</span></span>
* <span data-ttu-id="20a83-791">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="20a83-791">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="20a83-792">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="20a83-792">Az.ServiceBus</span></span>
* <span data-ttu-id="20a83-793">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="20a83-793">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="20a83-794">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="20a83-794">Az.Storage</span></span>
* <span data-ttu-id="20a83-795">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="20a83-795">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="20a83-796">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="20a83-796">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="20a83-797">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="20a83-797">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="20a83-798">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="20a83-798">New-AzStorageAccount</span></span>
* <span data-ttu-id="20a83-799">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="20a83-799">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="20a83-800">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="20a83-800">New-AzStorageAccount</span></span>
    - <span data-ttu-id="20a83-801">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="20a83-801">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="20a83-802">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="20a83-802">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="20a83-803">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="20a83-803">Az.Websites</span></span>
* <span data-ttu-id="20a83-804">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="20a83-804">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="20a83-805">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="20a83-805">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="20a83-806">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-806">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="20a83-807">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="20a83-807">Highlights since the last major release</span></span>
* <span data-ttu-id="20a83-808">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="20a83-808">General availability of `Az` module</span></span>
* <span data-ttu-id="20a83-809">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="20a83-809">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="20a83-810">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="20a83-810">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="20a83-811">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-811">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="20a83-812">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="20a83-812">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="20a83-813">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="20a83-813">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="20a83-814">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="20a83-814">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="20a83-815">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-815">Az.Accounts</span></span>
* <span data-ttu-id="20a83-816">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="20a83-816">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="20a83-817">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="20a83-817">Az.Batch</span></span>
* <span data-ttu-id="20a83-818">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-818">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="20a83-819">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="20a83-819">Az.Cdn</span></span>
* <span data-ttu-id="20a83-820">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-820">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="20a83-821">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="20a83-821">Az.CognitiveServices</span></span>
* <span data-ttu-id="20a83-822">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-822">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-823">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-823">Az.Compute</span></span>
* <span data-ttu-id="20a83-824">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="20a83-824">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="20a83-825">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-825">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="20a83-826">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="20a83-826">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="20a83-827">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="20a83-827">Az.DataFactory</span></span>
* <span data-ttu-id="20a83-828">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="20a83-828">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="20a83-829">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="20a83-829">Az.DataLakeStore</span></span>
* <span data-ttu-id="20a83-830">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-830">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="20a83-831">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="20a83-831">Az.EventGrid</span></span>
* <span data-ttu-id="20a83-832">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="20a83-832">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="20a83-833">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="20a83-833">Az.EventHub</span></span>
* <span data-ttu-id="20a83-834">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="20a83-834">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="20a83-835">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="20a83-835">Az.HDInsight</span></span>
* <span data-ttu-id="20a83-836">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-836">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="20a83-837">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="20a83-837">Az.IotHub</span></span>
* <span data-ttu-id="20a83-838">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-838">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="20a83-839">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="20a83-839">Az.KeyVault</span></span>
* <span data-ttu-id="20a83-840">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-840">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="20a83-841">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="20a83-841">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="20a83-842">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="20a83-842">Az.MachineLearning</span></span>
* <span data-ttu-id="20a83-843">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-843">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="20a83-844">Az.Media</span><span class="sxs-lookup"><span data-stu-id="20a83-844">Az.Media</span></span>
* <span data-ttu-id="20a83-845">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-845">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="20a83-846">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="20a83-846">Az.Monitor</span></span>
  * <span data-ttu-id="20a83-847">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="20a83-847">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="20a83-848">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="20a83-848">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="20a83-849">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="20a83-849">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="20a83-850">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="20a83-850">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="20a83-851">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="20a83-851">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="20a83-852">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="20a83-852">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="20a83-853">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="20a83-853">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-854">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-854">Az.Network</span></span>
* <span data-ttu-id="20a83-855">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-855">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="20a83-856">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="20a83-856">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="20a83-857">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="20a83-857">Az.NotificationHubs</span></span>
* <span data-ttu-id="20a83-858">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-858">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="20a83-859">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="20a83-859">Az.OperationalInsights</span></span>
* <span data-ttu-id="20a83-860">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-860">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="20a83-861">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="20a83-861">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="20a83-862">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-862">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="20a83-863">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="20a83-863">Az.RecoveryServices</span></span>
* <span data-ttu-id="20a83-864">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-864">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="20a83-865">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="20a83-865">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="20a83-866">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="20a83-866">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="20a83-867">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="20a83-867">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="20a83-868">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="20a83-868">Az.RedisCache</span></span>
* <span data-ttu-id="20a83-869">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-869">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-870">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-870">Az.Resources</span></span>
* <span data-ttu-id="20a83-871">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="20a83-871">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-872">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-872">Az.Sql</span></span>
* <span data-ttu-id="20a83-873">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="20a83-873">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="20a83-874">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-874">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="20a83-875">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="20a83-875">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="20a83-876">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="20a83-876">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="20a83-877">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="20a83-877">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="20a83-878">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="20a83-878">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="20a83-879">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="20a83-879">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="20a83-880">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="20a83-880">Az.Websites</span></span>
* <span data-ttu-id="20a83-881">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="20a83-881">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="20a83-882">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="20a83-882">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="20a83-883">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="20a83-883">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="20a83-884">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="20a83-884">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="20a83-885">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-885">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="20a83-886">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="20a83-886">Highlights since the last major release</span></span>
* <span data-ttu-id="20a83-887">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="20a83-887">General availability of `Az` module</span></span>
* <span data-ttu-id="20a83-888">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="20a83-888">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="20a83-889">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="20a83-889">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="20a83-890">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-890">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="20a83-891">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="20a83-891">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="20a83-892">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="20a83-892">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="20a83-893">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="20a83-893">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="20a83-894">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-894">Az.Accounts</span></span>
* <span data-ttu-id="20a83-895">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="20a83-895">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="20a83-896">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="20a83-896">Az.AnalysisServices</span></span>
* <span data-ttu-id="20a83-897">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="20a83-897">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="20a83-898">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="20a83-898">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="20a83-899">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="20a83-899">Az.Automation</span></span>
* <span data-ttu-id="20a83-900">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="20a83-900">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="20a83-901">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="20a83-901">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="20a83-902">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="20a83-902">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-903">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-903">Az.Compute</span></span>
* <span data-ttu-id="20a83-904">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-904">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="20a83-905">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="20a83-905">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="20a83-906">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="20a83-906">Az.ContainerInstance</span></span>
* <span data-ttu-id="20a83-907">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="20a83-907">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="20a83-908">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="20a83-908">Az.DataFactory</span></span>
* <span data-ttu-id="20a83-909">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="20a83-909">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="20a83-910">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="20a83-910">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-911">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-911">Az.Resources</span></span>
* <span data-ttu-id="20a83-912">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="20a83-912">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="20a83-913">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="20a83-913">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="20a83-914">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="20a83-914">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="20a83-915">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="20a83-915">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="20a83-916">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="20a83-916">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="20a83-917">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="20a83-917">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-918">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-918">Az.Sql</span></span>
* <span data-ttu-id="20a83-919">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="20a83-919">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="20a83-920">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="20a83-920">Az.Storage</span></span>
* <span data-ttu-id="20a83-921">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="20a83-921">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="20a83-922">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="20a83-922">New-AzStorageContext</span></span>
* <span data-ttu-id="20a83-923">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="20a83-923">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="20a83-924">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="20a83-924">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="20a83-925">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="20a83-925">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="20a83-926">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="20a83-926">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="20a83-927">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="20a83-927">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="20a83-928">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="20a83-928">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="20a83-929">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="20a83-929">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="20a83-930">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="20a83-930">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="20a83-931">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="20a83-931">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="20a83-932">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="20a83-932">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="20a83-933">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-933">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="20a83-934">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="20a83-934">Highlights since the last major release</span></span>
* <span data-ttu-id="20a83-935">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="20a83-935">General availability of `Az` module</span></span>
* <span data-ttu-id="20a83-936">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="20a83-936">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="20a83-937">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="20a83-937">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="20a83-938">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-938">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="20a83-939">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="20a83-939">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="20a83-940">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="20a83-940">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="20a83-941">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="20a83-941">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="20a83-942">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="20a83-942">Az.Automation</span></span>
* <span data-ttu-id="20a83-943">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="20a83-943">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="20a83-944">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="20a83-944">Dynamic grouping</span></span>
    * <span data-ttu-id="20a83-945">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="20a83-945">Pre-Post script</span></span>
    * <span data-ttu-id="20a83-946">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="20a83-946">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-947">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-947">Az.Compute</span></span>
* <span data-ttu-id="20a83-948">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="20a83-948">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="20a83-949">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="20a83-949">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="20a83-950">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="20a83-950">Az.KeyVault</span></span>
* <span data-ttu-id="20a83-951">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="20a83-951">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-952">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-952">Az.Network</span></span>
* <span data-ttu-id="20a83-953">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="20a83-953">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="20a83-954">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="20a83-954">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="20a83-955">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="20a83-955">Az.RecoveryServices</span></span>
* <span data-ttu-id="20a83-956">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="20a83-956">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="20a83-957">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="20a83-957">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-958">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-958">Az.Resources</span></span>
* <span data-ttu-id="20a83-959">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="20a83-959">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="20a83-960">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="20a83-960">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-961">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-961">Az.Sql</span></span>
* <span data-ttu-id="20a83-962">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="20a83-962">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="20a83-963">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="20a83-963">Az.Storage</span></span>
* <span data-ttu-id="20a83-964">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="20a83-964">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="20a83-965">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="20a83-965">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="20a83-966">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="20a83-966">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="20a83-967">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="20a83-967">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="20a83-968">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="20a83-968">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="20a83-969">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="20a83-969">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="20a83-970">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="20a83-970">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="20a83-971">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="20a83-971">Az.Websites</span></span>
* <span data-ttu-id="20a83-972">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="20a83-972">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="20a83-973">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-973">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="20a83-974">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-974">Az.Accounts</span></span>
* <span data-ttu-id="20a83-975">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="20a83-975">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="20a83-976">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="20a83-976">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="20a83-977">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="20a83-977">Az.Automation</span></span>
* <span data-ttu-id="20a83-978">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="20a83-978">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="20a83-979">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="20a83-979">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="20a83-980">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="20a83-980">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="20a83-981">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="20a83-981">Az.Cdn</span></span>
* <span data-ttu-id="20a83-982">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="20a83-982">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-983">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-983">Az.Compute</span></span>
* <span data-ttu-id="20a83-984">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="20a83-984">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="20a83-985">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="20a83-985">Az.DataFactory</span></span>
* <span data-ttu-id="20a83-986">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="20a83-986">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="20a83-987">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="20a83-987">Az.LogicApp</span></span>
* <span data-ttu-id="20a83-988">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="20a83-988">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-989">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-989">Az.Network</span></span>
* <span data-ttu-id="20a83-990">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="20a83-990">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="20a83-991">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="20a83-991">Az.RecoveryServices</span></span>
* <span data-ttu-id="20a83-992">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="20a83-992">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="20a83-993">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="20a83-993">SDK Update</span></span>
* <span data-ttu-id="20a83-994">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="20a83-994">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="20a83-995">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="20a83-995">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-996">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-996">Az.Resources</span></span>
* <span data-ttu-id="20a83-997">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="20a83-997">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="20a83-998">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="20a83-998">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="20a83-999">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="20a83-999">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="20a83-1000">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="20a83-1000">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="20a83-1001">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="20a83-1001">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="20a83-1002">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="20a83-1002">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-1003">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-1003">Az.Sql</span></span>
* <span data-ttu-id="20a83-1004">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="20a83-1004">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="20a83-1005">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="20a83-1005">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="20a83-1006">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="20a83-1006">Az.Storage</span></span>
* <span data-ttu-id="20a83-1007">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="20a83-1007">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="20a83-1008">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-1008">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="20a83-1009">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="20a83-1009">Az.AnalysisServices</span></span>
* <span data-ttu-id="20a83-1010">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="20a83-1010">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="20a83-1011">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="20a83-1011">Az.Automation</span></span>
* <span data-ttu-id="20a83-1012">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="20a83-1012">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="20a83-1013">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="20a83-1013">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="20a83-1014">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="20a83-1014">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="20a83-1015">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="20a83-1015">Az.CognitiveServices</span></span>
* <span data-ttu-id="20a83-1016">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="20a83-1016">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-1017">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-1017">Az.Compute</span></span>
* <span data-ttu-id="20a83-1018">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="20a83-1018">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="20a83-1019">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="20a83-1019">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="20a83-1020">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="20a83-1020">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="20a83-1021">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="20a83-1021">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="20a83-1022">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="20a83-1022">Az.DataLakeStore</span></span>
* <span data-ttu-id="20a83-1023">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="20a83-1023">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="20a83-1024">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="20a83-1024">Az.EventHub</span></span>
* <span data-ttu-id="20a83-1025">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="20a83-1025">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="20a83-1026">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="20a83-1026">Az.KeyVault</span></span>
* <span data-ttu-id="20a83-1027">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="20a83-1027">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="20a83-1028">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="20a83-1028">Az.LogicApp</span></span>
* <span data-ttu-id="20a83-1029">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="20a83-1029">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="20a83-1030">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="20a83-1030">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="20a83-1031">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="20a83-1031">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="20a83-1032">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="20a83-1032">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="20a83-1033">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="20a83-1033">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="20a83-1034">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="20a83-1034">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="20a83-1035">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="20a83-1035">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="20a83-1036">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="20a83-1036">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="20a83-1037">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="20a83-1037">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="20a83-1038">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="20a83-1038">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="20a83-1039">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="20a83-1039">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="20a83-1040">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="20a83-1040">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="20a83-1041">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="20a83-1041">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="20a83-1042">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="20a83-1042">Az.Monitor</span></span>
* <span data-ttu-id="20a83-1043">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="20a83-1043">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-1044">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-1044">Az.Network</span></span>
* <span data-ttu-id="20a83-1045">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="20a83-1045">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="20a83-1046">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="20a83-1046">Az.OperationalInsights</span></span>
* <span data-ttu-id="20a83-1047">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="20a83-1047">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="20a83-1048">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="20a83-1048">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="20a83-1049">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="20a83-1049">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="20a83-1050">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-1050">Az.Resources</span></span>
* <span data-ttu-id="20a83-1051">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="20a83-1051">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="20a83-1052">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="20a83-1052">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="20a83-1053">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="20a83-1053">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="20a83-1054">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="20a83-1054">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-1055">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-1055">Az.Sql</span></span>
* <span data-ttu-id="20a83-1056">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="20a83-1056">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="20a83-1057">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="20a83-1057">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="20a83-1058">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="20a83-1058">Az.Websites</span></span>
* <span data-ttu-id="20a83-1059">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="20a83-1059">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="20a83-1060">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-1060">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="20a83-1061">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-1061">Az.Accounts</span></span>
* <span data-ttu-id="20a83-1062">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="20a83-1062">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="20a83-1063">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="20a83-1063">Az.AnalysisServices</span></span>
<span data-ttu-id="20a83-1064">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="20a83-1064">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-1065">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-1065">Az.Compute</span></span>
* <span data-ttu-id="20a83-1066">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="20a83-1066">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="20a83-1067">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="20a83-1067">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="20a83-1068">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="20a83-1068">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="20a83-1069">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="20a83-1069">Az.RecoveryServices</span></span>
<span data-ttu-id="20a83-1070">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="20a83-1070">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-1071">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-1071">Az.Resources</span></span>
* <span data-ttu-id="20a83-1072">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="20a83-1072">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="20a83-1073">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="20a83-1073">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="20a83-1074">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="20a83-1074">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="20a83-1075">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="20a83-1075">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-1076">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-1076">Az.Sql</span></span>
* <span data-ttu-id="20a83-1077">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="20a83-1077">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="20a83-1078">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="20a83-1078">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="20a83-1079">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="20a83-1079">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="20a83-1080">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-1080">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="20a83-1081">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-1081">Az.Accounts</span></span>
* <span data-ttu-id="20a83-1082">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="20a83-1082">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="20a83-1083">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="20a83-1083">Az.AnalysisServices</span></span>
* <span data-ttu-id="20a83-1084">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="20a83-1084">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="20a83-1085">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="20a83-1085">Az.RecoveryServices</span></span>
* <span data-ttu-id="20a83-1086">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="20a83-1086">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="20a83-1087">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-1087">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="20a83-1088">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-1088">Az.Accounts</span></span>
* <span data-ttu-id="20a83-1089">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="20a83-1089">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="20a83-1090">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="20a83-1090">Update incorrect online help URLs</span></span>
* <span data-ttu-id="20a83-1091">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="20a83-1091">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="20a83-1092">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="20a83-1092">Az.Aks</span></span>
* <span data-ttu-id="20a83-1093">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="20a83-1093">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="20a83-1094">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="20a83-1094">Az.Automation</span></span>
* <span data-ttu-id="20a83-1095">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="20a83-1095">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="20a83-1096">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="20a83-1096">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="20a83-1097">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="20a83-1097">Az.Cdn</span></span>
* <span data-ttu-id="20a83-1098">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="20a83-1098">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-1099">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-1099">Az.Compute</span></span>
* <span data-ttu-id="20a83-1100">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="20a83-1100">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="20a83-1101">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="20a83-1101">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="20a83-1102">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="20a83-1102">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="20a83-1103">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="20a83-1103">Az.ContainerRegistry</span></span>
* <span data-ttu-id="20a83-1104">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="20a83-1104">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="20a83-1105">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="20a83-1105">Az.DataFactory</span></span>
* <span data-ttu-id="20a83-1106">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="20a83-1106">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="20a83-1107">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="20a83-1107">Az.DataLakeStore</span></span>
* <span data-ttu-id="20a83-1108">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="20a83-1108">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="20a83-1109">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="20a83-1109">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="20a83-1110">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="20a83-1110">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="20a83-1111">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="20a83-1111">Az.IotHub</span></span>
* <span data-ttu-id="20a83-1112">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="20a83-1112">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="20a83-1113">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="20a83-1113">Az.KeyVault</span></span>
* <span data-ttu-id="20a83-1114">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="20a83-1114">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-1115">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-1115">Az.Network</span></span>
* <span data-ttu-id="20a83-1116">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="20a83-1116">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-1117">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-1117">Az.Resources</span></span>
* <span data-ttu-id="20a83-1118">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="20a83-1118">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="20a83-1119">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="20a83-1119">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="20a83-1120">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="20a83-1120">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="20a83-1121">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="20a83-1121">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="20a83-1122">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="20a83-1122">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="20a83-1123">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="20a83-1123">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="20a83-1124">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="20a83-1124">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="20a83-1125">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="20a83-1125">Az.ServiceFabric</span></span>
* <span data-ttu-id="20a83-1126">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="20a83-1126">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="20a83-1127">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="20a83-1127">Fix some error messages.</span></span>
* <span data-ttu-id="20a83-1128">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="20a83-1128">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="20a83-1129">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="20a83-1129">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="20a83-1130">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="20a83-1130">Az.SignalR</span></span>
* <span data-ttu-id="20a83-1131">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="20a83-1131">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-1132">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-1132">Az.Sql</span></span>
* <span data-ttu-id="20a83-1133">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="20a83-1133">Update incorrect online help URLs</span></span>
* <span data-ttu-id="20a83-1134">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="20a83-1134">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="20a83-1135">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="20a83-1135">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="20a83-1136">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="20a83-1136">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="20a83-1137">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="20a83-1137">Az.Storage</span></span>
* <span data-ttu-id="20a83-1138">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="20a83-1138">Update incorrect online help URLs</span></span>
* <span data-ttu-id="20a83-1139">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="20a83-1139">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="20a83-1140">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="20a83-1140">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="20a83-1141">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="20a83-1141">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="20a83-1142">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="20a83-1142">Az.TrafficManager</span></span>
* <span data-ttu-id="20a83-1143">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="20a83-1143">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="20a83-1144">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="20a83-1144">Az.Websites</span></span>
* <span data-ttu-id="20a83-1145">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="20a83-1145">Update incorrect online help URLs</span></span>
* <span data-ttu-id="20a83-1146">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="20a83-1146">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="20a83-1147">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="20a83-1147">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="20a83-1148">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="20a83-1148">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="20a83-1149">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-1149">Az.Accounts</span></span>
* <span data-ttu-id="20a83-1150">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="20a83-1150">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-1151">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-1151">Az.Compute</span></span>
* <span data-ttu-id="20a83-1152">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="20a83-1152">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="20a83-1153">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="20a83-1153">Updated the description of ID in help files</span></span>
* <span data-ttu-id="20a83-1154">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-1154">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="20a83-1155">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="20a83-1155">Az.DataLakeStore</span></span>
* <span data-ttu-id="20a83-1156">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="20a83-1156">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="20a83-1157">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="20a83-1157">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="20a83-1158">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="20a83-1158">Az.EventGrid</span></span>
* <span data-ttu-id="20a83-1159">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="20a83-1159">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="20a83-1160">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="20a83-1160">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="20a83-1161">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="20a83-1161">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="20a83-1162">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="20a83-1162">Event Time-To-Live,</span></span>
        - <span data-ttu-id="20a83-1163">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="20a83-1163">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="20a83-1164">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="20a83-1164">Dead letter endpoint.</span></span>
    - <span data-ttu-id="20a83-1165">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="20a83-1165">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="20a83-1166">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="20a83-1166">Event Time-To-Live,</span></span>
        - <span data-ttu-id="20a83-1167">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="20a83-1167">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="20a83-1168">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="20a83-1168">Dead letter endpoint.</span></span>
* <span data-ttu-id="20a83-1169">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="20a83-1169">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="20a83-1170">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="20a83-1170">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="20a83-1171">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="20a83-1171">Az.IotHub</span></span>
* <span data-ttu-id="20a83-1172">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="20a83-1172">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="20a83-1173">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="20a83-1173">Az.LogicApp</span></span>
* <span data-ttu-id="20a83-1174">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="20a83-1174">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-1175">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-1175">Az.Resources</span></span>
* <span data-ttu-id="20a83-1176">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="20a83-1176">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="20a83-1177">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="20a83-1177">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="20a83-1178">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="20a83-1178">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="20a83-1179">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="20a83-1179">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="20a83-1180">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="20a83-1180">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="20a83-1181">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="20a83-1181">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="20a83-1182">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="20a83-1182">Az.SignalR</span></span>
* <span data-ttu-id="20a83-1183">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-1183">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-1184">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-1184">Az.Sql</span></span>
* <span data-ttu-id="20a83-1185">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="20a83-1185">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="20a83-1186">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="20a83-1186">Az.Storage</span></span>
* <span data-ttu-id="20a83-1187">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="20a83-1187">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="20a83-1188">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="20a83-1188">New-AzStorageContext</span></span>
* <span data-ttu-id="20a83-1189">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="20a83-1189">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="20a83-1190">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="20a83-1190">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="20a83-1191">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="20a83-1191">Az.Websites</span></span>
* <span data-ttu-id="20a83-1192">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="20a83-1192">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="20a83-1193">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-1193">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="20a83-1194">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="20a83-1194">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="20a83-1195">Geral</span><span class="sxs-lookup"><span data-stu-id="20a83-1195">General</span></span>

- <span data-ttu-id="20a83-1196">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="20a83-1196">General Availability of Az Module</span></span>
- <span data-ttu-id="20a83-1197">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="20a83-1197">Online help for each module</span></span>
- <span data-ttu-id="20a83-1198">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="20a83-1198">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="20a83-1199">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="20a83-1199">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="20a83-1200">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-1200">Az.Accounts</span></span>
- <span data-ttu-id="20a83-1201">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="20a83-1201">Changed from Az.Profile</span></span>
- <span data-ttu-id="20a83-1202">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="20a83-1202">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="20a83-1203">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="20a83-1203">Az.ApiManagement</span></span>
- <span data-ttu-id="20a83-1204">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="20a83-1204">Fixes for #7002</span></span>
- <span data-ttu-id="20a83-1205">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="20a83-1205">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="20a83-1206">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="20a83-1206">Az.Batch</span></span>
- <span data-ttu-id="20a83-1207">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="20a83-1207">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="20a83-1208">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="20a83-1208">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="20a83-1209">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="20a83-1209">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="20a83-1210">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="20a83-1210">Az.Billing</span></span>
- <span data-ttu-id="20a83-1211">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="20a83-1211">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="20a83-1212">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="20a83-1212">Az.CognitivServices</span></span>
- <span data-ttu-id="20a83-1213">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="20a83-1213">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="20a83-1214">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="20a83-1214">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="20a83-1215">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="20a83-1215">Az.ContainerInstance</span></span>
- <span data-ttu-id="20a83-1216">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="20a83-1216">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="20a83-1217">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="20a83-1217">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="20a83-1218">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="20a83-1218">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="20a83-1219">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="20a83-1219">Az.DataLakeStore</span></span>
- <span data-ttu-id="20a83-1220">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="20a83-1220">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="20a83-1221">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="20a83-1221">Az.Monitor</span></span>
- <span data-ttu-id="20a83-1222">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="20a83-1222">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="20a83-1223">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="20a83-1223">Az.KeyVault</span></span>
- <span data-ttu-id="20a83-1224">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="20a83-1224">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="20a83-1225">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="20a83-1225">Az.MachineLearning</span></span>
- <span data-ttu-id="20a83-1226">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="20a83-1226">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="20a83-1227">Az.Media</span><span class="sxs-lookup"><span data-stu-id="20a83-1227">Az.Media</span></span>
- <span data-ttu-id="20a83-1228">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="20a83-1228">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="20a83-1229">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-1229">Az.Network</span></span>
<span data-ttu-id="20a83-1230">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="20a83-1230">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="20a83-1231">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="20a83-1231">New cmdlets added:</span></span>
        - <span data-ttu-id="20a83-1232">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="20a83-1232">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="20a83-1233">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="20a83-1233">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="20a83-1234">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="20a83-1234">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="20a83-1235">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="20a83-1235">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="20a83-1236">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="20a83-1236">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="20a83-1237">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="20a83-1237">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="20a83-1238">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="20a83-1238">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="20a83-1239">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="20a83-1239">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="20a83-1240">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="20a83-1240">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="20a83-1241">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="20a83-1241">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="20a83-1242">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="20a83-1242">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="20a83-1243">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="20a83-1243">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="20a83-1244">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-1244">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="20a83-1245">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-1245">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="20a83-1246">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="20a83-1246">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="20a83-1247">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="20a83-1247">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="20a83-1248">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="20a83-1248">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="20a83-1249">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="20a83-1249">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="20a83-1250">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="20a83-1250">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="20a83-1251">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="20a83-1251">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="20a83-1252">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="20a83-1252">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="20a83-1253">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="20a83-1253">Az.OperationalInsights</span></span>
- <span data-ttu-id="20a83-1254">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="20a83-1254">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="20a83-1255">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="20a83-1255">Az.Profile</span></span>
- <span data-ttu-id="20a83-1256">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="20a83-1256">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="20a83-1257">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="20a83-1257">Az.RecoveryServices</span></span>
- <span data-ttu-id="20a83-1258">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="20a83-1258">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="20a83-1259">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-1259">Az.Resources</span></span>
- <span data-ttu-id="20a83-1260">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="20a83-1260">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="20a83-1261">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="20a83-1261">Az.ServiceFabric</span></span>
- <span data-ttu-id="20a83-1262">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="20a83-1262">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="20a83-1263">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="20a83-1263">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="20a83-1264">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="20a83-1264">Az.SIgnalR</span></span>
- <span data-ttu-id="20a83-1265">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="20a83-1265">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="20a83-1266">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-1266">Az.Sql</span></span>
- <span data-ttu-id="20a83-1267">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="20a83-1267">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="20a83-1268">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="20a83-1268">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="20a83-1269">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="20a83-1269">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="20a83-1270">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="20a83-1270">Az.Storage</span></span>
- <span data-ttu-id="20a83-1271">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="20a83-1271">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="20a83-1272">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="20a83-1272">Az.Websites</span></span>
- <span data-ttu-id="20a83-1273">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="20a83-1273">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="20a83-1274">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="20a83-1274">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="20a83-1275">Geral</span><span class="sxs-lookup"><span data-stu-id="20a83-1275">General</span></span>

* <span data-ttu-id="20a83-1276">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="20a83-1276">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="20a83-1277">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-1277">Az.Compute</span></span>

* <span data-ttu-id="20a83-1278">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="20a83-1278">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="20a83-1279">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="20a83-1279">Az.DataLakeStore</span></span>

* <span data-ttu-id="20a83-1280">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="20a83-1280">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="20a83-1281">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="20a83-1281">Az.FrontDoor</span></span>

* <span data-ttu-id="20a83-1282">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="20a83-1282">Fixed some broken links</span></span>
    - <span data-ttu-id="20a83-1283">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="20a83-1283">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="20a83-1284">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="20a83-1284">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="20a83-1285">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="20a83-1285">Az.RecoveryServices</span></span>

* <span data-ttu-id="20a83-1286">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="20a83-1286">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="20a83-1287">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="20a83-1287">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="20a83-1288">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-1288">Az.Resources</span></span>

* <span data-ttu-id="20a83-1289">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="20a83-1289">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="20a83-1290">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="20a83-1290">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="20a83-1291">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-1291">Az.Sql</span></span>

* <span data-ttu-id="20a83-1292">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="20a83-1292">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="20a83-1293">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="20a83-1293">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="20a83-1294">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="20a83-1294">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="20a83-1295">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="20a83-1295">Az.Storage</span></span>

* <span data-ttu-id="20a83-1296">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="20a83-1296">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="20a83-1297">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="20a83-1297">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="20a83-1298">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="20a83-1298">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="20a83-1299">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="20a83-1299">Support Static Website configuration</span></span>
    - <span data-ttu-id="20a83-1300">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="20a83-1300">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="20a83-1301">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="20a83-1301">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="20a83-1302">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="20a83-1302">Az.Websites</span></span>

* <span data-ttu-id="20a83-1303">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="20a83-1303">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="20a83-1304">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="20a83-1304">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="20a83-1305">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="20a83-1305">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="20a83-1306">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="20a83-1306">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="20a83-1307">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="20a83-1307">Az.ApiManagement</span></span>
* <span data-ttu-id="20a83-1308">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="20a83-1308">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="20a83-1309">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="20a83-1309">Az.Automation</span></span>
* <span data-ttu-id="20a83-1310">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="20a83-1310">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="20a83-1311">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="20a83-1311">Added Update Management cmdlets</span></span>
* <span data-ttu-id="20a83-1312">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="20a83-1312">Added Source Control cmdlets</span></span>
* <span data-ttu-id="20a83-1313">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="20a83-1313">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="20a83-1314">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="20a83-1314">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="20a83-1315">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-1315">Az.Compute</span></span>
* <span data-ttu-id="20a83-1316">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="20a83-1316">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="20a83-1317">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="20a83-1317">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="20a83-1318">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="20a83-1318">Az.ContainerInstance</span></span>
* <span data-ttu-id="20a83-1319">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="20a83-1319">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="20a83-1320">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="20a83-1320">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="20a83-1321">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="20a83-1321">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="20a83-1322">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-1322">Az.Network</span></span>
* <span data-ttu-id="20a83-1323">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="20a83-1323">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="20a83-1324">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="20a83-1324">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="20a83-1325">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="20a83-1325">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="20a83-1326">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="20a83-1326">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="20a83-1327">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="20a83-1327">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="20a83-1328">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="20a83-1328">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="20a83-1329">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="20a83-1329">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="20a83-1330">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="20a83-1330">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="20a83-1331">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="20a83-1331">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="20a83-1332">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="20a83-1332">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="20a83-1333">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="20a83-1333">Az.Relay</span></span>
* <span data-ttu-id="20a83-1334">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="20a83-1334">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="20a83-1335">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-1335">Az.Resources</span></span>
* <span data-ttu-id="20a83-1336">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="20a83-1336">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="20a83-1337">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="20a83-1337">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="20a83-1338">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="20a83-1338">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="20a83-1339">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="20a83-1339">Az.ServiceFabric</span></span>
* <span data-ttu-id="20a83-1340">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="20a83-1340">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="20a83-1341">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-1341">Az.Sql</span></span>
* <span data-ttu-id="20a83-1342">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="20a83-1342">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="20a83-1343">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="20a83-1343">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="20a83-1344">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="20a83-1344">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="20a83-1345">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="20a83-1345">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="20a83-1346">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="20a83-1346">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="20a83-1347">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="20a83-1347">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="20a83-1348">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="20a83-1348">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="20a83-1349">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="20a83-1349">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="20a83-1350">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="20a83-1350">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="20a83-1351">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="20a83-1351">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="20a83-1352">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="20a83-1352">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="20a83-1353">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="20a83-1353">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="20a83-1354">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="20a83-1354">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="20a83-1355">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="20a83-1355">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="20a83-1356">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="20a83-1356">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="20a83-1357">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="20a83-1357">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="20a83-1358">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="20a83-1358">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="20a83-1359">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="20a83-1359">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="20a83-1360">Geral</span><span class="sxs-lookup"><span data-stu-id="20a83-1360">General</span></span>
* <span data-ttu-id="20a83-1361">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="20a83-1361">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="20a83-1362">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="20a83-1362">Az.Profile</span></span>
* <span data-ttu-id="20a83-1363">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="20a83-1363">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="20a83-1364">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="20a83-1364">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="20a83-1365">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="20a83-1365">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="20a83-1366">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="20a83-1366">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="20a83-1367">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="20a83-1367">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="20a83-1368">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="20a83-1368">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="20a83-1369">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="20a83-1369">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="20a83-1370">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="20a83-1370">Az.CognitiveServices</span></span>
* <span data-ttu-id="20a83-1371">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="20a83-1371">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-1372">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-1372">Az.Compute</span></span>
* <span data-ttu-id="20a83-1373">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="20a83-1373">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="20a83-1374">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="20a83-1374">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="20a83-1375">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="20a83-1375">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="20a83-1376">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="20a83-1376">Az.DataLakeStore</span></span>
* <span data-ttu-id="20a83-1377">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="20a83-1377">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="20a83-1378">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="20a83-1378">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="20a83-1379">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="20a83-1379">Az.Insights</span></span>
* <span data-ttu-id="20a83-1380">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="20a83-1380">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="20a83-1381">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="20a83-1381">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="20a83-1382">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="20a83-1382">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="20a83-1383">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="20a83-1383">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-1384">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-1384">Az.Network</span></span>
* <span data-ttu-id="20a83-1385">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="20a83-1385">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="20a83-1386">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="20a83-1386">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="20a83-1387">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="20a83-1387">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="20a83-1388">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="20a83-1388">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="20a83-1389">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="20a83-1389">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="20a83-1390">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="20a83-1390">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="20a83-1391">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="20a83-1391">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="20a83-1392">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="20a83-1392">Az.PolicyInsights</span></span>
* <span data-ttu-id="20a83-1393">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="20a83-1393">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-1394">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-1394">Az.Resources</span></span>
* <span data-ttu-id="20a83-1395">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="20a83-1395">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="20a83-1396">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="20a83-1396">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="20a83-1397">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="20a83-1397">Az.ServiceBus</span></span>
* <span data-ttu-id="20a83-1398">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="20a83-1398">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="20a83-1399">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="20a83-1399">Az.ServiceFabric</span></span>
* <span data-ttu-id="20a83-1400">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="20a83-1400">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="20a83-1401">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="20a83-1401">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="20a83-1402">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="20a83-1402">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="20a83-1403">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="20a83-1403">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="20a83-1404">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="20a83-1404">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="20a83-1405">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="20a83-1405">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="20a83-1406">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="20a83-1406">Az.Profile</span></span>
* <span data-ttu-id="20a83-1407">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="20a83-1407">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="20a83-1408">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="20a83-1408">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-1409">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-1409">Az.Compute</span></span>
* <span data-ttu-id="20a83-1410">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="20a83-1410">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="20a83-1411">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="20a83-1411">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="20a83-1412">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="20a83-1412">Az.DataLakeStore</span></span>
* <span data-ttu-id="20a83-1413">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="20a83-1413">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="20a83-1414">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="20a83-1414">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="20a83-1415">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="20a83-1415">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="20a83-1416">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="20a83-1416">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="20a83-1417">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="20a83-1417">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-1418">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-1418">Az.Network</span></span>
* <span data-ttu-id="20a83-1419">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="20a83-1419">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="20a83-1420">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="20a83-1420">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-1421">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-1421">Az.Resources</span></span>
* <span data-ttu-id="20a83-1422">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="20a83-1422">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="20a83-1423">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="20a83-1423">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="20a83-1424">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="20a83-1424">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="20a83-1425">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="20a83-1425">Azure.Storage</span></span>
* <span data-ttu-id="20a83-1426">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="20a83-1426">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="20a83-1427">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="20a83-1427">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="20a83-1428">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="20a83-1428">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="20a83-1429">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="20a83-1429">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="20a83-1430">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="20a83-1430">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="20a83-1431">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="20a83-1431">Az.CognitiveServices</span></span>
* <span data-ttu-id="20a83-1432">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="20a83-1432">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="20a83-1433">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="20a83-1433">Az.Compute</span></span>
* <span data-ttu-id="20a83-1434">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="20a83-1434">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="20a83-1435">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="20a83-1435">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="20a83-1436">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="20a83-1436">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="20a83-1437">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="20a83-1437">Az.DataFactoryV2</span></span>
* <span data-ttu-id="20a83-1438">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="20a83-1438">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="20a83-1439">Az.Network</span><span class="sxs-lookup"><span data-stu-id="20a83-1439">Az.Network</span></span>
* <span data-ttu-id="20a83-1440">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="20a83-1440">Added NetworkProfile functionality.</span></span> <span data-ttu-id="20a83-1441">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="20a83-1441">new cmdlets added</span></span>
    - <span data-ttu-id="20a83-1442">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="20a83-1442">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="20a83-1443">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="20a83-1443">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="20a83-1444">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="20a83-1444">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="20a83-1445">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="20a83-1445">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="20a83-1446">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-1446">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="20a83-1447">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-1447">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="20a83-1448">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="20a83-1448">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="20a83-1449">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="20a83-1449">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="20a83-1450">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="20a83-1450">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="20a83-1451">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="20a83-1451">Az.RedisCache</span></span>
* <span data-ttu-id="20a83-1452">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="20a83-1452">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="20a83-1453">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="20a83-1453">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="20a83-1454">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="20a83-1454">Az.Resources</span></span>
* <span data-ttu-id="20a83-1455">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="20a83-1455">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="20a83-1456">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="20a83-1456">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="20a83-1457">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="20a83-1457">Az.Sql</span></span>
* <span data-ttu-id="20a83-1458">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="20a83-1458">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="20a83-1459">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="20a83-1459">Az.Websites</span></span>
* <span data-ttu-id="20a83-1460">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="20a83-1460">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="20a83-1461">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="20a83-1461">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="20a83-1462">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="20a83-1462">0.2.0 - September 2018</span></span>
 <span data-ttu-id="20a83-1463">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="20a83-1463">Initial Release</span></span>