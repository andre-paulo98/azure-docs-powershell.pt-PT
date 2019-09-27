---
ms.openlocfilehash: 96e6d7bc0cc29adc1c0e49ba344d27349454c214
ms.sourcegitcommit: 92722d603b60dc769660e7517da60110133d9959
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/24/2019
ms.locfileid: "71226444"
---
## <a name="270---september-2019"></a><span data-ttu-id="db2d7-101">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-101">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="db2d7-102">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="db2d7-102">Az.ApiManagement</span></span>
* <span data-ttu-id="db2d7-103">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="db2d7-103">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="db2d7-104">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="db2d7-104">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="db2d7-105">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="db2d7-105">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="db2d7-106">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="db2d7-106">Az.Automation</span></span>
* <span data-ttu-id="db2d7-107">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="db2d7-107">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="db2d7-108">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="db2d7-108">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="db2d7-109">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="db2d7-109">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-110">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-110">Az.Compute</span></span>
* <span data-ttu-id="db2d7-111">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-111">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="db2d7-112">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-112">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="db2d7-113">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="db2d7-113">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="db2d7-114">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="db2d7-114">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="db2d7-115">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="db2d7-115">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="db2d7-116">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="db2d7-116">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="db2d7-117">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="db2d7-117">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="db2d7-118">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="db2d7-118">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="db2d7-119">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="db2d7-119">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="db2d7-120">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="db2d7-120">Az.DataFactory</span></span>
* <span data-ttu-id="db2d7-121">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="db2d7-121">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="db2d7-122">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="db2d7-122">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="db2d7-123">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="db2d7-123">Az.HDInsight</span></span>
* <span data-ttu-id="db2d7-124">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="db2d7-124">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="db2d7-125">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="db2d7-125">Az.IotHub</span></span>
* <span data-ttu-id="db2d7-126">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="db2d7-126">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="db2d7-127">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="db2d7-127">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="db2d7-128">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="db2d7-128">New cmdlets are:</span></span>
    - <span data-ttu-id="db2d7-129">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="db2d7-129">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="db2d7-130">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="db2d7-130">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="db2d7-131">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="db2d7-131">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="db2d7-132">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="db2d7-132">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="db2d7-133">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="db2d7-133">Az.Monitor</span></span>
* <span data-ttu-id="db2d7-134">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="db2d7-134">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="db2d7-135">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="db2d7-135">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="db2d7-136">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="db2d7-136">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="db2d7-137">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="db2d7-137">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="db2d7-138">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="db2d7-138">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="db2d7-139">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="db2d7-139">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="db2d7-140">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="db2d7-140">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="db2d7-141">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="db2d7-141">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="db2d7-142">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="db2d7-142">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="db2d7-143">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="db2d7-143">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="db2d7-144">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="db2d7-144">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="db2d7-145">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="db2d7-145">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="db2d7-146">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="db2d7-146">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="db2d7-147">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="db2d7-147">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="db2d7-148">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="db2d7-148">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="db2d7-149">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="db2d7-149">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="db2d7-150">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="db2d7-150">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="db2d7-151">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="db2d7-151">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="db2d7-152">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="db2d7-152">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="db2d7-153">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="db2d7-153">Overall improved help files</span></span>
* <span data-ttu-id="db2d7-154">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="db2d7-154">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-155">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-155">Az.Network</span></span>
* <span data-ttu-id="db2d7-156">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="db2d7-156">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="db2d7-157">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="db2d7-157">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="db2d7-158">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="db2d7-158">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="db2d7-159">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="db2d7-159">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="db2d7-160">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="db2d7-160">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="db2d7-161">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="db2d7-161">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="db2d7-162">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="db2d7-162">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="db2d7-163">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="db2d7-163">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="db2d7-164">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="db2d7-164">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="db2d7-165">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="db2d7-165">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="db2d7-166">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="db2d7-166">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="db2d7-167">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="db2d7-167">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="db2d7-168">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="db2d7-168">New cmdlets</span></span>
        - <span data-ttu-id="db2d7-169">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="db2d7-169">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="db2d7-170">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="db2d7-170">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="db2d7-171">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="db2d7-171">Updated cmdlet:</span></span>
        - <span data-ttu-id="db2d7-172">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="db2d7-172">New-VpnSite</span></span>
        - <span data-ttu-id="db2d7-173">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="db2d7-173">Update-VpnSite</span></span>
        - <span data-ttu-id="db2d7-174">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="db2d7-174">New-VpnConnection</span></span>
        - <span data-ttu-id="db2d7-175">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="db2d7-175">Update-VpnConnection</span></span>
* <span data-ttu-id="db2d7-176">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="db2d7-176">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="db2d7-177">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-177">Az.RecoveryServices</span></span>
* <span data-ttu-id="db2d7-178">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="db2d7-178">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="db2d7-179">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="db2d7-179">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-180">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-180">Az.Resources</span></span>
* <span data-ttu-id="db2d7-181">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="db2d7-181">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="db2d7-182">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="db2d7-182">Az.ServiceFabric</span></span>
* <span data-ttu-id="db2d7-183">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="db2d7-183">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="db2d7-184">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="db2d7-184">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="db2d7-185">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="db2d7-185">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="db2d7-186">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="db2d7-186">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="db2d7-187">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="db2d7-187">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="db2d7-188">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="db2d7-188">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="db2d7-189">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="db2d7-189">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="db2d7-190">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="db2d7-190">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="db2d7-191">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="db2d7-191">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="db2d7-192">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="db2d7-192">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="db2d7-193">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="db2d7-193">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="db2d7-194">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="db2d7-194">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="db2d7-195">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="db2d7-195">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="db2d7-196">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="db2d7-196">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="db2d7-197">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="db2d7-197">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="db2d7-198">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="db2d7-198">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="db2d7-199">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="db2d7-199">Az.SignalR</span></span>
* <span data-ttu-id="db2d7-200">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="db2d7-200">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-201">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-201">Az.Sql</span></span>
* <span data-ttu-id="db2d7-202">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="db2d7-202">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="db2d7-203">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="db2d7-203">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="db2d7-204">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="db2d7-204">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="db2d7-205">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="db2d7-205">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="db2d7-206">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="db2d7-206">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="db2d7-207">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="db2d7-207">Az.Storage</span></span>
* <span data-ttu-id="db2d7-208">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="db2d7-208">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="db2d7-209">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="db2d7-209">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="db2d7-210">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="db2d7-210">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="db2d7-211">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="db2d7-211">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="db2d7-212">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="db2d7-212">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="db2d7-213">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="db2d7-213">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="db2d7-214">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="db2d7-214">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="db2d7-215">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="db2d7-215">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="db2d7-216">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="db2d7-216">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="db2d7-217">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="db2d7-217">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="db2d7-218">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="db2d7-218">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="db2d7-219">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="db2d7-219">Az.Websites</span></span>
* <span data-ttu-id="db2d7-220">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="db2d7-220">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="db2d7-221">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="db2d7-221">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="db2d7-222">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="db2d7-222">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="db2d7-223">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-223">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="db2d7-224">Geral</span><span class="sxs-lookup"><span data-stu-id="db2d7-224">General</span></span>
* <span data-ttu-id="db2d7-225">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="db2d7-225">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="db2d7-226">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-226">Az.Accounts</span></span>
* <span data-ttu-id="db2d7-227">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="db2d7-227">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="db2d7-228">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="db2d7-228">Az.Aks</span></span>
* <span data-ttu-id="db2d7-229">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="db2d7-229">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="db2d7-230">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="db2d7-230">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="db2d7-231">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="db2d7-231">Az.ApiManagement</span></span>
* <span data-ttu-id="db2d7-232">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="db2d7-232">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="db2d7-233">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="db2d7-233">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="db2d7-234">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="db2d7-234">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="db2d7-235">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="db2d7-235">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="db2d7-236">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="db2d7-236">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="db2d7-237">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="db2d7-237">Az.Batch</span></span>
* <span data-ttu-id="db2d7-238">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="db2d7-238">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="db2d7-239">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="db2d7-239">Az.Cdn</span></span>
* <span data-ttu-id="db2d7-240">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="db2d7-240">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-241">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-241">Az.Compute</span></span>
* <span data-ttu-id="db2d7-242">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-242">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="db2d7-243">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="db2d7-243">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="db2d7-244">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="db2d7-244">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="db2d7-245">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="db2d7-245">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="db2d7-246">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="db2d7-246">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="db2d7-247">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="db2d7-247">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="db2d7-248">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="db2d7-248">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="db2d7-249">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="db2d7-249">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="db2d7-250">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="db2d7-250">Az.DataFactory</span></span>
* <span data-ttu-id="db2d7-251">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="db2d7-251">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="db2d7-252">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="db2d7-252">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="db2d7-253">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="db2d7-253">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="db2d7-254">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="db2d7-254">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="db2d7-255">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="db2d7-255">Az.DataLakeStore</span></span>
* <span data-ttu-id="db2d7-256">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="db2d7-256">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="db2d7-257">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="db2d7-257">Az.EventHub</span></span>
* <span data-ttu-id="db2d7-258">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="db2d7-258">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="db2d7-259">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="db2d7-259">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="db2d7-260">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="db2d7-260">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="db2d7-261">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="db2d7-261">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="db2d7-262">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="db2d7-262">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="db2d7-263">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="db2d7-263">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="db2d7-264">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="db2d7-264">Az.Monitor</span></span>
* <span data-ttu-id="db2d7-265">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="db2d7-265">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-266">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-266">Az.Network</span></span>
* <span data-ttu-id="db2d7-267">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="db2d7-267">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="db2d7-268">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="db2d7-268">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="db2d7-269">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="db2d7-269">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="db2d7-270">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="db2d7-270">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="db2d7-271">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="db2d7-271">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="db2d7-272">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="db2d7-272">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="db2d7-273">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="db2d7-273">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="db2d7-274">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="db2d7-274">Az.OperationalInsights</span></span>
* <span data-ttu-id="db2d7-275">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="db2d7-275">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="db2d7-276">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="db2d7-276">Added example</span></span>
    - <span data-ttu-id="db2d7-277">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="db2d7-277">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="db2d7-278">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="db2d7-278">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="db2d7-279">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="db2d7-279">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="db2d7-280">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-280">Az.RecoveryServices</span></span>
* <span data-ttu-id="db2d7-281">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="db2d7-281">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-282">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-282">Az.Resources</span></span>
* <span data-ttu-id="db2d7-283">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="db2d7-283">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="db2d7-284">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="db2d7-284">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="db2d7-285">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="db2d7-285">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="db2d7-286">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="db2d7-286">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="db2d7-287">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="db2d7-287">Az.ServiceBus</span></span>
* <span data-ttu-id="db2d7-288">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="db2d7-288">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="db2d7-289">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="db2d7-289">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="db2d7-290">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="db2d7-290">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="db2d7-291">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="db2d7-291">Az.ServiceFabric</span></span>
* <span data-ttu-id="db2d7-292">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="db2d7-292">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="db2d7-293">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="db2d7-293">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="db2d7-294">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="db2d7-294">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="db2d7-295">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="db2d7-295">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="db2d7-296">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="db2d7-296">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="db2d7-297">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="db2d7-297">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-298">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-298">Az.Sql</span></span>
* <span data-ttu-id="db2d7-299">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="db2d7-299">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="db2d7-300">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="db2d7-300">Az.Storage</span></span>
* <span data-ttu-id="db2d7-301">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="db2d7-301">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="db2d7-302">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="db2d7-302">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="db2d7-303">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="db2d7-303">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="db2d7-304">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="db2d7-304">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="db2d7-305">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="db2d7-305">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="db2d7-306">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="db2d7-306">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="db2d7-307">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="db2d7-307">Az.Websites</span></span>
* <span data-ttu-id="db2d7-308">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="db2d7-308">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="db2d7-309">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-309">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="db2d7-310">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-310">Az.Accounts</span></span>
* <span data-ttu-id="db2d7-311">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="db2d7-311">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="db2d7-312">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="db2d7-312">Az.ApplicationInsights</span></span>
* <span data-ttu-id="db2d7-313">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="db2d7-313">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="db2d7-314">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="db2d7-314">Az.Automation</span></span>
* <span data-ttu-id="db2d7-315">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="db2d7-315">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="db2d7-316">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-316">Az.CognitiveServices</span></span>
* <span data-ttu-id="db2d7-317">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="db2d7-317">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-318">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-318">Az.Compute</span></span>
* <span data-ttu-id="db2d7-319">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="db2d7-319">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="db2d7-320">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="db2d7-320">Az.ContainerRegistry</span></span>
* <span data-ttu-id="db2d7-321">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="db2d7-321">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="db2d7-322">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="db2d7-322">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="db2d7-323">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="db2d7-323">Az.DataFactory</span></span>
* <span data-ttu-id="db2d7-324">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="db2d7-324">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="db2d7-325">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="db2d7-325">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="db2d7-326">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="db2d7-326">Az.EventHub</span></span>
* <span data-ttu-id="db2d7-327">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="db2d7-327">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="db2d7-328">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="db2d7-328">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="db2d7-329">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="db2d7-329">Az.KeyVault</span></span>
* <span data-ttu-id="db2d7-330">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="db2d7-330">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="db2d7-331">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="db2d7-331">Az.LogicApp</span></span>
* <span data-ttu-id="db2d7-332">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="db2d7-332">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="db2d7-333">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="db2d7-333">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="db2d7-334">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-334">Az.ManagedServices</span></span>
* <span data-ttu-id="db2d7-335">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="db2d7-335">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-336">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-336">Az.Network</span></span>
* <span data-ttu-id="db2d7-337">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="db2d7-337">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="db2d7-338">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="db2d7-338">New cmdlets</span></span>
        - <span data-ttu-id="db2d7-339">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="db2d7-339">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="db2d7-340">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="db2d7-340">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="db2d7-341">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="db2d7-341">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="db2d7-342">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="db2d7-342">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="db2d7-343">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="db2d7-343">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="db2d7-344">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="db2d7-344">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="db2d7-345">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="db2d7-345">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="db2d7-346">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="db2d7-346">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="db2d7-347">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="db2d7-347">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="db2d7-348">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-348">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="db2d7-349">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="db2d7-349">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="db2d7-350">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="db2d7-350">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="db2d7-351">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="db2d7-351">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="db2d7-352">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="db2d7-352">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="db2d7-353">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="db2d7-353">Updated cmdlets</span></span>
        - <span data-ttu-id="db2d7-354">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-354">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="db2d7-355">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-355">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="db2d7-356">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-356">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="db2d7-357">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="db2d7-357">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="db2d7-358">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="db2d7-358">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="db2d7-359">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="db2d7-359">Updated cmdlet:</span></span>
        - <span data-ttu-id="db2d7-360">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-360">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="db2d7-361">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-361">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="db2d7-362">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-362">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="db2d7-363">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="db2d7-363">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="db2d7-364">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="db2d7-364">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="db2d7-365">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="db2d7-365">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="db2d7-366">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="db2d7-366">Az.OperationalInsights</span></span>
* <span data-ttu-id="db2d7-367">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="db2d7-367">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="db2d7-368">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="db2d7-368">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="db2d7-369">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-369">Az.RecoveryServices</span></span>
* <span data-ttu-id="db2d7-370">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="db2d7-370">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="db2d7-371">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="db2d7-371">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="db2d7-372">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="db2d7-372">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="db2d7-373">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="db2d7-373">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="db2d7-374">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="db2d7-374">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="db2d7-375">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="db2d7-375">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="db2d7-376">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="db2d7-376">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="db2d7-377">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="db2d7-377">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="db2d7-378">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="db2d7-378">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="db2d7-379">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="db2d7-379">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-380">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-380">Az.Resources</span></span>
- <span data-ttu-id="db2d7-381">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="db2d7-381">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="db2d7-382">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="db2d7-382">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="db2d7-383">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="db2d7-383">Az.ServiceBus</span></span>
* <span data-ttu-id="db2d7-384">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="db2d7-384">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="db2d7-385">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="db2d7-385">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-386">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-386">Az.Sql</span></span>
* <span data-ttu-id="db2d7-387">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="db2d7-387">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="db2d7-388">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="db2d7-388">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="db2d7-389">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="db2d7-389">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="db2d7-390">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="db2d7-390">Az.Storage</span></span>
* <span data-ttu-id="db2d7-391">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="db2d7-391">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="db2d7-392">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="db2d7-392">Az.StorageSync</span></span>
* <span data-ttu-id="db2d7-393">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="db2d7-393">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="db2d7-394">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="db2d7-394">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="db2d7-395">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="db2d7-395">Az.Websites</span></span>
* <span data-ttu-id="db2d7-396">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="db2d7-396">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="db2d7-397">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="db2d7-397">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="db2d7-398">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="db2d7-398">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="db2d7-399">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-399">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="db2d7-400">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-400">Az.Accounts</span></span>
* <span data-ttu-id="db2d7-401">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="db2d7-401">Add support for profile cmdlets</span></span>
* <span data-ttu-id="db2d7-402">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="db2d7-402">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="db2d7-403">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="db2d7-403">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="db2d7-404">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="db2d7-404">Az.Advisor</span></span>
* <span data-ttu-id="db2d7-405">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="db2d7-405">GA release of Az.Advisor</span></span>
* <span data-ttu-id="db2d7-406">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="db2d7-406">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="db2d7-407">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="db2d7-407">Az.ApiManagement</span></span>
* <span data-ttu-id="db2d7-408">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="db2d7-408">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="db2d7-409">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="db2d7-409">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="db2d7-410">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="db2d7-410">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="db2d7-411">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="db2d7-411">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="db2d7-412">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="db2d7-412">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="db2d7-413">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="db2d7-413">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="db2d7-414">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="db2d7-414">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="db2d7-415">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="db2d7-415">Az.Automation</span></span>
* <span data-ttu-id="db2d7-416">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="db2d7-416">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-417">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-417">Az.Compute</span></span>
* <span data-ttu-id="db2d7-418">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-418">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="db2d7-419">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="db2d7-419">Az.DataFactory</span></span>
* <span data-ttu-id="db2d7-420">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="db2d7-420">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="db2d7-421">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="db2d7-421">Az.EventGrid</span></span>
* <span data-ttu-id="db2d7-422">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="db2d7-422">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="db2d7-423">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="db2d7-423">Az.IotHub</span></span>
* <span data-ttu-id="db2d7-424">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="db2d7-424">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-425">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-425">Az.Network</span></span>
* <span data-ttu-id="db2d7-426">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="db2d7-426">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="db2d7-427">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="db2d7-427">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="db2d7-428">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="db2d7-428">Az.PolicyInsights</span></span>
* <span data-ttu-id="db2d7-429">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="db2d7-429">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="db2d7-430">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="db2d7-430">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="db2d7-431">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="db2d7-431">Az.OperationalInsights</span></span>
* <span data-ttu-id="db2d7-432">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="db2d7-432">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="db2d7-433">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-433">Az.RecoveryServices</span></span>
* <span data-ttu-id="db2d7-434">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="db2d7-434">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-435">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-435">Az.Resources</span></span>
    - <span data-ttu-id="db2d7-436">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="db2d7-436">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="db2d7-437">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="db2d7-437">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="db2d7-438">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="db2d7-438">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="db2d7-439">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="db2d7-439">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="db2d7-440">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="db2d7-440">Az.ServiceBus</span></span>
* <span data-ttu-id="db2d7-441">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="db2d7-441">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-442">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-442">Az.Sql</span></span>
* <span data-ttu-id="db2d7-443">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="db2d7-443">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="db2d7-444">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="db2d7-444">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="db2d7-445">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="db2d7-445">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="db2d7-446">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="db2d7-446">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="db2d7-447">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="db2d7-447">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="db2d7-448">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="db2d7-448">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="db2d7-449">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="db2d7-449">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="db2d7-450">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="db2d7-450">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="db2d7-451">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="db2d7-451">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="db2d7-452">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="db2d7-452">Az.Storage</span></span>
* <span data-ttu-id="db2d7-453">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="db2d7-453">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="db2d7-454">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="db2d7-454">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="db2d7-455">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="db2d7-455">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="db2d7-456">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="db2d7-456">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="db2d7-457">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="db2d7-457">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="db2d7-458">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="db2d7-458">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="db2d7-459">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="db2d7-459">Set-AzStorageAccount</span></span>
* <span data-ttu-id="db2d7-460">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="db2d7-460">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="db2d7-461">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="db2d7-461">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="db2d7-462">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="db2d7-462">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="db2d7-463">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="db2d7-463">Az.StorageSync</span></span>
* <span data-ttu-id="db2d7-464">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="db2d7-464">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="db2d7-465">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-465">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="db2d7-466">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-466">Az.Accounts</span></span>
* <span data-ttu-id="db2d7-467">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="db2d7-467">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="db2d7-468">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="db2d7-468">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="db2d7-469">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="db2d7-469">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="db2d7-470">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="db2d7-470">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="db2d7-471">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="db2d7-471">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-472">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-472">Az.Compute</span></span>
* <span data-ttu-id="db2d7-473">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="db2d7-473">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="db2d7-474">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="db2d7-474">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="db2d7-475">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="db2d7-475">Az.Dns</span></span>
* <span data-ttu-id="db2d7-476">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="db2d7-476">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="db2d7-477">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="db2d7-477">Az.EventGrid</span></span>
* <span data-ttu-id="db2d7-478">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="db2d7-478">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="db2d7-479">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="db2d7-479">New cmdlets:</span></span>
    - <span data-ttu-id="db2d7-480">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="db2d7-480">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="db2d7-481">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="db2d7-481">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="db2d7-482">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="db2d7-482">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="db2d7-483">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="db2d7-483">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="db2d7-484">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="db2d7-484">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="db2d7-485">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="db2d7-485">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="db2d7-486">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="db2d7-486">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="db2d7-487">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="db2d7-487">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="db2d7-488">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="db2d7-488">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="db2d7-489">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="db2d7-489">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="db2d7-490">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="db2d7-490">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="db2d7-491">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="db2d7-491">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="db2d7-492">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="db2d7-492">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="db2d7-493">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="db2d7-493">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="db2d7-494">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="db2d7-494">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="db2d7-495">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="db2d7-495">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="db2d7-496">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="db2d7-496">Updated cmdlets:</span></span>
    - <span data-ttu-id="db2d7-497">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="db2d7-497">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="db2d7-498">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="db2d7-498">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="db2d7-499">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="db2d7-499">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="db2d7-500">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="db2d7-500">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="db2d7-501">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="db2d7-501">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="db2d7-502">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="db2d7-502">Event subscription expiration date,</span></span>
            - <span data-ttu-id="db2d7-503">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="db2d7-503">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="db2d7-504">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="db2d7-504">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="db2d7-505">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="db2d7-505">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="db2d7-506">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="db2d7-506">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="db2d7-507">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="db2d7-507">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="db2d7-508">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="db2d7-508">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="db2d7-509">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="db2d7-509">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="db2d7-510">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="db2d7-510">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="db2d7-511">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="db2d7-511">Az.FrontDoor</span></span>
* <span data-ttu-id="db2d7-512">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="db2d7-512">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="db2d7-513">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="db2d7-513">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="db2d7-514">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="db2d7-514">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="db2d7-515">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="db2d7-515">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-516">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-516">Az.Network</span></span>
* <span data-ttu-id="db2d7-517">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="db2d7-517">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="db2d7-518">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="db2d7-518">New cmdlets</span></span>
        - <span data-ttu-id="db2d7-519">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="db2d7-519">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="db2d7-520">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="db2d7-520">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="db2d7-521">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="db2d7-521">New cmdlets</span></span> 
        - <span data-ttu-id="db2d7-522">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="db2d7-522">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="db2d7-523">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="db2d7-523">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="db2d7-524">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="db2d7-524">New cmdlets</span></span> 
        - <span data-ttu-id="db2d7-525">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="db2d7-525">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="db2d7-526">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="db2d7-526">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="db2d7-527">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="db2d7-527">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="db2d7-528">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-528">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="db2d7-529">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="db2d7-529">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="db2d7-530">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="db2d7-530">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="db2d7-531">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="db2d7-531">New cmdlets</span></span>
        - <span data-ttu-id="db2d7-532">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="db2d7-532">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="db2d7-533">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="db2d7-533">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="db2d7-534">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="db2d7-534">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="db2d7-535">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="db2d7-535">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="db2d7-536">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="db2d7-536">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="db2d7-537">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="db2d7-537">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="db2d7-538">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="db2d7-538">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="db2d7-539">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="db2d7-539">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="db2d7-540">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="db2d7-540">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="db2d7-541">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="db2d7-541">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="db2d7-542">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="db2d7-542">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="db2d7-543">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="db2d7-543">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="db2d7-544">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="db2d7-544">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="db2d7-545">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="db2d7-545">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="db2d7-546">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="db2d7-546">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="db2d7-547">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="db2d7-547">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="db2d7-548">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="db2d7-548">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="db2d7-549">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="db2d7-549">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="db2d7-550">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="db2d7-550">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="db2d7-551">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="db2d7-551">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="db2d7-552">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="db2d7-552">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="db2d7-553">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="db2d7-553">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="db2d7-554">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="db2d7-554">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="db2d7-555">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="db2d7-555">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="db2d7-556">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="db2d7-556">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="db2d7-557">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="db2d7-557">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="db2d7-558">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="db2d7-558">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="db2d7-559">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="db2d7-559">Az.OperationalInsights</span></span>
* <span data-ttu-id="db2d7-560">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="db2d7-560">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-561">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-561">Az.Resources</span></span>
* <span data-ttu-id="db2d7-562">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="db2d7-562">Support for additional Template Export options</span></span>
    - <span data-ttu-id="db2d7-563">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="db2d7-563">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="db2d7-564">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="db2d7-564">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="db2d7-565">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="db2d7-565">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="db2d7-566">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="db2d7-566">Az.ServiceFabric</span></span>
* <span data-ttu-id="db2d7-567">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="db2d7-567">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-568">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-568">Az.Sql</span></span>
* <span data-ttu-id="db2d7-569">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="db2d7-569">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="db2d7-570">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="db2d7-570">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="db2d7-571">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="db2d7-571">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="db2d7-572">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="db2d7-572">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="db2d7-573">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="db2d7-573">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="db2d7-574">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="db2d7-574">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="db2d7-575">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="db2d7-575">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="db2d7-576">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="db2d7-576">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="db2d7-577">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="db2d7-577">Az.Storage</span></span>
* <span data-ttu-id="db2d7-578">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="db2d7-578">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="db2d7-579">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="db2d7-579">New-AzStorageAccount</span></span>
* <span data-ttu-id="db2d7-580">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="db2d7-580">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="db2d7-581">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="db2d7-581">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="db2d7-582">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="db2d7-582">Az.Websites</span></span>
* <span data-ttu-id="db2d7-583">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="db2d7-583">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="db2d7-584">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="db2d7-584">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="db2d7-585">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-585">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="db2d7-586">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="db2d7-586">Az.Cdn</span></span>
* <span data-ttu-id="db2d7-587">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="db2d7-587">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-588">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-588">Az.Compute</span></span>
* <span data-ttu-id="db2d7-589">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="db2d7-589">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="db2d7-590">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="db2d7-590">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="db2d7-591">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="db2d7-591">Az.EventHub</span></span>
* <span data-ttu-id="db2d7-592">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="db2d7-592">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="db2d7-593">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="db2d7-593">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-594">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-594">Az.Network</span></span>
* <span data-ttu-id="db2d7-595">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="db2d7-595">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="db2d7-596">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="db2d7-596">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="db2d7-597">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="db2d7-597">Az.PolicyInsights</span></span>
* <span data-ttu-id="db2d7-598">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="db2d7-598">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="db2d7-599">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-599">Az.RecoveryServices</span></span>
* <span data-ttu-id="db2d7-600">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="db2d7-600">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="db2d7-601">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="db2d7-601">Az.ServiceBus</span></span>
* <span data-ttu-id="db2d7-602">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="db2d7-602">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="db2d7-603">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="db2d7-603">Az.ServiceFabric</span></span>
* <span data-ttu-id="db2d7-604">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="db2d7-604">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="db2d7-605">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="db2d7-605">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-606">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-606">Az.Sql</span></span>
* <span data-ttu-id="db2d7-607">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="db2d7-607">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="db2d7-608">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="db2d7-608">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="db2d7-609">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="db2d7-609">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="db2d7-610">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="db2d7-610">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="db2d7-611">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="db2d7-611">Az.Websites</span></span>
* <span data-ttu-id="db2d7-612">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="db2d7-612">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="db2d7-613">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-613">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="db2d7-614">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="db2d7-614">Az.ApiManagement</span></span>
* <span data-ttu-id="db2d7-615">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="db2d7-615">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="db2d7-616">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="db2d7-616">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="db2d7-617">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="db2d7-617">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="db2d7-618">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="db2d7-618">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="db2d7-619">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="db2d7-619">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="db2d7-620">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="db2d7-620">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="db2d7-621">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="db2d7-621">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="db2d7-622">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="db2d7-622">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="db2d7-623">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="db2d7-623">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="db2d7-624">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="db2d7-624">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="db2d7-625">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="db2d7-625">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="db2d7-626">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="db2d7-626">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="db2d7-627">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="db2d7-627">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="db2d7-628">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="db2d7-628">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="db2d7-629">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="db2d7-629">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="db2d7-630">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="db2d7-630">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="db2d7-631">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="db2d7-631">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="db2d7-632">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="db2d7-632">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="db2d7-633">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="db2d7-633">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="db2d7-634">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="db2d7-634">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="db2d7-635">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="db2d7-635">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="db2d7-636">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="db2d7-636">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="db2d7-637">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="db2d7-637">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="db2d7-638">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="db2d7-638">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="db2d7-639">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="db2d7-639">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="db2d7-640">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="db2d7-640">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="db2d7-641">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="db2d7-641">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="db2d7-642">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="db2d7-642">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="db2d7-643">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="db2d7-643">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="db2d7-644">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="db2d7-644">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="db2d7-645">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="db2d7-645">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="db2d7-646">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="db2d7-646">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="db2d7-647">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="db2d7-647">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="db2d7-648">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="db2d7-648">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="db2d7-649">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="db2d7-649">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="db2d7-650">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="db2d7-650">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="db2d7-651">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="db2d7-651">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="db2d7-652">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="db2d7-652">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="db2d7-653">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="db2d7-653">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="db2d7-654">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="db2d7-654">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="db2d7-655">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="db2d7-655">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="db2d7-656">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="db2d7-656">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="db2d7-657">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="db2d7-657">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="db2d7-658">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="db2d7-658">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="db2d7-659">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="db2d7-659">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="db2d7-660">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="db2d7-660">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="db2d7-661">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="db2d7-661">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="db2d7-662">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="db2d7-662">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="db2d7-663">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="db2d7-663">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="db2d7-664">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="db2d7-664">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="db2d7-665">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="db2d7-665">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="db2d7-666">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="db2d7-666">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="db2d7-667">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="db2d7-667">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="db2d7-668">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="db2d7-668">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="db2d7-669">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="db2d7-669">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="db2d7-670">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="db2d7-670">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="db2d7-671">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="db2d7-671">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="db2d7-672">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="db2d7-672">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="db2d7-673">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="db2d7-673">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="db2d7-674">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="db2d7-674">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="db2d7-675">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="db2d7-675">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="db2d7-676">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="db2d7-676">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="db2d7-677">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="db2d7-677">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="db2d7-678">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="db2d7-678">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="db2d7-679">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="db2d7-679">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="db2d7-680">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="db2d7-680">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="db2d7-681">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="db2d7-681">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="db2d7-682">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="db2d7-682">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="db2d7-683">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="db2d7-683">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="db2d7-684">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="db2d7-684">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="db2d7-685">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="db2d7-685">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="db2d7-686">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="db2d7-686">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="db2d7-687">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="db2d7-687">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="db2d7-688">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="db2d7-688">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="db2d7-689">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="db2d7-689">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="db2d7-690">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="db2d7-690">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="db2d7-691">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="db2d7-691">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="db2d7-692">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="db2d7-692">Az.Automation</span></span>
* <span data-ttu-id="db2d7-693">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="db2d7-693">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="db2d7-694">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="db2d7-694">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="db2d7-695">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="db2d7-695">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="db2d7-696">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="db2d7-696">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="db2d7-697">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="db2d7-697">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="db2d7-698">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="db2d7-698">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="db2d7-699">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="db2d7-699">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-700">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-700">Az.Compute</span></span>
* <span data-ttu-id="db2d7-701">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="db2d7-701">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="db2d7-702">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="db2d7-702">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="db2d7-703">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="db2d7-703">Az.DataLakeStore</span></span>
* <span data-ttu-id="db2d7-704">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="db2d7-704">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="db2d7-705">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="db2d7-705">Az.Monitor</span></span>
* <span data-ttu-id="db2d7-706">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="db2d7-706">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-707">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-707">Az.Network</span></span>
* <span data-ttu-id="db2d7-708">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="db2d7-708">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="db2d7-709">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="db2d7-709">Updated cmdlet:</span></span>
        - <span data-ttu-id="db2d7-710">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="db2d7-710">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="db2d7-711">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="db2d7-711">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-712">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-712">Az.Resources</span></span>
* <span data-ttu-id="db2d7-713">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="db2d7-713">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-714">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-714">Az.Sql</span></span>
* <span data-ttu-id="db2d7-715">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="db2d7-715">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="db2d7-716">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-716">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="db2d7-717">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-717">Az.Accounts</span></span>
* <span data-ttu-id="db2d7-718">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="db2d7-718">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="db2d7-719">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-719">Az.CognitiveServices</span></span>
* <span data-ttu-id="db2d7-720">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="db2d7-720">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="db2d7-721">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="db2d7-721">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-722">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-722">Az.Compute</span></span>
* <span data-ttu-id="db2d7-723">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="db2d7-723">Proximity placement group feature.</span></span>
    - <span data-ttu-id="db2d7-724">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="db2d7-724">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="db2d7-725">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-725">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="db2d7-726">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="db2d7-726">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="db2d7-727">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="db2d7-727">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="db2d7-728">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="db2d7-728">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="db2d7-729">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="db2d7-729">Breaking changes</span></span>
    - <span data-ttu-id="db2d7-730">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="db2d7-730">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="db2d7-731">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="db2d7-731">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="db2d7-732">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="db2d7-732">Az.DeploymentManager</span></span>
* <span data-ttu-id="db2d7-733">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="db2d7-733">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="db2d7-734">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="db2d7-734">Az.Dns</span></span>
* <span data-ttu-id="db2d7-735">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="db2d7-735">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="db2d7-736">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="db2d7-736">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="db2d7-737">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="db2d7-737">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="db2d7-738">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="db2d7-738">Az.FrontDoor</span></span>
* <span data-ttu-id="db2d7-739">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="db2d7-739">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="db2d7-740">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="db2d7-740">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="db2d7-741">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="db2d7-741">Az.HDInsight</span></span>
* <span data-ttu-id="db2d7-742">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="db2d7-742">Removed two cmdlets:</span></span>
    - <span data-ttu-id="db2d7-743">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="db2d7-743">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="db2d7-744">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="db2d7-744">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="db2d7-745">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="db2d7-745">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="db2d7-746">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="db2d7-746">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="db2d7-747">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="db2d7-747">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="db2d7-748">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="db2d7-748">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="db2d7-749">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="db2d7-749">Az.Monitor</span></span>
* <span data-ttu-id="db2d7-750">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="db2d7-750">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="db2d7-751">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="db2d7-751">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="db2d7-752">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="db2d7-752">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="db2d7-753">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="db2d7-753">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="db2d7-754">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="db2d7-754">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="db2d7-755">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="db2d7-755">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="db2d7-756">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="db2d7-756">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="db2d7-757">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="db2d7-757">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="db2d7-758">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="db2d7-758">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="db2d7-759">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="db2d7-759">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="db2d7-760">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="db2d7-760">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="db2d7-761">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="db2d7-761">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="db2d7-762">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="db2d7-762">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="db2d7-763">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="db2d7-763">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-764">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-764">Az.Network</span></span>
* <span data-ttu-id="db2d7-765">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="db2d7-765">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="db2d7-766">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="db2d7-766">New cmdlets</span></span>
        - <span data-ttu-id="db2d7-767">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="db2d7-767">New-AzNatGateway</span></span>
        - <span data-ttu-id="db2d7-768">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="db2d7-768">Get-AzNatGateway</span></span>
        - <span data-ttu-id="db2d7-769">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="db2d7-769">Set-AzNatGateway</span></span>
        - <span data-ttu-id="db2d7-770">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="db2d7-770">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="db2d7-771">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="db2d7-771">Updated cmdlets</span></span>
        - <span data-ttu-id="db2d7-772">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="db2d7-772">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="db2d7-773">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="db2d7-773">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="db2d7-774">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="db2d7-774">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="db2d7-775">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="db2d7-775">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="db2d7-776">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="db2d7-776">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="db2d7-777">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="db2d7-777">Az.PolicyInsights</span></span>
* <span data-ttu-id="db2d7-778">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="db2d7-778">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="db2d7-779">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="db2d7-779">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="db2d7-780">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="db2d7-780">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="db2d7-781">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-781">Az.RecoveryServices</span></span>
* <span data-ttu-id="db2d7-782">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="db2d7-782">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="db2d7-783">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="db2d7-783">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="db2d7-784">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="db2d7-784">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="db2d7-785">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="db2d7-785">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="db2d7-786">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="db2d7-786">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="db2d7-787">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="db2d7-787">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="db2d7-788">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="db2d7-788">Az.Relay</span></span>
* <span data-ttu-id="db2d7-789">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="db2d7-789">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="db2d7-790">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="db2d7-790">Az.ServiceBus</span></span>
* <span data-ttu-id="db2d7-791">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="db2d7-791">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="db2d7-792">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="db2d7-792">Az.Storage</span></span>
* <span data-ttu-id="db2d7-793">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="db2d7-793">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="db2d7-794">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="db2d7-794">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="db2d7-795">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="db2d7-795">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="db2d7-796">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="db2d7-796">New-AzStorageAccount</span></span>
* <span data-ttu-id="db2d7-797">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="db2d7-797">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="db2d7-798">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="db2d7-798">New-AzStorageAccount</span></span>
    - <span data-ttu-id="db2d7-799">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="db2d7-799">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="db2d7-800">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="db2d7-800">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="db2d7-801">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="db2d7-801">Az.Websites</span></span>
* <span data-ttu-id="db2d7-802">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="db2d7-802">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="db2d7-803">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="db2d7-803">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="db2d7-804">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-804">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="db2d7-805">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="db2d7-805">Highlights since the last major release</span></span>
* <span data-ttu-id="db2d7-806">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="db2d7-806">General availability of `Az` module</span></span>
* <span data-ttu-id="db2d7-807">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="db2d7-807">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="db2d7-808">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="db2d7-808">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="db2d7-809">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-809">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="db2d7-810">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="db2d7-810">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="db2d7-811">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="db2d7-811">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="db2d7-812">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="db2d7-812">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="db2d7-813">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-813">Az.Accounts</span></span>
* <span data-ttu-id="db2d7-814">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="db2d7-814">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="db2d7-815">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="db2d7-815">Az.Batch</span></span>
* <span data-ttu-id="db2d7-816">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-816">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="db2d7-817">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="db2d7-817">Az.Cdn</span></span>
* <span data-ttu-id="db2d7-818">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-818">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="db2d7-819">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-819">Az.CognitiveServices</span></span>
* <span data-ttu-id="db2d7-820">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-820">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-821">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-821">Az.Compute</span></span>
* <span data-ttu-id="db2d7-822">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="db2d7-822">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="db2d7-823">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-823">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="db2d7-824">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="db2d7-824">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="db2d7-825">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="db2d7-825">Az.DataFactory</span></span>
* <span data-ttu-id="db2d7-826">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="db2d7-826">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="db2d7-827">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="db2d7-827">Az.DataLakeStore</span></span>
* <span data-ttu-id="db2d7-828">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-828">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="db2d7-829">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="db2d7-829">Az.EventGrid</span></span>
* <span data-ttu-id="db2d7-830">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="db2d7-830">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="db2d7-831">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="db2d7-831">Az.EventHub</span></span>
* <span data-ttu-id="db2d7-832">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="db2d7-832">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="db2d7-833">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="db2d7-833">Az.HDInsight</span></span>
* <span data-ttu-id="db2d7-834">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-834">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="db2d7-835">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="db2d7-835">Az.IotHub</span></span>
* <span data-ttu-id="db2d7-836">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-836">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="db2d7-837">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="db2d7-837">Az.KeyVault</span></span>
* <span data-ttu-id="db2d7-838">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-838">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="db2d7-839">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="db2d7-839">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="db2d7-840">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="db2d7-840">Az.MachineLearning</span></span>
* <span data-ttu-id="db2d7-841">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-841">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="db2d7-842">Az.Media</span><span class="sxs-lookup"><span data-stu-id="db2d7-842">Az.Media</span></span>
* <span data-ttu-id="db2d7-843">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-843">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="db2d7-844">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="db2d7-844">Az.Monitor</span></span>
  * <span data-ttu-id="db2d7-845">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="db2d7-845">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="db2d7-846">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="db2d7-846">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="db2d7-847">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="db2d7-847">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="db2d7-848">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="db2d7-848">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="db2d7-849">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="db2d7-849">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="db2d7-850">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="db2d7-850">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="db2d7-851">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="db2d7-851">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-852">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-852">Az.Network</span></span>
* <span data-ttu-id="db2d7-853">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-853">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="db2d7-854">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="db2d7-854">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="db2d7-855">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="db2d7-855">Az.NotificationHubs</span></span>
* <span data-ttu-id="db2d7-856">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-856">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="db2d7-857">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="db2d7-857">Az.OperationalInsights</span></span>
* <span data-ttu-id="db2d7-858">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-858">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="db2d7-859">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="db2d7-859">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="db2d7-860">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-860">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="db2d7-861">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-861">Az.RecoveryServices</span></span>
* <span data-ttu-id="db2d7-862">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-862">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="db2d7-863">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="db2d7-863">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="db2d7-864">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="db2d7-864">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="db2d7-865">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="db2d7-865">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="db2d7-866">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="db2d7-866">Az.RedisCache</span></span>
* <span data-ttu-id="db2d7-867">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-867">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-868">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-868">Az.Resources</span></span>
* <span data-ttu-id="db2d7-869">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="db2d7-869">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-870">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-870">Az.Sql</span></span>
* <span data-ttu-id="db2d7-871">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="db2d7-871">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="db2d7-872">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-872">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="db2d7-873">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="db2d7-873">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="db2d7-874">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="db2d7-874">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="db2d7-875">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="db2d7-875">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="db2d7-876">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="db2d7-876">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="db2d7-877">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="db2d7-877">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="db2d7-878">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="db2d7-878">Az.Websites</span></span>
* <span data-ttu-id="db2d7-879">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="db2d7-879">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="db2d7-880">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="db2d7-880">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="db2d7-881">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="db2d7-881">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="db2d7-882">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="db2d7-882">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="db2d7-883">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-883">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="db2d7-884">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="db2d7-884">Highlights since the last major release</span></span>
* <span data-ttu-id="db2d7-885">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="db2d7-885">General availability of `Az` module</span></span>
* <span data-ttu-id="db2d7-886">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="db2d7-886">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="db2d7-887">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="db2d7-887">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="db2d7-888">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-888">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="db2d7-889">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="db2d7-889">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="db2d7-890">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="db2d7-890">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="db2d7-891">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="db2d7-891">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="db2d7-892">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-892">Az.Accounts</span></span>
* <span data-ttu-id="db2d7-893">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="db2d7-893">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="db2d7-894">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-894">Az.AnalysisServices</span></span>
* <span data-ttu-id="db2d7-895">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="db2d7-895">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="db2d7-896">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="db2d7-896">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="db2d7-897">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="db2d7-897">Az.Automation</span></span>
* <span data-ttu-id="db2d7-898">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="db2d7-898">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="db2d7-899">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="db2d7-899">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="db2d7-900">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="db2d7-900">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-901">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-901">Az.Compute</span></span>
* <span data-ttu-id="db2d7-902">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-902">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="db2d7-903">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="db2d7-903">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="db2d7-904">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="db2d7-904">Az.ContainerInstance</span></span>
* <span data-ttu-id="db2d7-905">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="db2d7-905">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="db2d7-906">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="db2d7-906">Az.DataFactory</span></span>
* <span data-ttu-id="db2d7-907">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="db2d7-907">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="db2d7-908">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="db2d7-908">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-909">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-909">Az.Resources</span></span>
* <span data-ttu-id="db2d7-910">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="db2d7-910">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="db2d7-911">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="db2d7-911">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="db2d7-912">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="db2d7-912">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="db2d7-913">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="db2d7-913">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="db2d7-914">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="db2d7-914">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="db2d7-915">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="db2d7-915">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-916">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-916">Az.Sql</span></span>
* <span data-ttu-id="db2d7-917">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="db2d7-917">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="db2d7-918">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="db2d7-918">Az.Storage</span></span>
* <span data-ttu-id="db2d7-919">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="db2d7-919">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="db2d7-920">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="db2d7-920">New-AzStorageContext</span></span>
* <span data-ttu-id="db2d7-921">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="db2d7-921">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="db2d7-922">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="db2d7-922">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="db2d7-923">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="db2d7-923">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="db2d7-924">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="db2d7-924">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="db2d7-925">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="db2d7-925">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="db2d7-926">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="db2d7-926">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="db2d7-927">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="db2d7-927">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="db2d7-928">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="db2d7-928">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="db2d7-929">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="db2d7-929">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="db2d7-930">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="db2d7-930">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="db2d7-931">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-931">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="db2d7-932">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="db2d7-932">Highlights since the last major release</span></span>
* <span data-ttu-id="db2d7-933">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="db2d7-933">General availability of `Az` module</span></span>
* <span data-ttu-id="db2d7-934">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="db2d7-934">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="db2d7-935">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="db2d7-935">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="db2d7-936">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-936">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="db2d7-937">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="db2d7-937">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="db2d7-938">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="db2d7-938">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="db2d7-939">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="db2d7-939">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="db2d7-940">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="db2d7-940">Az.Automation</span></span>
* <span data-ttu-id="db2d7-941">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="db2d7-941">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="db2d7-942">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="db2d7-942">Dynamic grouping</span></span>
    * <span data-ttu-id="db2d7-943">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="db2d7-943">Pre-Post script</span></span>
    * <span data-ttu-id="db2d7-944">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="db2d7-944">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-945">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-945">Az.Compute</span></span>
* <span data-ttu-id="db2d7-946">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="db2d7-946">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="db2d7-947">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="db2d7-947">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="db2d7-948">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="db2d7-948">Az.KeyVault</span></span>
* <span data-ttu-id="db2d7-949">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="db2d7-949">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-950">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-950">Az.Network</span></span>
* <span data-ttu-id="db2d7-951">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="db2d7-951">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="db2d7-952">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="db2d7-952">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="db2d7-953">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-953">Az.RecoveryServices</span></span>
* <span data-ttu-id="db2d7-954">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="db2d7-954">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="db2d7-955">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="db2d7-955">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-956">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-956">Az.Resources</span></span>
* <span data-ttu-id="db2d7-957">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="db2d7-957">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="db2d7-958">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="db2d7-958">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-959">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-959">Az.Sql</span></span>
* <span data-ttu-id="db2d7-960">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="db2d7-960">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="db2d7-961">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="db2d7-961">Az.Storage</span></span>
* <span data-ttu-id="db2d7-962">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="db2d7-962">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="db2d7-963">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="db2d7-963">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="db2d7-964">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="db2d7-964">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="db2d7-965">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="db2d7-965">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="db2d7-966">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="db2d7-966">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="db2d7-967">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="db2d7-967">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="db2d7-968">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="db2d7-968">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="db2d7-969">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="db2d7-969">Az.Websites</span></span>
* <span data-ttu-id="db2d7-970">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="db2d7-970">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="db2d7-971">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-971">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="db2d7-972">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-972">Az.Accounts</span></span>
* <span data-ttu-id="db2d7-973">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="db2d7-973">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="db2d7-974">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="db2d7-974">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="db2d7-975">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="db2d7-975">Az.Automation</span></span>
* <span data-ttu-id="db2d7-976">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="db2d7-976">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="db2d7-977">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="db2d7-977">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="db2d7-978">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="db2d7-978">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="db2d7-979">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="db2d7-979">Az.Cdn</span></span>
* <span data-ttu-id="db2d7-980">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="db2d7-980">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-981">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-981">Az.Compute</span></span>
* <span data-ttu-id="db2d7-982">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="db2d7-982">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="db2d7-983">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="db2d7-983">Az.DataFactory</span></span>
* <span data-ttu-id="db2d7-984">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="db2d7-984">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="db2d7-985">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="db2d7-985">Az.LogicApp</span></span>
* <span data-ttu-id="db2d7-986">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="db2d7-986">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-987">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-987">Az.Network</span></span>
* <span data-ttu-id="db2d7-988">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-988">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="db2d7-989">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-989">Az.RecoveryServices</span></span>
* <span data-ttu-id="db2d7-990">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="db2d7-990">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="db2d7-991">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="db2d7-991">SDK Update</span></span>
* <span data-ttu-id="db2d7-992">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="db2d7-992">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="db2d7-993">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="db2d7-993">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-994">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-994">Az.Resources</span></span>
* <span data-ttu-id="db2d7-995">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="db2d7-995">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="db2d7-996">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="db2d7-996">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="db2d7-997">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="db2d7-997">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="db2d7-998">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="db2d7-998">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="db2d7-999">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="db2d7-999">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="db2d7-1000">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="db2d7-1000">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-1001">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-1001">Az.Sql</span></span>
* <span data-ttu-id="db2d7-1002">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1002">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="db2d7-1003">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1003">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="db2d7-1004">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="db2d7-1004">Az.Storage</span></span>
* <span data-ttu-id="db2d7-1005">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="db2d7-1005">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="db2d7-1006">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-1006">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="db2d7-1007">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-1007">Az.AnalysisServices</span></span>
* <span data-ttu-id="db2d7-1008">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="db2d7-1008">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="db2d7-1009">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="db2d7-1009">Az.Automation</span></span>
* <span data-ttu-id="db2d7-1010">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="db2d7-1010">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="db2d7-1011">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="db2d7-1011">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="db2d7-1012">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="db2d7-1012">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="db2d7-1013">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-1013">Az.CognitiveServices</span></span>
* <span data-ttu-id="db2d7-1014">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1014">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-1015">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-1015">Az.Compute</span></span>
* <span data-ttu-id="db2d7-1016">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="db2d7-1016">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="db2d7-1017">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="db2d7-1017">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="db2d7-1018">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="db2d7-1018">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="db2d7-1019">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1019">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="db2d7-1020">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="db2d7-1020">Az.DataLakeStore</span></span>
* <span data-ttu-id="db2d7-1021">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="db2d7-1021">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="db2d7-1022">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="db2d7-1022">Az.EventHub</span></span>
* <span data-ttu-id="db2d7-1023">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="db2d7-1023">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="db2d7-1024">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="db2d7-1024">Az.KeyVault</span></span>
* <span data-ttu-id="db2d7-1025">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="db2d7-1025">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="db2d7-1026">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="db2d7-1026">Az.LogicApp</span></span>
* <span data-ttu-id="db2d7-1027">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="db2d7-1027">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="db2d7-1028">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1028">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="db2d7-1029">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="db2d7-1029">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="db2d7-1030">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="db2d7-1030">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="db2d7-1031">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="db2d7-1031">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="db2d7-1032">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="db2d7-1032">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="db2d7-1033">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="db2d7-1033">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="db2d7-1034">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="db2d7-1034">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="db2d7-1035">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="db2d7-1035">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="db2d7-1036">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="db2d7-1036">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="db2d7-1037">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="db2d7-1037">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="db2d7-1038">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="db2d7-1038">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="db2d7-1039">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="db2d7-1039">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="db2d7-1040">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="db2d7-1040">Az.Monitor</span></span>
* <span data-ttu-id="db2d7-1041">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="db2d7-1041">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-1042">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-1042">Az.Network</span></span>
* <span data-ttu-id="db2d7-1043">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="db2d7-1043">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="db2d7-1044">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="db2d7-1044">Az.OperationalInsights</span></span>
* <span data-ttu-id="db2d7-1045">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1045">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="db2d7-1046">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1046">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="db2d7-1047">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1047">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="db2d7-1048">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-1048">Az.Resources</span></span>
* <span data-ttu-id="db2d7-1049">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="db2d7-1049">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="db2d7-1050">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="db2d7-1050">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="db2d7-1051">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="db2d7-1051">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="db2d7-1052">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="db2d7-1052">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-1053">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-1053">Az.Sql</span></span>
* <span data-ttu-id="db2d7-1054">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="db2d7-1054">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="db2d7-1055">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="db2d7-1055">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="db2d7-1056">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="db2d7-1056">Az.Websites</span></span>
* <span data-ttu-id="db2d7-1057">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="db2d7-1057">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="db2d7-1058">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-1058">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="db2d7-1059">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-1059">Az.Accounts</span></span>
* <span data-ttu-id="db2d7-1060">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="db2d7-1060">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="db2d7-1061">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-1061">Az.AnalysisServices</span></span>
<span data-ttu-id="db2d7-1062">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1062">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-1063">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-1063">Az.Compute</span></span>
* <span data-ttu-id="db2d7-1064">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="db2d7-1064">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="db2d7-1065">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="db2d7-1065">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="db2d7-1066">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="db2d7-1066">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="db2d7-1067">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-1067">Az.RecoveryServices</span></span>
<span data-ttu-id="db2d7-1068">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1068">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-1069">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-1069">Az.Resources</span></span>
* <span data-ttu-id="db2d7-1070">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="db2d7-1070">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="db2d7-1071">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="db2d7-1071">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="db2d7-1072">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="db2d7-1072">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="db2d7-1073">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="db2d7-1073">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-1074">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-1074">Az.Sql</span></span>
* <span data-ttu-id="db2d7-1075">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="db2d7-1075">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="db2d7-1076">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="db2d7-1076">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="db2d7-1077">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="db2d7-1077">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="db2d7-1078">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-1078">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="db2d7-1079">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-1079">Az.Accounts</span></span>
* <span data-ttu-id="db2d7-1080">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="db2d7-1080">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="db2d7-1081">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-1081">Az.AnalysisServices</span></span>
* <span data-ttu-id="db2d7-1082">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="db2d7-1082">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="db2d7-1083">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-1083">Az.RecoveryServices</span></span>
* <span data-ttu-id="db2d7-1084">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="db2d7-1084">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="db2d7-1085">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-1085">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="db2d7-1086">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-1086">Az.Accounts</span></span>
* <span data-ttu-id="db2d7-1087">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="db2d7-1087">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="db2d7-1088">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1088">Update incorrect online help URLs</span></span>
* <span data-ttu-id="db2d7-1089">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="db2d7-1089">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="db2d7-1090">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="db2d7-1090">Az.Aks</span></span>
* <span data-ttu-id="db2d7-1091">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1091">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="db2d7-1092">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="db2d7-1092">Az.Automation</span></span>
* <span data-ttu-id="db2d7-1093">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="db2d7-1093">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="db2d7-1094">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1094">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="db2d7-1095">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="db2d7-1095">Az.Cdn</span></span>
* <span data-ttu-id="db2d7-1096">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1096">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-1097">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-1097">Az.Compute</span></span>
* <span data-ttu-id="db2d7-1098">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="db2d7-1098">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="db2d7-1099">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="db2d7-1099">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="db2d7-1100">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="db2d7-1100">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="db2d7-1101">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="db2d7-1101">Az.ContainerRegistry</span></span>
* <span data-ttu-id="db2d7-1102">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1102">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="db2d7-1103">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="db2d7-1103">Az.DataFactory</span></span>
* <span data-ttu-id="db2d7-1104">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="db2d7-1104">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="db2d7-1105">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="db2d7-1105">Az.DataLakeStore</span></span>
* <span data-ttu-id="db2d7-1106">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="db2d7-1106">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="db2d7-1107">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="db2d7-1107">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="db2d7-1108">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1108">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="db2d7-1109">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="db2d7-1109">Az.IotHub</span></span>
* <span data-ttu-id="db2d7-1110">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1110">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="db2d7-1111">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="db2d7-1111">Az.KeyVault</span></span>
* <span data-ttu-id="db2d7-1112">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1112">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-1113">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-1113">Az.Network</span></span>
* <span data-ttu-id="db2d7-1114">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1114">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-1115">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-1115">Az.Resources</span></span>
* <span data-ttu-id="db2d7-1116">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="db2d7-1116">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="db2d7-1117">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1117">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="db2d7-1118">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="db2d7-1118">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="db2d7-1119">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="db2d7-1119">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="db2d7-1120">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="db2d7-1120">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="db2d7-1121">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="db2d7-1121">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="db2d7-1122">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="db2d7-1122">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="db2d7-1123">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="db2d7-1123">Az.ServiceFabric</span></span>
* <span data-ttu-id="db2d7-1124">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="db2d7-1124">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="db2d7-1125">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1125">Fix some error messages.</span></span>
* <span data-ttu-id="db2d7-1126">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1126">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="db2d7-1127">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1127">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="db2d7-1128">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="db2d7-1128">Az.SignalR</span></span>
* <span data-ttu-id="db2d7-1129">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1129">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-1130">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-1130">Az.Sql</span></span>
* <span data-ttu-id="db2d7-1131">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1131">Update incorrect online help URLs</span></span>
* <span data-ttu-id="db2d7-1132">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="db2d7-1132">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="db2d7-1133">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="db2d7-1133">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="db2d7-1134">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="db2d7-1134">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="db2d7-1135">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="db2d7-1135">Az.Storage</span></span>
* <span data-ttu-id="db2d7-1136">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1136">Update incorrect online help URLs</span></span>
* <span data-ttu-id="db2d7-1137">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1137">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="db2d7-1138">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="db2d7-1138">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="db2d7-1139">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="db2d7-1139">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="db2d7-1140">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="db2d7-1140">Az.TrafficManager</span></span>
* <span data-ttu-id="db2d7-1141">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1141">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="db2d7-1142">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="db2d7-1142">Az.Websites</span></span>
* <span data-ttu-id="db2d7-1143">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1143">Update incorrect online help URLs</span></span>
* <span data-ttu-id="db2d7-1144">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1144">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="db2d7-1145">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="db2d7-1145">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="db2d7-1146">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="db2d7-1146">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="db2d7-1147">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-1147">Az.Accounts</span></span>
* <span data-ttu-id="db2d7-1148">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="db2d7-1148">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-1149">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-1149">Az.Compute</span></span>
* <span data-ttu-id="db2d7-1150">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="db2d7-1150">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="db2d7-1151">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="db2d7-1151">Updated the description of ID in help files</span></span>
* <span data-ttu-id="db2d7-1152">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-1152">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="db2d7-1153">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="db2d7-1153">Az.DataLakeStore</span></span>
* <span data-ttu-id="db2d7-1154">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1154">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="db2d7-1155">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="db2d7-1155">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="db2d7-1156">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="db2d7-1156">Az.EventGrid</span></span>
* <span data-ttu-id="db2d7-1157">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1157">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="db2d7-1158">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="db2d7-1158">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="db2d7-1159">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="db2d7-1159">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="db2d7-1160">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="db2d7-1160">Event Time-To-Live,</span></span>
        - <span data-ttu-id="db2d7-1161">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="db2d7-1161">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="db2d7-1162">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1162">Dead letter endpoint.</span></span>
    - <span data-ttu-id="db2d7-1163">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="db2d7-1163">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="db2d7-1164">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="db2d7-1164">Event Time-To-Live,</span></span>
        - <span data-ttu-id="db2d7-1165">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="db2d7-1165">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="db2d7-1166">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1166">Dead letter endpoint.</span></span>
* <span data-ttu-id="db2d7-1167">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1167">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="db2d7-1168">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1168">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="db2d7-1169">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="db2d7-1169">Az.IotHub</span></span>
* <span data-ttu-id="db2d7-1170">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="db2d7-1170">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="db2d7-1171">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="db2d7-1171">Az.LogicApp</span></span>
* <span data-ttu-id="db2d7-1172">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="db2d7-1172">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-1173">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-1173">Az.Resources</span></span>
* <span data-ttu-id="db2d7-1174">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="db2d7-1174">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="db2d7-1175">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="db2d7-1175">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="db2d7-1176">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="db2d7-1176">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="db2d7-1177">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="db2d7-1177">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="db2d7-1178">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="db2d7-1178">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="db2d7-1179">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="db2d7-1179">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="db2d7-1180">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="db2d7-1180">Az.SignalR</span></span>
* <span data-ttu-id="db2d7-1181">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-1181">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-1182">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-1182">Az.Sql</span></span>
* <span data-ttu-id="db2d7-1183">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1183">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="db2d7-1184">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="db2d7-1184">Az.Storage</span></span>
* <span data-ttu-id="db2d7-1185">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="db2d7-1185">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="db2d7-1186">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="db2d7-1186">New-AzStorageContext</span></span>
* <span data-ttu-id="db2d7-1187">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="db2d7-1187">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="db2d7-1188">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="db2d7-1188">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="db2d7-1189">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="db2d7-1189">Az.Websites</span></span>
* <span data-ttu-id="db2d7-1190">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="db2d7-1190">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="db2d7-1191">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-1191">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="db2d7-1192">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="db2d7-1192">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="db2d7-1193">Geral</span><span class="sxs-lookup"><span data-stu-id="db2d7-1193">General</span></span>

- <span data-ttu-id="db2d7-1194">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="db2d7-1194">General Availability of Az Module</span></span>
- <span data-ttu-id="db2d7-1195">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="db2d7-1195">Online help for each module</span></span>
- <span data-ttu-id="db2d7-1196">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="db2d7-1196">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="db2d7-1197">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="db2d7-1197">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="db2d7-1198">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-1198">Az.Accounts</span></span>
- <span data-ttu-id="db2d7-1199">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="db2d7-1199">Changed from Az.Profile</span></span>
- <span data-ttu-id="db2d7-1200">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="db2d7-1200">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="db2d7-1201">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="db2d7-1201">Az.ApiManagement</span></span>
- <span data-ttu-id="db2d7-1202">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="db2d7-1202">Fixes for #7002</span></span>
- <span data-ttu-id="db2d7-1203">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="db2d7-1203">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="db2d7-1204">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="db2d7-1204">Az.Batch</span></span>
- <span data-ttu-id="db2d7-1205">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1205">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="db2d7-1206">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1206">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="db2d7-1207">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="db2d7-1207">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="db2d7-1208">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="db2d7-1208">Az.Billing</span></span>
- <span data-ttu-id="db2d7-1209">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="db2d7-1209">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="db2d7-1210">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-1210">Az.CognitivServices</span></span>
- <span data-ttu-id="db2d7-1211">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="db2d7-1211">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="db2d7-1212">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="db2d7-1212">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="db2d7-1213">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="db2d7-1213">Az.ContainerInstance</span></span>
- <span data-ttu-id="db2d7-1214">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="db2d7-1214">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="db2d7-1215">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="db2d7-1215">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="db2d7-1216">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="db2d7-1216">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="db2d7-1217">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="db2d7-1217">Az.DataLakeStore</span></span>
- <span data-ttu-id="db2d7-1218">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="db2d7-1218">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="db2d7-1219">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="db2d7-1219">Az.Monitor</span></span>
- <span data-ttu-id="db2d7-1220">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="db2d7-1220">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="db2d7-1221">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="db2d7-1221">Az.KeyVault</span></span>
- <span data-ttu-id="db2d7-1222">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="db2d7-1222">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="db2d7-1223">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="db2d7-1223">Az.MachineLearning</span></span>
- <span data-ttu-id="db2d7-1224">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="db2d7-1224">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="db2d7-1225">Az.Media</span><span class="sxs-lookup"><span data-stu-id="db2d7-1225">Az.Media</span></span>
- <span data-ttu-id="db2d7-1226">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="db2d7-1226">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="db2d7-1227">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-1227">Az.Network</span></span>
<span data-ttu-id="db2d7-1228">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="db2d7-1228">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="db2d7-1229">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="db2d7-1229">New cmdlets added:</span></span>
        - <span data-ttu-id="db2d7-1230">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="db2d7-1230">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="db2d7-1231">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="db2d7-1231">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="db2d7-1232">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="db2d7-1232">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="db2d7-1233">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="db2d7-1233">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="db2d7-1234">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="db2d7-1234">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="db2d7-1235">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="db2d7-1235">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="db2d7-1236">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="db2d7-1236">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="db2d7-1237">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="db2d7-1237">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="db2d7-1238">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="db2d7-1238">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="db2d7-1239">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="db2d7-1239">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="db2d7-1240">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="db2d7-1240">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="db2d7-1241">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="db2d7-1241">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="db2d7-1242">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-1242">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="db2d7-1243">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-1243">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="db2d7-1244">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1244">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="db2d7-1245">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="db2d7-1245">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="db2d7-1246">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="db2d7-1246">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="db2d7-1247">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="db2d7-1247">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="db2d7-1248">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="db2d7-1248">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="db2d7-1249">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="db2d7-1249">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="db2d7-1250">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="db2d7-1250">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="db2d7-1251">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="db2d7-1251">Az.OperationalInsights</span></span>
- <span data-ttu-id="db2d7-1252">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="db2d7-1252">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="db2d7-1253">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="db2d7-1253">Az.Profile</span></span>
- <span data-ttu-id="db2d7-1254">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="db2d7-1254">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="db2d7-1255">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-1255">Az.RecoveryServices</span></span>
- <span data-ttu-id="db2d7-1256">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="db2d7-1256">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="db2d7-1257">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-1257">Az.Resources</span></span>
- <span data-ttu-id="db2d7-1258">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="db2d7-1258">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="db2d7-1259">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="db2d7-1259">Az.ServiceFabric</span></span>
- <span data-ttu-id="db2d7-1260">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="db2d7-1260">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="db2d7-1261">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="db2d7-1261">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="db2d7-1262">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="db2d7-1262">Az.SIgnalR</span></span>
- <span data-ttu-id="db2d7-1263">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="db2d7-1263">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="db2d7-1264">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-1264">Az.Sql</span></span>
- <span data-ttu-id="db2d7-1265">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="db2d7-1265">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="db2d7-1266">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="db2d7-1266">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="db2d7-1267">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="db2d7-1267">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="db2d7-1268">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="db2d7-1268">Az.Storage</span></span>
- <span data-ttu-id="db2d7-1269">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="db2d7-1269">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="db2d7-1270">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="db2d7-1270">Az.Websites</span></span>
- <span data-ttu-id="db2d7-1271">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="db2d7-1271">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="db2d7-1272">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="db2d7-1272">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="db2d7-1273">Geral</span><span class="sxs-lookup"><span data-stu-id="db2d7-1273">General</span></span>

* <span data-ttu-id="db2d7-1274">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="db2d7-1274">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="db2d7-1275">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-1275">Az.Compute</span></span>

* <span data-ttu-id="db2d7-1276">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1276">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="db2d7-1277">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="db2d7-1277">Az.DataLakeStore</span></span>

* <span data-ttu-id="db2d7-1278">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="db2d7-1278">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="db2d7-1279">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="db2d7-1279">Az.FrontDoor</span></span>

* <span data-ttu-id="db2d7-1280">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="db2d7-1280">Fixed some broken links</span></span>
    - <span data-ttu-id="db2d7-1281">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1281">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="db2d7-1282">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1282">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="db2d7-1283">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-1283">Az.RecoveryServices</span></span>

* <span data-ttu-id="db2d7-1284">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1284">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="db2d7-1285">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1285">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="db2d7-1286">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-1286">Az.Resources</span></span>

* <span data-ttu-id="db2d7-1287">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="db2d7-1287">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="db2d7-1288">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1288">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="db2d7-1289">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-1289">Az.Sql</span></span>

* <span data-ttu-id="db2d7-1290">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="db2d7-1290">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="db2d7-1291">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="db2d7-1291">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="db2d7-1292">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1292">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="db2d7-1293">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="db2d7-1293">Az.Storage</span></span>

* <span data-ttu-id="db2d7-1294">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="db2d7-1294">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="db2d7-1295">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="db2d7-1295">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="db2d7-1296">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="db2d7-1296">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="db2d7-1297">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="db2d7-1297">Support Static Website configuration</span></span>
    - <span data-ttu-id="db2d7-1298">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="db2d7-1298">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="db2d7-1299">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="db2d7-1299">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="db2d7-1300">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="db2d7-1300">Az.Websites</span></span>

* <span data-ttu-id="db2d7-1301">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="db2d7-1301">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="db2d7-1302">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1302">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="db2d7-1303">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1303">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="db2d7-1304">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="db2d7-1304">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="db2d7-1305">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="db2d7-1305">Az.ApiManagement</span></span>
* <span data-ttu-id="db2d7-1306">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1306">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="db2d7-1307">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="db2d7-1307">Az.Automation</span></span>
* <span data-ttu-id="db2d7-1308">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="db2d7-1308">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="db2d7-1309">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="db2d7-1309">Added Update Management cmdlets</span></span>
* <span data-ttu-id="db2d7-1310">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="db2d7-1310">Added Source Control cmdlets</span></span>
* <span data-ttu-id="db2d7-1311">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="db2d7-1311">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="db2d7-1312">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="db2d7-1312">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="db2d7-1313">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-1313">Az.Compute</span></span>
* <span data-ttu-id="db2d7-1314">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="db2d7-1314">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="db2d7-1315">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1315">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="db2d7-1316">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="db2d7-1316">Az.ContainerInstance</span></span>
* <span data-ttu-id="db2d7-1317">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1317">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="db2d7-1318">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="db2d7-1318">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="db2d7-1319">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="db2d7-1319">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="db2d7-1320">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-1320">Az.Network</span></span>
* <span data-ttu-id="db2d7-1321">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="db2d7-1321">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="db2d7-1322">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="db2d7-1322">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="db2d7-1323">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1323">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="db2d7-1324">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="db2d7-1324">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="db2d7-1325">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="db2d7-1325">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="db2d7-1326">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1326">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="db2d7-1327">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1327">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="db2d7-1328">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="db2d7-1328">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="db2d7-1329">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="db2d7-1329">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="db2d7-1330">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="db2d7-1330">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="db2d7-1331">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="db2d7-1331">Az.Relay</span></span>
* <span data-ttu-id="db2d7-1332">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1332">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="db2d7-1333">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-1333">Az.Resources</span></span>
* <span data-ttu-id="db2d7-1334">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="db2d7-1334">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="db2d7-1335">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="db2d7-1335">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="db2d7-1336">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="db2d7-1336">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="db2d7-1337">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="db2d7-1337">Az.ServiceFabric</span></span>
* <span data-ttu-id="db2d7-1338">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="db2d7-1338">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="db2d7-1339">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-1339">Az.Sql</span></span>
* <span data-ttu-id="db2d7-1340">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="db2d7-1340">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="db2d7-1341">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="db2d7-1341">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="db2d7-1342">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="db2d7-1342">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="db2d7-1343">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="db2d7-1343">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="db2d7-1344">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="db2d7-1344">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="db2d7-1345">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="db2d7-1345">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="db2d7-1346">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="db2d7-1346">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="db2d7-1347">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="db2d7-1347">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="db2d7-1348">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="db2d7-1348">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="db2d7-1349">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1349">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="db2d7-1350">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1350">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="db2d7-1351">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1351">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="db2d7-1352">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1352">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="db2d7-1353">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1353">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="db2d7-1354">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1354">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="db2d7-1355">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1355">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="db2d7-1356">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="db2d7-1356">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="db2d7-1357">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="db2d7-1357">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="db2d7-1358">Geral</span><span class="sxs-lookup"><span data-stu-id="db2d7-1358">General</span></span>
* <span data-ttu-id="db2d7-1359">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="db2d7-1359">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="db2d7-1360">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="db2d7-1360">Az.Profile</span></span>
* <span data-ttu-id="db2d7-1361">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="db2d7-1361">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="db2d7-1362">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="db2d7-1362">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="db2d7-1363">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="db2d7-1363">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="db2d7-1364">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="db2d7-1364">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="db2d7-1365">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="db2d7-1365">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="db2d7-1366">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="db2d7-1366">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="db2d7-1367">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="db2d7-1367">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="db2d7-1368">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-1368">Az.CognitiveServices</span></span>
* <span data-ttu-id="db2d7-1369">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1369">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-1370">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-1370">Az.Compute</span></span>
* <span data-ttu-id="db2d7-1371">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="db2d7-1371">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="db2d7-1372">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="db2d7-1372">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="db2d7-1373">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1373">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="db2d7-1374">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="db2d7-1374">Az.DataLakeStore</span></span>
* <span data-ttu-id="db2d7-1375">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1375">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="db2d7-1376">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1376">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="db2d7-1377">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="db2d7-1377">Az.Insights</span></span>
* <span data-ttu-id="db2d7-1378">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="db2d7-1378">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="db2d7-1379">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="db2d7-1379">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="db2d7-1380">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="db2d7-1380">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="db2d7-1381">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="db2d7-1381">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-1382">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-1382">Az.Network</span></span>
* <span data-ttu-id="db2d7-1383">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="db2d7-1383">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="db2d7-1384">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="db2d7-1384">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="db2d7-1385">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="db2d7-1385">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="db2d7-1386">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="db2d7-1386">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="db2d7-1387">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="db2d7-1387">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="db2d7-1388">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="db2d7-1388">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="db2d7-1389">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="db2d7-1389">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="db2d7-1390">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="db2d7-1390">Az.PolicyInsights</span></span>
* <span data-ttu-id="db2d7-1391">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="db2d7-1391">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-1392">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-1392">Az.Resources</span></span>
* <span data-ttu-id="db2d7-1393">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="db2d7-1393">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="db2d7-1394">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="db2d7-1394">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="db2d7-1395">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="db2d7-1395">Az.ServiceBus</span></span>
* <span data-ttu-id="db2d7-1396">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1396">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="db2d7-1397">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="db2d7-1397">Az.ServiceFabric</span></span>
* <span data-ttu-id="db2d7-1398">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1398">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="db2d7-1399">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="db2d7-1399">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="db2d7-1400">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="db2d7-1400">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="db2d7-1401">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="db2d7-1401">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="db2d7-1402">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1402">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="db2d7-1403">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="db2d7-1403">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="db2d7-1404">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="db2d7-1404">Az.Profile</span></span>
* <span data-ttu-id="db2d7-1405">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="db2d7-1405">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="db2d7-1406">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="db2d7-1406">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-1407">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-1407">Az.Compute</span></span>
* <span data-ttu-id="db2d7-1408">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="db2d7-1408">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="db2d7-1409">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1409">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="db2d7-1410">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="db2d7-1410">Az.DataLakeStore</span></span>
* <span data-ttu-id="db2d7-1411">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="db2d7-1411">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="db2d7-1412">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1412">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="db2d7-1413">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1413">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="db2d7-1414">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1414">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="db2d7-1415">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1415">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-1416">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-1416">Az.Network</span></span>
* <span data-ttu-id="db2d7-1417">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1417">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="db2d7-1418">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1418">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-1419">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-1419">Az.Resources</span></span>
* <span data-ttu-id="db2d7-1420">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1420">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="db2d7-1421">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="db2d7-1421">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="db2d7-1422">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="db2d7-1422">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="db2d7-1423">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="db2d7-1423">Azure.Storage</span></span>
* <span data-ttu-id="db2d7-1424">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="db2d7-1424">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="db2d7-1425">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="db2d7-1425">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="db2d7-1426">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="db2d7-1426">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="db2d7-1427">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1427">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="db2d7-1428">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="db2d7-1428">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="db2d7-1429">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="db2d7-1429">Az.CognitiveServices</span></span>
* <span data-ttu-id="db2d7-1430">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1430">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="db2d7-1431">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="db2d7-1431">Az.Compute</span></span>
* <span data-ttu-id="db2d7-1432">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="db2d7-1432">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="db2d7-1433">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1433">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="db2d7-1434">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="db2d7-1434">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="db2d7-1435">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="db2d7-1435">Az.DataFactoryV2</span></span>
* <span data-ttu-id="db2d7-1436">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1436">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="db2d7-1437">Az.Network</span><span class="sxs-lookup"><span data-stu-id="db2d7-1437">Az.Network</span></span>
* <span data-ttu-id="db2d7-1438">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1438">Added NetworkProfile functionality.</span></span> <span data-ttu-id="db2d7-1439">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="db2d7-1439">new cmdlets added</span></span>
    - <span data-ttu-id="db2d7-1440">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="db2d7-1440">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="db2d7-1441">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="db2d7-1441">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="db2d7-1442">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="db2d7-1442">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="db2d7-1443">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="db2d7-1443">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="db2d7-1444">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-1444">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="db2d7-1445">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-1445">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="db2d7-1446">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="db2d7-1446">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="db2d7-1447">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="db2d7-1447">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="db2d7-1448">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="db2d7-1448">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="db2d7-1449">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="db2d7-1449">Az.RedisCache</span></span>
* <span data-ttu-id="db2d7-1450">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="db2d7-1450">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="db2d7-1451">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="db2d7-1451">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="db2d7-1452">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="db2d7-1452">Az.Resources</span></span>
* <span data-ttu-id="db2d7-1453">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="db2d7-1453">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="db2d7-1454">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="db2d7-1454">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="db2d7-1455">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="db2d7-1455">Az.Sql</span></span>
* <span data-ttu-id="db2d7-1456">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="db2d7-1456">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="db2d7-1457">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="db2d7-1457">Az.Websites</span></span>
* <span data-ttu-id="db2d7-1458">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="db2d7-1458">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="db2d7-1459">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="db2d7-1459">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="db2d7-1460">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="db2d7-1460">0.2.0 - September 2018</span></span>
 <span data-ttu-id="db2d7-1461">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="db2d7-1461">Initial Release</span></span>