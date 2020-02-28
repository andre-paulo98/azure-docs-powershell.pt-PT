---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/09/2020
ms.openlocfilehash: 81afcd63e5ca7a776965849de9090b833f49acc7
ms.sourcegitcommit: a321ef9d134c684fa24ababcbd898f86b00d9364
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/20/2020
ms.locfileid: "77477238"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="a117f-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a117f-103">Azure PowerShell release notes</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="a117f-104">3.5.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="a117f-104">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a117f-105">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a117f-105">Highlights since the last major release</span></span>
* <span data-ttu-id="a117f-106">Telemetria do lado do cliente atualizada.</span><span class="sxs-lookup"><span data-stu-id="a117f-106">Updated client side telemetry.</span></span>
* <span data-ttu-id="a117f-107">O Az.IotHub adicionou cmdlets para suportar a gestão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a117f-107">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="a117f-108">O Az.SqlVirtualMachine adicionou cmdlets ao Serviço de Escuta do Grupo de Disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="a117f-108">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a117f-109">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-109">Az.Accounts</span></span>
* <span data-ttu-id="a117f-110">SubscriptionId, TenantId e tempo de execução adicionados aos dados de telemetria do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="a117f-110">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a117f-111">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a117f-111">Az.Automation</span></span>
* <span data-ttu-id="a117f-112">Foi corrigido o erro no Exemplo 1 na documentação de referência de "New-AzAutomationSoftwareUpdateConfiguration"</span><span class="sxs-lookup"><span data-stu-id="a117f-112">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a117f-113">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a117f-113">Az.CognitiveServices</span></span>
* <span data-ttu-id="a117f-114">SDK atualizado para a versão 7.0</span><span class="sxs-lookup"><span data-stu-id="a117f-114">Updated SDK to 7.0</span></span>
* <span data-ttu-id="a117f-115">Mensagem de erro melhorada quando o servidor responde ao corpo vazio</span><span class="sxs-lookup"><span data-stu-id="a117f-115">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-116">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-116">Az.Compute</span></span>
* <span data-ttu-id="a117f-117">Valor vazio permitido para ProximityPlacementGroupId durante a atualização</span><span class="sxs-lookup"><span data-stu-id="a117f-117">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a117f-118">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a117f-118">Az.FrontDoor</span></span>
* <span data-ttu-id="a117f-119">Cmdlet adicionado para obter definições de regras geridas que podem ser utilizadas na WAF</span><span class="sxs-lookup"><span data-stu-id="a117f-119">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a117f-120">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a117f-120">Az.IotHub</span></span>
* <span data-ttu-id="a117f-121">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="a117f-121">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="a117f-122">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="a117f-122">New Cmdlets are:</span></span>
    - <span data-ttu-id="a117f-123">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="a117f-123">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="a117f-124">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="a117f-124">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="a117f-125">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="a117f-125">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="a117f-126">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="a117f-126">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a117f-127">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a117f-127">Az.KeyVault</span></span>
* <span data-ttu-id="a117f-128">Texto duplicado fixo para Add-AzKeyVaultKey.md</span><span class="sxs-lookup"><span data-stu-id="a117f-128">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a117f-129">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a117f-129">Az.Monitor</span></span>
* <span data-ttu-id="a117f-130">Descrição fixa do cmdlet Get-AzLog.</span><span class="sxs-lookup"><span data-stu-id="a117f-130">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="a117f-131">Foi adicionado um novo parâmetro chamado ActionGroupId ao comando "New-AzMetricAlertRuleV2".</span><span class="sxs-lookup"><span data-stu-id="a117f-131">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="a117f-132">O utilizador pode fornecer ActionGroupId(string) ou ActionGorup(ActivityLogAlertActionGroup).</span><span class="sxs-lookup"><span data-stu-id="a117f-132">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-133">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-133">Az.Network</span></span>
* <span data-ttu-id="a117f-134">Foi adicionada uma nota de parâmetro adicional para o parâmetro "-EnableProxyProtocol" para o cmdlet "New-AzPrivateLinkService".</span><span class="sxs-lookup"><span data-stu-id="a117f-134">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="a117f-135">Exemplo de FilterData fixo em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="a117f-135">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="a117f-136">Exemplo de Captura de Pacotes adicionado para capturar todos os pacotes internos e externos em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="a117f-136">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="a117f-137">Política do Azure Firewall suportada em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="a117f-137">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="a117f-138">Não foram adicionados novos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="a117f-138">No new cmdlets are added.</span></span> <span data-ttu-id="a117f-139">Simplificação da restrição da política de firewall em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="a117f-139">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-140">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-140">Az.RecoveryServices</span></span>
* <span data-ttu-id="a117f-141">Suporte adicionado da funcionalidade Restaurar como ficheiros para Bases de Dados SQL.</span><span class="sxs-lookup"><span data-stu-id="a117f-141">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-142">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-142">Az.Resources</span></span>
* <span data-ttu-id="a117f-143">Cmdlets de implementação de modelos refatorizados</span><span class="sxs-lookup"><span data-stu-id="a117f-143">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="a117f-144">Foram adicionados novos cmdlets para gerir implementações no grupo de gestão: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="a117f-144">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="a117f-145">Foram adicionados novos cmdlets para gerir implementações no inquilino: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="a117f-145">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="a117f-146">Cmdlets \*-AzDeployment refatorizados para trabalhar especificamente no âmbito da subscrição</span><span class="sxs-lookup"><span data-stu-id="a117f-146">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="a117f-147">Foram criados aliases \*-AzSubscriptionDeployment para os cmdlets \*-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="a117f-147">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="a117f-148">"Update-AzADApplication" fixo quando o parâmetro "AvailableToOtherTenants" não está definido</span><span class="sxs-lookup"><span data-stu-id="a117f-148">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="a117f-149">ApplicationObjectWithoutCredentialParameterSet removido para evitar AmbiguousParameterSetException.</span><span class="sxs-lookup"><span data-stu-id="a117f-149">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="a117f-150">Ficheiros de ajuda regenerados</span><span class="sxs-lookup"><span data-stu-id="a117f-150">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-151">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-151">Az.Sql</span></span>
* <span data-ttu-id="a117f-152">Suporte adicionado para restauro para um ponto anterior no tempo entre subscrições nas Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="a117f-152">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="a117f-153">Suporte adicionado para alterar a geração de hardware das Instâncias Geridas de SQL existentes</span><span class="sxs-lookup"><span data-stu-id="a117f-153">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="a117f-154">Exemplos de ajuda "Update-AzSqlServerVulnerabilityAssessmentSetting" fixos: saída do parâmetro/propriedade - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="a117f-154">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="a117f-155">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="a117f-155">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="a117f-156">Cmdlets adicionados para o Serviço de Escuta do Grupo de Disponibilidade</span><span class="sxs-lookup"><span data-stu-id="a117f-156">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="a117f-157">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="a117f-157">Az.StorageSync</span></span>
* <span data-ttu-id="a117f-158">Conjuntos de carateres suportados atualizados em "Invoke-AzStorageSyncCompatibilityCheck".</span><span class="sxs-lookup"><span data-stu-id="a117f-158">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="a117f-159">3.4.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="a117f-159">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a117f-160">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a117f-160">Highlights since the last major release</span></span>
* <span data-ttu-id="a117f-161">Versão inicial Az.CosmosDB 0.1.0 lançada</span><span class="sxs-lookup"><span data-stu-id="a117f-161">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="a117f-162">Foi adicionado suporte para Az.Network ConnectionMonitor V2</span><span class="sxs-lookup"><span data-stu-id="a117f-162">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a117f-163">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-163">Az.Accounts</span></span>
* <span data-ttu-id="a117f-164">Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível</span><span class="sxs-lookup"><span data-stu-id="a117f-164">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="a117f-165">Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5</span><span class="sxs-lookup"><span data-stu-id="a117f-165">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="a117f-166">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a117f-166">Az.ApiManagement</span></span>
* <span data-ttu-id="a117f-167">**Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="a117f-167">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="a117f-168">**New-AzApiManagementProduct**\* e **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="a117f-168">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="a117f-169">Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472</span><span class="sxs-lookup"><span data-stu-id="a117f-169">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="a117f-170">**Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet</span><span class="sxs-lookup"><span data-stu-id="a117f-170">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-171">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-171">Az.Compute</span></span>
* <span data-ttu-id="a117f-172">Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.</span><span class="sxs-lookup"><span data-stu-id="a117f-172">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="a117f-173">Foi adicionado o cmdlet Update-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="a117f-173">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="a117f-174">Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a117f-174">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="a117f-175">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-175">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="a117f-176">Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="a117f-176">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a117f-177">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a117f-177">Az.DataFactory</span></span>
* <span data-ttu-id="a117f-178">Atualização do SDK .NET do ADF para a versão 4.7.0</span><span class="sxs-lookup"><span data-stu-id="a117f-178">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="a117f-179">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="a117f-179">Az.DeploymentManager</span></span>
* <span data-ttu-id="a117f-180">Adiciona operações LIST para os recursos</span><span class="sxs-lookup"><span data-stu-id="a117f-180">Adds LIST operations for resources</span></span>
* <span data-ttu-id="a117f-181">Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="a117f-181">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a117f-182">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a117f-182">Az.HDInsight</span></span>
* <span data-ttu-id="a117f-183">Foi corrigido o erro do documento de New-AzHDInsightCluster.</span><span class="sxs-lookup"><span data-stu-id="a117f-183">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a117f-184">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a117f-184">Az.KeyVault</span></span>
* <span data-ttu-id="a117f-185">Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.</span><span class="sxs-lookup"><span data-stu-id="a117f-185">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-186">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-186">Az.Network</span></span>
* <span data-ttu-id="a117f-187">Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="a117f-187">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="a117f-188">Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão</span><span class="sxs-lookup"><span data-stu-id="a117f-188">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="a117f-189">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="a117f-189">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="a117f-190">Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="a117f-190">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="a117f-191">Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"</span><span class="sxs-lookup"><span data-stu-id="a117f-191">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="a117f-192">Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.</span><span class="sxs-lookup"><span data-stu-id="a117f-192">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="a117f-193">Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a117f-193">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="a117f-194">Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="a117f-194">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="a117f-195">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a117f-195">New cmdlets added:</span></span>
        - <span data-ttu-id="a117f-196">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="a117f-196">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="a117f-197">Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="a117f-197">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="a117f-198">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="a117f-198">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="a117f-199">Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2</span><span class="sxs-lookup"><span data-stu-id="a117f-199">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a117f-200">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a117f-200">Az.PolicyInsights</span></span>
* <span data-ttu-id="a117f-201">Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar</span><span class="sxs-lookup"><span data-stu-id="a117f-201">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="a117f-202">Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation</span><span class="sxs-lookup"><span data-stu-id="a117f-202">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="a117f-203">Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política</span><span class="sxs-lookup"><span data-stu-id="a117f-203">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="a117f-204">Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="a117f-204">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-205">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-205">Az.RecoveryServices</span></span>
* <span data-ttu-id="a117f-206">Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.</span><span class="sxs-lookup"><span data-stu-id="a117f-206">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="a117f-207">O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.</span><span class="sxs-lookup"><span data-stu-id="a117f-207">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-208">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-208">Az.Resources</span></span>
* <span data-ttu-id="a117f-209">-Scope foi tornado opcional nos cmdlets \*-AzPolicyAssignment com subscrição de contexto predefinida</span><span class="sxs-lookup"><span data-stu-id="a117f-209">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="a117f-210">Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves</span><span class="sxs-lookup"><span data-stu-id="a117f-210">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-211">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-211">Az.Sql</span></span>
<span data-ttu-id="a117f-212">Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.</span><span class="sxs-lookup"><span data-stu-id="a117f-212">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-213">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-213">Az.Storage</span></span>
* <span data-ttu-id="a117f-214">Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a117f-214">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="a117f-215">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-215">New-AzStorageAccount</span></span>
* <span data-ttu-id="a117f-216">Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation</span><span class="sxs-lookup"><span data-stu-id="a117f-216">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="a117f-217">Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="a117f-217">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a117f-218">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-218">Az.Websites</span></span>
* <span data-ttu-id="a117f-219">Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState</span><span class="sxs-lookup"><span data-stu-id="a117f-219">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="a117f-220">Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido</span><span class="sxs-lookup"><span data-stu-id="a117f-220">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="a117f-221">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="a117f-221">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a117f-222">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-222">Az.Accounts</span></span>
* <span data-ttu-id="a117f-223">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="a117f-223">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a117f-224">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a117f-224">Az.Cdn</span></span>
* <span data-ttu-id="a117f-225">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="a117f-225">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-226">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-226">Az.Compute</span></span>
* <span data-ttu-id="a117f-227">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="a117f-227">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="a117f-228">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a117f-228">Az.ContainerInstance</span></span>
* <span data-ttu-id="a117f-229">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="a117f-229">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="a117f-230">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="a117f-230">Az.DataBoxEdge</span></span>
* <span data-ttu-id="a117f-231">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="a117f-231">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="a117f-232">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="a117f-232">Get the Edge Storage Container</span></span>
* <span data-ttu-id="a117f-233">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="a117f-233">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="a117f-234">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="a117f-234">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="a117f-235">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="a117f-235">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="a117f-236">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="a117f-236">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="a117f-237">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="a117f-237">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="a117f-238">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="a117f-238">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="a117f-239">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a117f-239">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="a117f-240">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="a117f-240">Get the Edge Storage Account</span></span>
* <span data-ttu-id="a117f-241">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a117f-241">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="a117f-242">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="a117f-242">Create new Edge Storage Account</span></span>
* <span data-ttu-id="a117f-243">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="a117f-243">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="a117f-244">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="a117f-244">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="a117f-245">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="a117f-245">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="a117f-246">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="a117f-246">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="a117f-247">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="a117f-247">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="a117f-248">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="a117f-248">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a117f-249">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a117f-249">Az.DataFactory</span></span>
* <span data-ttu-id="a117f-250">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="a117f-250">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="a117f-251">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="a117f-251">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="a117f-252">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="a117f-252">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="a117f-253">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="a117f-253">Az.DevTestLabs</span></span>
* <span data-ttu-id="a117f-254">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="a117f-254">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a117f-255">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a117f-255">Az.EventHub</span></span>
* <span data-ttu-id="a117f-256">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="a117f-256">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a117f-257">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a117f-257">Az.HDInsight</span></span>
* <span data-ttu-id="a117f-258">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="a117f-258">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="a117f-259">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="a117f-259">Az.MachineLearning</span></span>
* <span data-ttu-id="a117f-260">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="a117f-260">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="a117f-261">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="a117f-261">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="a117f-262">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="a117f-262">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="a117f-263">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="a117f-263">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="a117f-264">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="a117f-264">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="a117f-265">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="a117f-265">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="a117f-266">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="a117f-266">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="a117f-267">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="a117f-267">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-268">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-268">Az.Network</span></span>
* <span data-ttu-id="a117f-269">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="a117f-269">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-270">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-270">Az.RecoveryServices</span></span>
* <span data-ttu-id="a117f-271">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-271">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="a117f-272">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-272">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="a117f-273">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-273">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="a117f-274">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-274">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-275">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-275">Az.Resources</span></span>
* <span data-ttu-id="a117f-276">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="a117f-276">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-277">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-277">Az.Sql</span></span>
* <span data-ttu-id="a117f-278">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="a117f-278">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="a117f-279">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="a117f-279">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="a117f-280">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="a117f-280">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="a117f-281">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="a117f-281">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-282">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-282">Az.Storage</span></span>
* <span data-ttu-id="a117f-283">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="a117f-283">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="a117f-284">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="a117f-284">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="a117f-285">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="a117f-285">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span> 
    - <span data-ttu-id="a117f-286">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-286">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="a117f-287">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-287">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="a117f-288">Geral</span><span class="sxs-lookup"><span data-stu-id="a117f-288">General</span></span>
* <span data-ttu-id="a117f-289">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="a117f-289">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a117f-290">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-290">Az.Accounts</span></span>
* <span data-ttu-id="a117f-291">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="a117f-291">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="a117f-292">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="a117f-292">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="a117f-293">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a117f-293">Az.Batch</span></span>
* <span data-ttu-id="a117f-294">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="a117f-294">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a117f-295">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a117f-295">Az.DataFactory</span></span>
* <span data-ttu-id="a117f-296">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="a117f-296">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a117f-297">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a117f-297">Az.FrontDoor</span></span>
* <span data-ttu-id="a117f-298">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="a117f-298">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="a117f-299">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="a117f-299">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="a117f-300">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="a117f-300">Az.HealthcareApis</span></span>
* <span data-ttu-id="a117f-301">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="a117f-301">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a117f-302">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a117f-302">Az.KeyVault</span></span>
* <span data-ttu-id="a117f-303">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="a117f-303">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="a117f-304">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="a117f-304">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="a117f-305">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="a117f-305">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a117f-306">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a117f-306">Az.Monitor</span></span>
* <span data-ttu-id="a117f-307">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="a117f-307">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="a117f-308">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="a117f-308">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="a117f-309">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="a117f-309">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-310">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-310">Az.Network</span></span>
* <span data-ttu-id="a117f-311">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="a117f-311">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-312">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-312">Az.Resources</span></span>
* <span data-ttu-id="a117f-313">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="a117f-313">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="a117f-314">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="a117f-314">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-315">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-315">Az.Sql</span></span>
* <span data-ttu-id="a117f-316">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="a117f-316">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-317">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-317">Az.Storage</span></span>
* <span data-ttu-id="a117f-318">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="a117f-318">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="a117f-319">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="a117f-319">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="a117f-320">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="a117f-320">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="a117f-321">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="a117f-321">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="a117f-322">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="a117f-322">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="a117f-323">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="a117f-323">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="a117f-324">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="a117f-324">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span> 
    - <span data-ttu-id="a117f-325">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="a117f-325">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="a117f-326">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="a117f-326">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="a117f-327">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="a117f-327">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="a117f-328">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="a117f-328">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="a117f-329">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="a117f-329">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="a117f-330">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="a117f-330">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="a117f-331">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-331">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a117f-332">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a117f-332">Highlights since the last major release</span></span>
* <span data-ttu-id="a117f-333">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="a117f-333">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="a117f-334">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="a117f-334">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-335">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-335">Az.Compute</span></span>
* <span data-ttu-id="a117f-336">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="a117f-336">VM Reapply feature</span></span>
    - <span data-ttu-id="a117f-337">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="a117f-337">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="a117f-338">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="a117f-338">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="a117f-339">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a117f-339">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="a117f-340">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="a117f-340">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="a117f-341">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a117f-341">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="a117f-342">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="a117f-342">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="a117f-343">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="a117f-343">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="a117f-344">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="a117f-344">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="a117f-345">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="a117f-345">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="a117f-346">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a117f-346">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="a117f-347">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="a117f-347">Az.DataBoxEdge</span></span>
* <span data-ttu-id="a117f-348">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="a117f-348">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="a117f-349">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="a117f-349">Get the Order</span></span>
* <span data-ttu-id="a117f-350">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="a117f-350">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="a117f-351">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="a117f-351">Create new Order</span></span>
* <span data-ttu-id="a117f-352">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="a117f-352">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="a117f-353">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="a117f-353">Remove the Order</span></span>
* <span data-ttu-id="a117f-354">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="a117f-354">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="a117f-355">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="a117f-355">Now creates Local Share</span></span>
* <span data-ttu-id="a117f-356">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="a117f-356">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="a117f-357">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="a117f-357">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="a117f-358">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="a117f-358">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="a117f-359">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="a117f-359">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="a117f-360">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="a117f-360">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="a117f-361">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="a117f-361">Gets the information about Triggers</span></span>
* <span data-ttu-id="a117f-362">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="a117f-362">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="a117f-363">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="a117f-363">Create new Triggers</span></span>
* <span data-ttu-id="a117f-364">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="a117f-364">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="a117f-365">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="a117f-365">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a117f-366">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a117f-366">Az.DataFactory</span></span>
* <span data-ttu-id="a117f-367">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="a117f-367">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="a117f-368">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="a117f-368">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a117f-369">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a117f-369">Az.DataLakeStore</span></span>
* <span data-ttu-id="a117f-370">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="a117f-370">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a117f-371">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a117f-371">Az.EventHub</span></span>
* <span data-ttu-id="a117f-372">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="a117f-372">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a117f-373">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a117f-373">Az.FrontDoor</span></span>
* <span data-ttu-id="a117f-374">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="a117f-374">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="a117f-375">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="a117f-375">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="a117f-376">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="a117f-376">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="a117f-377">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="a117f-377">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-378">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-378">Az.Network</span></span>
* <span data-ttu-id="a117f-379">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="a117f-379">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="a117f-380">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="a117f-380">Az.PrivateDns</span></span>
* <span data-ttu-id="a117f-381">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="a117f-381">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-382">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-382">Az.RecoveryServices</span></span>
* <span data-ttu-id="a117f-383">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="a117f-383">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="a117f-384">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="a117f-384">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="a117f-385">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="a117f-385">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="a117f-386">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="a117f-386">Az.RedisCache</span></span>
* <span data-ttu-id="a117f-387">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="a117f-387">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="a117f-388">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="a117f-388">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="a117f-389">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="a117f-389">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-390">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-390">Az.Resources</span></span>
- <span data-ttu-id="a117f-391">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="a117f-391">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="a117f-392">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="a117f-392">Updated create policy definition help example</span></span>
- <span data-ttu-id="a117f-393">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="a117f-393">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="a117f-394">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="a117f-394">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="a117f-395">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="a117f-395">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-396">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-396">Az.Sql</span></span>
* <span data-ttu-id="a117f-397">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="a117f-397">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="a117f-398">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="a117f-398">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="a117f-399">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-399">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="a117f-400">Geral</span><span class="sxs-lookup"><span data-stu-id="a117f-400">General</span></span>
* <span data-ttu-id="a117f-401">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="a117f-401">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a117f-402">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-402">Az.Accounts</span></span>
* <span data-ttu-id="a117f-403">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="a117f-403">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="a117f-404">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="a117f-404">Az.Advisor</span></span>
* <span data-ttu-id="a117f-405">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="a117f-405">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="a117f-406">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a117f-406">Az.Batch</span></span>
* <span data-ttu-id="a117f-407">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="a117f-407">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="a117f-408">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="a117f-408">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="a117f-409">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="a117f-409">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="a117f-410">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="a117f-410">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="a117f-411">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="a117f-411">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="a117f-412">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="a117f-412">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="a117f-413">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="a117f-413">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="a117f-414">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="a117f-414">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="a117f-415">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="a117f-415">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="a117f-416">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="a117f-416">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="a117f-417">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="a117f-417">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="a117f-418">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="a117f-418">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="a117f-419">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="a117f-419">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="a117f-420">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="a117f-420">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="a117f-421">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="a117f-421">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="a117f-422">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="a117f-422">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="a117f-423">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="a117f-423">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="a117f-424">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="a117f-424">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="a117f-425">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="a117f-425">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="a117f-426">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="a117f-426">This operation is no longer supported.</span></span>
* <span data-ttu-id="a117f-427">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="a117f-427">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="a117f-428">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="a117f-428">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="a117f-429">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="a117f-429">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="a117f-430">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="a117f-430">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span> 
  - <span data-ttu-id="a117f-431">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="a117f-431">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="a117f-432">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="a117f-432">New non-verified images are also now returned.</span></span> <span data-ttu-id="a117f-433">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="a117f-433">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="a117f-434">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="a117f-434">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="a117f-435">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="a117f-435">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="a117f-436">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="a117f-436">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="a117f-437">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="a117f-437">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="a117f-438">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="a117f-438">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="a117f-439">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="a117f-439">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="a117f-440">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="a117f-440">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="a117f-441">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="a117f-441">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="a117f-442">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="a117f-442">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a117f-443">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a117f-443">Az.Cdn</span></span>
* <span data-ttu-id="a117f-444">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="a117f-444">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="a117f-445">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="a117f-445">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-446">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-446">Az.Compute</span></span>
* <span data-ttu-id="a117f-447">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="a117f-447">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="a117f-448">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="a117f-448">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="a117f-449">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span><span class="sxs-lookup"><span data-stu-id="a117f-449">DiskEncryptionSetId parameter is added to the following cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span></span>        
        <span data-ttu-id="a117f-450">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="a117f-450">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="a117f-451">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-451">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="a117f-452">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-452">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="a117f-453">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="a117f-453">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="a117f-454">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a117f-454">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="a117f-455">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="a117f-455">Breaking changes</span></span>
    - <span data-ttu-id="a117f-456">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="a117f-456">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="a117f-457">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="a117f-457">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a117f-458">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a117f-458">Az.DataFactory</span></span>
* <span data-ttu-id="a117f-459">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="a117f-459">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a117f-460">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a117f-460">Az.DataLakeStore</span></span>
* <span data-ttu-id="a117f-461">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="a117f-461">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="a117f-462">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="a117f-462">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="a117f-463">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="a117f-463">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="a117f-464">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="a117f-464">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="a117f-465">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="a117f-465">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="a117f-466">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="a117f-466">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a117f-467">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a117f-467">Az.FrontDoor</span></span>
* <span data-ttu-id="a117f-468">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="a117f-468">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a117f-469">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a117f-469">Az.HDInsight</span></span>
* <span data-ttu-id="a117f-470">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="a117f-470">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="a117f-471">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="a117f-471">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="a117f-472">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="a117f-472">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="a117f-473">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a117f-473">Removed five cmdlets:</span></span>
    - <span data-ttu-id="a117f-474">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="a117f-474">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="a117f-475">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="a117f-475">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="a117f-476">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="a117f-476">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="a117f-477">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="a117f-477">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="a117f-478">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="a117f-478">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="a117f-479">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a117f-479">Added three cmdlets:</span></span>
    - <span data-ttu-id="a117f-480">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="a117f-480">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="a117f-481">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="a117f-481">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="a117f-482">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="a117f-482">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="a117f-483">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="a117f-483">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="a117f-484">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="a117f-484">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="a117f-485">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="a117f-485">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="a117f-486">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a117f-486">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="a117f-487">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="a117f-487">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="a117f-488">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="a117f-488">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="a117f-489">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="a117f-489">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="a117f-490">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="a117f-490">Added some scenario test cases.</span></span>
* <span data-ttu-id="a117f-491">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="a117f-491">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a117f-492">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a117f-492">Az.IotHub</span></span>
* <span data-ttu-id="a117f-493">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="a117f-493">Breaking changes:</span></span>
    - <span data-ttu-id="a117f-494">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="a117f-494">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="a117f-495">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="a117f-495">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="a117f-496">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="a117f-496">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="a117f-497">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="a117f-497">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="a117f-498">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="a117f-498">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="a117f-499">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="a117f-499">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="a117f-500">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="a117f-500">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="a117f-501">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="a117f-501">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="a117f-502">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="a117f-502">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="a117f-503">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="a117f-503">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="a117f-504">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="a117f-504">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="a117f-505">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="a117f-505">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-506">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-506">Az.RecoveryServices</span></span>
* <span data-ttu-id="a117f-507">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-507">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="a117f-508">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-508">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="a117f-509">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-509">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="a117f-510">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-510">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="a117f-511">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-511">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="a117f-512">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-512">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="a117f-513">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-513">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="a117f-514">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-514">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="a117f-515">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="a117f-515">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-516">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-516">Az.Resources</span></span>
* <span data-ttu-id="a117f-517">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="a117f-517">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-518">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-518">Az.Network</span></span>
* <span data-ttu-id="a117f-519">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="a117f-519">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="a117f-520">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="a117f-520">Updated cmdlet:</span></span>
        - <span data-ttu-id="a117f-521">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-521">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a117f-522">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-522">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a117f-523">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-523">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a117f-524">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-524">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a117f-525">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-525">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="a117f-526">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="a117f-526">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="a117f-527">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="a117f-527">New cmdlet:</span></span>
        - <span data-ttu-id="a117f-528">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="a117f-528">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="a117f-529">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="a117f-529">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="a117f-530">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a117f-530">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="a117f-531">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-531">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="a117f-532">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="a117f-532">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="a117f-533">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="a117f-533">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="a117f-534">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="a117f-534">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="a117f-535">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="a117f-535">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="a117f-536">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a117f-536">New cmdlets added:</span></span>
        - <span data-ttu-id="a117f-537">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="a117f-537">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="a117f-538">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="a117f-538">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="a117f-539">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="a117f-539">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="a117f-540">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="a117f-540">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="a117f-541">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="a117f-541">Set-AzVirtualHub</span></span>
* <span data-ttu-id="a117f-542">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="a117f-542">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="a117f-543">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="a117f-543">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="a117f-544">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="a117f-544">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="a117f-545">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="a117f-545">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="a117f-546">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="a117f-546">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="a117f-547">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="a117f-547">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="a117f-548">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-548">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="a117f-549">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a117f-549">New cmdlets added:</span></span>
        - <span data-ttu-id="a117f-550">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-550">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="a117f-551">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="a117f-551">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="a117f-552">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="a117f-552">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="a117f-553">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="a117f-553">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="a117f-554">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="a117f-554">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="a117f-555">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="a117f-555">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="a117f-556">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="a117f-556">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="a117f-557">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="a117f-557">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="a117f-558">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a117f-558">New cmdlets added:</span></span>
        - <span data-ttu-id="a117f-559">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="a117f-559">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="a117f-560">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="a117f-560">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="a117f-561">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="a117f-561">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="a117f-562">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="a117f-562">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="a117f-563">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="a117f-563">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="a117f-564">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="a117f-564">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="a117f-565">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="a117f-565">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="a117f-566">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="a117f-566">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="a117f-567">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="a117f-567">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="a117f-568">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="a117f-568">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="a117f-569">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="a117f-569">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="a117f-570">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="a117f-570">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="a117f-571">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="a117f-571">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="a117f-572">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="a117f-572">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="a117f-573">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="a117f-573">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="a117f-574">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="a117f-574">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="a117f-575">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="a117f-575">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="a117f-576">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a117f-576">New cmdlets added:</span></span>
        - <span data-ttu-id="a117f-577">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="a117f-577">New-AzIpGroup</span></span>
        - <span data-ttu-id="a117f-578">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="a117f-578">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="a117f-579">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="a117f-579">Get-AzIpGroup</span></span>
        - <span data-ttu-id="a117f-580">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="a117f-580">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a117f-581">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a117f-581">Az.ServiceFabric</span></span>
* <span data-ttu-id="a117f-582">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="a117f-582">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-583">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-583">Az.Sql</span></span>
* <span data-ttu-id="a117f-584">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="a117f-584">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="a117f-585">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="a117f-585">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="a117f-586">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="a117f-586">Removed deprecated aliases:</span></span>
* <span data-ttu-id="a117f-587">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="a117f-587">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="a117f-588">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="a117f-588">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="a117f-589">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a117f-589">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="a117f-590">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="a117f-590">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="a117f-591">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="a117f-591">Deprecate Advanced Threat Detection Settings cmdlets</span></span> 
* <span data-ttu-id="a117f-592">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="a117f-592">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-593">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-593">Az.Storage</span></span>
* <span data-ttu-id="a117f-594">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="a117f-594">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="a117f-595">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-595">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="a117f-596">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-596">Set-AzStorageAccount</span></span>
* <span data-ttu-id="a117f-597">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="a117f-597">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="a117f-598">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="a117f-598">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="a117f-599">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="a117f-599">Close-AzStorageFileHandle</span></span>
    
## <a name="280---october-2019"></a><span data-ttu-id="a117f-600">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-600">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="a117f-601">Geral</span><span class="sxs-lookup"><span data-stu-id="a117f-601">General</span></span>
* <span data-ttu-id="a117f-602">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="a117f-602">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a117f-603">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-603">Az.Accounts</span></span>
* <span data-ttu-id="a117f-604">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="a117f-604">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="a117f-605">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a117f-605">Az.ApiManagement</span></span>
* <span data-ttu-id="a117f-606">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="a117f-606">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="a117f-607">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="a117f-607">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a117f-608">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a117f-608">Az.Automation</span></span>
* <span data-ttu-id="a117f-609">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="a117f-609">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="a117f-610">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a117f-610">Az.Batch</span></span>
* <span data-ttu-id="a117f-611">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="a117f-611">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-612">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-612">Az.Compute</span></span>
* <span data-ttu-id="a117f-613">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a117f-613">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="a117f-614">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="a117f-614">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="a117f-615">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="a117f-615">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="a117f-616">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="a117f-616">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a117f-617">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a117f-617">Az.DataFactory</span></span>
* <span data-ttu-id="a117f-618">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="a117f-618">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="a117f-619">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="a117f-619">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="a117f-620">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="a117f-620">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a117f-621">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a117f-621">Az.DataLakeStore</span></span>
* <span data-ttu-id="a117f-622">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="a117f-622">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="a117f-623">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="a117f-623">Az.HealthcareApis</span></span>
* <span data-ttu-id="a117f-624">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="a117f-624">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="a117f-625">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="a117f-625">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="a117f-626">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="a117f-626">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="a117f-627">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="a117f-627">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a117f-628">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a117f-628">Az.IotHub</span></span>
* <span data-ttu-id="a117f-629">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="a117f-629">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="a117f-630">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="a117f-630">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="a117f-631">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a117f-631">Az.Monitor</span></span>
* <span data-ttu-id="a117f-632">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="a117f-632">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="a117f-633">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="a117f-633">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="a117f-634">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="a117f-634">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="a117f-635">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a117f-635">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-636">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-636">Az.Network</span></span>
* <span data-ttu-id="a117f-637">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="a117f-637">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="a117f-638">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="a117f-638">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="a117f-639">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a117f-639">New cmdlets added:</span></span>
        - <span data-ttu-id="a117f-640">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="a117f-640">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="a117f-641">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-641">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="a117f-642">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="a117f-642">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="a117f-643">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="a117f-643">Updated cmdlets:</span></span>
        - <span data-ttu-id="a117f-644">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-644">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="a117f-645">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-645">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="a117f-646">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-646">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="a117f-647">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="a117f-647">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="a117f-648">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="a117f-648">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="a117f-649">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="a117f-649">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="a117f-650">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="a117f-650">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="a117f-651">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="a117f-651">Az.RedisCache</span></span>
* <span data-ttu-id="a117f-652">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="a117f-652">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-653">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-653">Az.Sql</span></span>
* <span data-ttu-id="a117f-654">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="a117f-654">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-655">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-655">Az.Storage</span></span>
* <span data-ttu-id="a117f-656">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="a117f-656">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="a117f-657">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="a117f-657">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="a117f-658">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="a117f-658">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="a117f-659">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="a117f-659">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="a117f-660">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-660">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="a117f-661">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="a117f-661">Az.StorageSync</span></span>
* <span data-ttu-id="a117f-662">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="a117f-662">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a117f-663">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-663">Az.Websites</span></span>
* <span data-ttu-id="a117f-664">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="a117f-664">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="a117f-665">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-665">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="a117f-666">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a117f-666">Az.ApiManagement</span></span>
* <span data-ttu-id="a117f-667">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="a117f-667">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="a117f-668">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="a117f-668">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="a117f-669">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="a117f-669">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a117f-670">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a117f-670">Az.Automation</span></span>
* <span data-ttu-id="a117f-671">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="a117f-671">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="a117f-672">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="a117f-672">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="a117f-673">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="a117f-673">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-674">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-674">Az.Compute</span></span>
* <span data-ttu-id="a117f-675">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-675">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="a117f-676">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-676">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="a117f-677">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="a117f-677">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="a117f-678">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="a117f-678">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="a117f-679">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="a117f-679">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="a117f-680">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="a117f-680">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="a117f-681">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="a117f-681">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="a117f-682">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="a117f-682">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="a117f-683">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="a117f-683">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a117f-684">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a117f-684">Az.DataFactory</span></span>
* <span data-ttu-id="a117f-685">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="a117f-685">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="a117f-686">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="a117f-686">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="a117f-687">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a117f-687">Az.HDInsight</span></span>
* <span data-ttu-id="a117f-688">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="a117f-688">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a117f-689">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a117f-689">Az.IotHub</span></span>
* <span data-ttu-id="a117f-690">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="a117f-690">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="a117f-691">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="a117f-691">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="a117f-692">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="a117f-692">New cmdlets are:</span></span>
    - <span data-ttu-id="a117f-693">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="a117f-693">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="a117f-694">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="a117f-694">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="a117f-695">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="a117f-695">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="a117f-696">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="a117f-696">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a117f-697">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a117f-697">Az.Monitor</span></span>
* <span data-ttu-id="a117f-698">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="a117f-698">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="a117f-699">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="a117f-699">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="a117f-700">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="a117f-700">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="a117f-701">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="a117f-701">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="a117f-702">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="a117f-702">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="a117f-703">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="a117f-703">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="a117f-704">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="a117f-704">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="a117f-705">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="a117f-705">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="a117f-706">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="a117f-706">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="a117f-707">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="a117f-707">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="a117f-708">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="a117f-708">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="a117f-709">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="a117f-709">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="a117f-710">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="a117f-710">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="a117f-711">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="a117f-711">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="a117f-712">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="a117f-712">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="a117f-713">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="a117f-713">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="a117f-714">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="a117f-714">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="a117f-715">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="a117f-715">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="a117f-716">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="a117f-716">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="a117f-717">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="a117f-717">Overall improved help files</span></span>
* <span data-ttu-id="a117f-718">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="a117f-718">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-719">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-719">Az.Network</span></span>
* <span data-ttu-id="a117f-720">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="a117f-720">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="a117f-721">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="a117f-721">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="a117f-722">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="a117f-722">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="a117f-723">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="a117f-723">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="a117f-724">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="a117f-724">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="a117f-725">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="a117f-725">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="a117f-726">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="a117f-726">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="a117f-727">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="a117f-727">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="a117f-728">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="a117f-728">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="a117f-729">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="a117f-729">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="a117f-730">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="a117f-730">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="a117f-731">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="a117f-731">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="a117f-732">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a117f-732">New cmdlets</span></span>
        - <span data-ttu-id="a117f-733">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="a117f-733">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="a117f-734">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-734">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="a117f-735">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="a117f-735">Updated cmdlet:</span></span>
        - <span data-ttu-id="a117f-736">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="a117f-736">New-VpnSite</span></span>
        - <span data-ttu-id="a117f-737">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="a117f-737">Update-VpnSite</span></span>
        - <span data-ttu-id="a117f-738">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-738">New-VpnConnection</span></span>
        - <span data-ttu-id="a117f-739">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-739">Update-VpnConnection</span></span>
* <span data-ttu-id="a117f-740">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="a117f-740">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-741">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-741">Az.RecoveryServices</span></span>
* <span data-ttu-id="a117f-742">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="a117f-742">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="a117f-743">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="a117f-743">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-744">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-744">Az.Resources</span></span>
* <span data-ttu-id="a117f-745">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="a117f-745">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a117f-746">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a117f-746">Az.ServiceFabric</span></span>
* <span data-ttu-id="a117f-747">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="a117f-747">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="a117f-748">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="a117f-748">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="a117f-749">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="a117f-749">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="a117f-750">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="a117f-750">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="a117f-751">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="a117f-751">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="a117f-752">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="a117f-752">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="a117f-753">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="a117f-753">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="a117f-754">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="a117f-754">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="a117f-755">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="a117f-755">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="a117f-756">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="a117f-756">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="a117f-757">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="a117f-757">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="a117f-758">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="a117f-758">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="a117f-759">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="a117f-759">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="a117f-760">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="a117f-760">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="a117f-761">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="a117f-761">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="a117f-762">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="a117f-762">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="a117f-763">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="a117f-763">Az.SignalR</span></span>
* <span data-ttu-id="a117f-764">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="a117f-764">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-765">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-765">Az.Sql</span></span>
* <span data-ttu-id="a117f-766">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="a117f-766">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="a117f-767">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="a117f-767">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="a117f-768">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a117f-768">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="a117f-769">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="a117f-769">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="a117f-770">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="a117f-770">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-771">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-771">Az.Storage</span></span>
* <span data-ttu-id="a117f-772">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="a117f-772">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="a117f-773">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="a117f-773">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="a117f-774">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="a117f-774">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="a117f-775">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="a117f-775">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="a117f-776">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="a117f-776">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="a117f-777">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="a117f-777">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="a117f-778">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="a117f-778">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="a117f-779">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="a117f-779">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="a117f-780">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="a117f-780">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="a117f-781">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="a117f-781">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="a117f-782">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="a117f-782">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a117f-783">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-783">Az.Websites</span></span>
* <span data-ttu-id="a117f-784">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="a117f-784">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="a117f-785">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="a117f-785">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="a117f-786">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="a117f-786">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="a117f-787">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-787">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="a117f-788">Geral</span><span class="sxs-lookup"><span data-stu-id="a117f-788">General</span></span>
* <span data-ttu-id="a117f-789">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="a117f-789">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a117f-790">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-790">Az.Accounts</span></span>
* <span data-ttu-id="a117f-791">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="a117f-791">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="a117f-792">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="a117f-792">Az.Aks</span></span>
* <span data-ttu-id="a117f-793">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="a117f-793">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="a117f-794">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="a117f-794">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="a117f-795">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a117f-795">Az.ApiManagement</span></span>
* <span data-ttu-id="a117f-796">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="a117f-796">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="a117f-797">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="a117f-797">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="a117f-798">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="a117f-798">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="a117f-799">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="a117f-799">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="a117f-800">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="a117f-800">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="a117f-801">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a117f-801">Az.Batch</span></span>
* <span data-ttu-id="a117f-802">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="a117f-802">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a117f-803">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a117f-803">Az.Cdn</span></span>
* <span data-ttu-id="a117f-804">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="a117f-804">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-805">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-805">Az.Compute</span></span>
* <span data-ttu-id="a117f-806">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-806">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="a117f-807">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a117f-807">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="a117f-808">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="a117f-808">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="a117f-809">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="a117f-809">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="a117f-810">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="a117f-810">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="a117f-811">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="a117f-811">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="a117f-812">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="a117f-812">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="a117f-813">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="a117f-813">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a117f-814">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a117f-814">Az.DataFactory</span></span>
* <span data-ttu-id="a117f-815">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="a117f-815">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="a117f-816">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="a117f-816">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="a117f-817">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="a117f-817">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="a117f-818">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="a117f-818">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a117f-819">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a117f-819">Az.DataLakeStore</span></span>
* <span data-ttu-id="a117f-820">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="a117f-820">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a117f-821">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a117f-821">Az.EventHub</span></span>
* <span data-ttu-id="a117f-822">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="a117f-822">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="a117f-823">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="a117f-823">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="a117f-824">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="a117f-824">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="a117f-825">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="a117f-825">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="a117f-826">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="a117f-826">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="a117f-827">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="a117f-827">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a117f-828">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a117f-828">Az.Monitor</span></span>
* <span data-ttu-id="a117f-829">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="a117f-829">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-830">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-830">Az.Network</span></span>
* <span data-ttu-id="a117f-831">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="a117f-831">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="a117f-832">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="a117f-832">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="a117f-833">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="a117f-833">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="a117f-834">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="a117f-834">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="a117f-835">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="a117f-835">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="a117f-836">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="a117f-836">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="a117f-837">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="a117f-837">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a117f-838">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a117f-838">Az.OperationalInsights</span></span>
* <span data-ttu-id="a117f-839">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="a117f-839">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="a117f-840">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="a117f-840">Added example</span></span>
    - <span data-ttu-id="a117f-841">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="a117f-841">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="a117f-842">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="a117f-842">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="a117f-843">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="a117f-843">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-844">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-844">Az.RecoveryServices</span></span>
* <span data-ttu-id="a117f-845">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="a117f-845">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-846">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-846">Az.Resources</span></span>
* <span data-ttu-id="a117f-847">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="a117f-847">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="a117f-848">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="a117f-848">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="a117f-849">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="a117f-849">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="a117f-850">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="a117f-850">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a117f-851">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a117f-851">Az.ServiceBus</span></span>
* <span data-ttu-id="a117f-852">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="a117f-852">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="a117f-853">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="a117f-853">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="a117f-854">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="a117f-854">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="a117f-855">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a117f-855">Az.ServiceFabric</span></span>
* <span data-ttu-id="a117f-856">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="a117f-856">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="a117f-857">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="a117f-857">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="a117f-858">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="a117f-858">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="a117f-859">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="a117f-859">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="a117f-860">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="a117f-860">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="a117f-861">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="a117f-861">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-862">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-862">Az.Sql</span></span>
* <span data-ttu-id="a117f-863">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="a117f-863">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-864">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-864">Az.Storage</span></span>
* <span data-ttu-id="a117f-865">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="a117f-865">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="a117f-866">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="a117f-866">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="a117f-867">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="a117f-867">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="a117f-868">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="a117f-868">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="a117f-869">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="a117f-869">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="a117f-870">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="a117f-870">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a117f-871">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-871">Az.Websites</span></span>
* <span data-ttu-id="a117f-872">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="a117f-872">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="a117f-873">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-873">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a117f-874">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-874">Az.Accounts</span></span>
* <span data-ttu-id="a117f-875">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="a117f-875">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="a117f-876">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="a117f-876">Az.ApplicationInsights</span></span>
* <span data-ttu-id="a117f-877">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="a117f-877">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="a117f-878">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a117f-878">Az.Automation</span></span>
* <span data-ttu-id="a117f-879">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="a117f-879">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="a117f-880">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a117f-880">Az.CognitiveServices</span></span>
* <span data-ttu-id="a117f-881">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="a117f-881">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-882">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-882">Az.Compute</span></span>
* <span data-ttu-id="a117f-883">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="a117f-883">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="a117f-884">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="a117f-884">Az.ContainerRegistry</span></span>
* <span data-ttu-id="a117f-885">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="a117f-885">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="a117f-886">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="a117f-886">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a117f-887">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a117f-887">Az.DataFactory</span></span>
* <span data-ttu-id="a117f-888">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="a117f-888">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="a117f-889">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="a117f-889">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a117f-890">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a117f-890">Az.EventHub</span></span>
* <span data-ttu-id="a117f-891">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="a117f-891">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="a117f-892">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="a117f-892">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a117f-893">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a117f-893">Az.KeyVault</span></span>
* <span data-ttu-id="a117f-894">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="a117f-894">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a117f-895">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a117f-895">Az.LogicApp</span></span>
* <span data-ttu-id="a117f-896">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="a117f-896">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="a117f-897">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="a117f-897">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="a117f-898">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="a117f-898">Az.ManagedServices</span></span>
* <span data-ttu-id="a117f-899">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="a117f-899">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-900">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-900">Az.Network</span></span>
* <span data-ttu-id="a117f-901">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="a117f-901">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="a117f-902">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a117f-902">New cmdlets</span></span>
        - <span data-ttu-id="a117f-903">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="a117f-903">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="a117f-904">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a117f-904">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="a117f-905">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-905">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a117f-906">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-906">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a117f-907">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-907">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a117f-908">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-908">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="a117f-909">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="a117f-909">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="a117f-910">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a117f-910">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="a117f-911">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="a117f-911">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="a117f-912">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-912">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="a117f-913">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="a117f-913">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="a117f-914">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="a117f-914">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="a117f-915">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="a117f-915">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="a117f-916">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="a117f-916">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="a117f-917">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="a117f-917">Updated cmdlets</span></span>
        - <span data-ttu-id="a117f-918">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-918">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="a117f-919">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-919">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="a117f-920">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-920">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="a117f-921">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-921">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="a117f-922">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="a117f-922">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="a117f-923">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="a117f-923">Updated cmdlet:</span></span>
        - <span data-ttu-id="a117f-924">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-924">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="a117f-925">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-925">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="a117f-926">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-926">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="a117f-927">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="a117f-927">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="a117f-928">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="a117f-928">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="a117f-929">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="a117f-929">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a117f-930">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a117f-930">Az.OperationalInsights</span></span>
* <span data-ttu-id="a117f-931">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="a117f-931">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="a117f-932">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="a117f-932">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-933">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-933">Az.RecoveryServices</span></span>
* <span data-ttu-id="a117f-934">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="a117f-934">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="a117f-935">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="a117f-935">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="a117f-936">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="a117f-936">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="a117f-937">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="a117f-937">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="a117f-938">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="a117f-938">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="a117f-939">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="a117f-939">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="a117f-940">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="a117f-940">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="a117f-941">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="a117f-941">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="a117f-942">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="a117f-942">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="a117f-943">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="a117f-943">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-944">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-944">Az.Resources</span></span>
- <span data-ttu-id="a117f-945">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="a117f-945">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="a117f-946">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="a117f-946">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a117f-947">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a117f-947">Az.ServiceBus</span></span>
* <span data-ttu-id="a117f-948">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="a117f-948">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="a117f-949">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="a117f-949">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-950">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-950">Az.Sql</span></span>
* <span data-ttu-id="a117f-951">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="a117f-951">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="a117f-952">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="a117f-952">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="a117f-953">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="a117f-953">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-954">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-954">Az.Storage</span></span>
* <span data-ttu-id="a117f-955">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="a117f-955">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="a117f-956">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="a117f-956">Az.StorageSync</span></span>
* <span data-ttu-id="a117f-957">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="a117f-957">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="a117f-958">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="a117f-958">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a117f-959">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-959">Az.Websites</span></span>
* <span data-ttu-id="a117f-960">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="a117f-960">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="a117f-961">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="a117f-961">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="a117f-962">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="a117f-962">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="a117f-963">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-963">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a117f-964">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-964">Az.Accounts</span></span>
* <span data-ttu-id="a117f-965">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="a117f-965">Add support for profile cmdlets</span></span>
* <span data-ttu-id="a117f-966">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="a117f-966">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="a117f-967">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="a117f-967">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="a117f-968">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="a117f-968">Az.Advisor</span></span>
* <span data-ttu-id="a117f-969">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="a117f-969">GA release of Az.Advisor</span></span>
* <span data-ttu-id="a117f-970">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="a117f-970">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="a117f-971">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a117f-971">Az.ApiManagement</span></span>
* <span data-ttu-id="a117f-972">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="a117f-972">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="a117f-973">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="a117f-973">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="a117f-974">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="a117f-974">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="a117f-975">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="a117f-975">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="a117f-976">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="a117f-976">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="a117f-977">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="a117f-977">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="a117f-978">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="a117f-978">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a117f-979">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a117f-979">Az.Automation</span></span>
* <span data-ttu-id="a117f-980">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="a117f-980">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-981">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-981">Az.Compute</span></span>
* <span data-ttu-id="a117f-982">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-982">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a117f-983">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a117f-983">Az.DataFactory</span></span>
* <span data-ttu-id="a117f-984">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="a117f-984">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="a117f-985">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a117f-985">Az.EventGrid</span></span>
* <span data-ttu-id="a117f-986">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="a117f-986">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a117f-987">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a117f-987">Az.IotHub</span></span>
* <span data-ttu-id="a117f-988">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="a117f-988">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-989">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-989">Az.Network</span></span>
* <span data-ttu-id="a117f-990">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="a117f-990">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="a117f-991">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="a117f-991">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a117f-992">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a117f-992">Az.PolicyInsights</span></span>
* <span data-ttu-id="a117f-993">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="a117f-993">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="a117f-994">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="a117f-994">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a117f-995">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a117f-995">Az.OperationalInsights</span></span>
* <span data-ttu-id="a117f-996">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="a117f-996">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-997">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-997">Az.RecoveryServices</span></span>
* <span data-ttu-id="a117f-998">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="a117f-998">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-999">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-999">Az.Resources</span></span>
    - <span data-ttu-id="a117f-1000">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="a117f-1000">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="a117f-1001">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="a117f-1001">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="a117f-1002">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="a117f-1002">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="a117f-1003">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="a117f-1003">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a117f-1004">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a117f-1004">Az.ServiceBus</span></span>
* <span data-ttu-id="a117f-1005">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="a117f-1005">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-1006">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-1006">Az.Sql</span></span>
* <span data-ttu-id="a117f-1007">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="a117f-1007">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="a117f-1008">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="a117f-1008">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="a117f-1009">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="a117f-1009">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="a117f-1010">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="a117f-1010">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="a117f-1011">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="a117f-1011">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="a117f-1012">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="a117f-1012">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="a117f-1013">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="a117f-1013">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="a117f-1014">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="a117f-1014">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="a117f-1015">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="a117f-1015">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-1016">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-1016">Az.Storage</span></span>
* <span data-ttu-id="a117f-1017">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="a117f-1017">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="a117f-1018">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="a117f-1018">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="a117f-1019">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="a117f-1019">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="a117f-1020">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="a117f-1020">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="a117f-1021">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="a117f-1021">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="a117f-1022">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-1022">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="a117f-1023">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-1023">Set-AzStorageAccount</span></span>
* <span data-ttu-id="a117f-1024">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="a117f-1024">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="a117f-1025">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="a117f-1025">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="a117f-1026">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="a117f-1026">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="a117f-1027">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="a117f-1027">Az.StorageSync</span></span>
* <span data-ttu-id="a117f-1028">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="a117f-1028">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="a117f-1029">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-1029">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a117f-1030">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-1030">Az.Accounts</span></span>
* <span data-ttu-id="a117f-1031">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="a117f-1031">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="a117f-1032">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="a117f-1032">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="a117f-1033">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="a117f-1033">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="a117f-1034">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="a117f-1034">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="a117f-1035">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="a117f-1035">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-1036">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1036">Az.Compute</span></span>
* <span data-ttu-id="a117f-1037">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="a117f-1037">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="a117f-1038">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="a117f-1038">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="a117f-1039">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="a117f-1039">Az.Dns</span></span>
* <span data-ttu-id="a117f-1040">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="a117f-1040">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="a117f-1041">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a117f-1041">Az.EventGrid</span></span>
* <span data-ttu-id="a117f-1042">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="a117f-1042">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="a117f-1043">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a117f-1043">New cmdlets:</span></span>
    - <span data-ttu-id="a117f-1044">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="a117f-1044">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="a117f-1045">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="a117f-1045">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="a117f-1046">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="a117f-1046">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="a117f-1047">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-1047">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="a117f-1048">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="a117f-1048">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="a117f-1049">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="a117f-1049">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="a117f-1050">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="a117f-1050">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="a117f-1051">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="a117f-1051">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="a117f-1052">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="a117f-1052">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="a117f-1053">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="a117f-1053">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="a117f-1054">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="a117f-1054">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="a117f-1055">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="a117f-1055">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="a117f-1056">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="a117f-1056">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="a117f-1057">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="a117f-1057">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="a117f-1058">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="a117f-1058">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="a117f-1059">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="a117f-1059">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="a117f-1060">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="a117f-1060">Updated cmdlets:</span></span>
    - <span data-ttu-id="a117f-1061">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="a117f-1061">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="a117f-1062">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="a117f-1062">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="a117f-1063">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="a117f-1063">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="a117f-1064">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="a117f-1064">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="a117f-1065">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="a117f-1065">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="a117f-1066">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="a117f-1066">Event subscription expiration date,</span></span>
            - <span data-ttu-id="a117f-1067">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="a117f-1067">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="a117f-1068">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="a117f-1068">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="a117f-1069">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="a117f-1069">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="a117f-1070">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="a117f-1070">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="a117f-1071">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="a117f-1071">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="a117f-1072">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="a117f-1072">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="a117f-1073">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="a117f-1073">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="a117f-1074">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="a117f-1074">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a117f-1075">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a117f-1075">Az.FrontDoor</span></span>
* <span data-ttu-id="a117f-1076">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="a117f-1076">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="a117f-1077">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="a117f-1077">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="a117f-1078">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="a117f-1078">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="a117f-1079">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="a117f-1079">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-1080">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1080">Az.Network</span></span>
* <span data-ttu-id="a117f-1081">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="a117f-1081">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="a117f-1082">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a117f-1082">New cmdlets</span></span>
        - <span data-ttu-id="a117f-1083">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="a117f-1083">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="a117f-1084">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="a117f-1084">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="a117f-1085">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a117f-1085">New cmdlets</span></span> 
        - <span data-ttu-id="a117f-1086">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="a117f-1086">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="a117f-1087">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a117f-1087">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="a117f-1088">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a117f-1088">New cmdlets</span></span> 
        - <span data-ttu-id="a117f-1089">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a117f-1089">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="a117f-1090">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a117f-1090">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="a117f-1091">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="a117f-1091">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="a117f-1092">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-1092">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="a117f-1093">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-1093">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="a117f-1094">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="a117f-1094">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="a117f-1095">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a117f-1095">New cmdlets</span></span>
        - <span data-ttu-id="a117f-1096">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="a117f-1096">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="a117f-1097">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="a117f-1097">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="a117f-1098">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="a117f-1098">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="a117f-1099">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-1099">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="a117f-1100">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="a117f-1100">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="a117f-1101">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="a117f-1101">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="a117f-1102">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="a117f-1102">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="a117f-1103">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="a117f-1103">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="a117f-1104">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="a117f-1104">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="a117f-1105">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="a117f-1105">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="a117f-1106">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="a117f-1106">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="a117f-1107">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="a117f-1107">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="a117f-1108">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="a117f-1108">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="a117f-1109">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="a117f-1109">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="a117f-1110">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="a117f-1110">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="a117f-1111">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="a117f-1111">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="a117f-1112">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="a117f-1112">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="a117f-1113">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="a117f-1113">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="a117f-1114">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="a117f-1114">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="a117f-1115">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="a117f-1115">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="a117f-1116">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="a117f-1116">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="a117f-1117">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="a117f-1117">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="a117f-1118">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="a117f-1118">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="a117f-1119">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="a117f-1119">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="a117f-1120">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="a117f-1120">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="a117f-1121">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="a117f-1121">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="a117f-1122">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="a117f-1122">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a117f-1123">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a117f-1123">Az.OperationalInsights</span></span>
* <span data-ttu-id="a117f-1124">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="a117f-1124">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-1125">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-1125">Az.Resources</span></span>
* <span data-ttu-id="a117f-1126">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="a117f-1126">Support for additional Template Export options</span></span>
    - <span data-ttu-id="a117f-1127">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="a117f-1127">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="a117f-1128">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="a117f-1128">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="a117f-1129">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="a117f-1129">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a117f-1130">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a117f-1130">Az.ServiceFabric</span></span>
* <span data-ttu-id="a117f-1131">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="a117f-1131">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-1132">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-1132">Az.Sql</span></span>
* <span data-ttu-id="a117f-1133">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="a117f-1133">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="a117f-1134">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="a117f-1134">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="a117f-1135">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="a117f-1135">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="a117f-1136">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="a117f-1136">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="a117f-1137">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="a117f-1137">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="a117f-1138">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="a117f-1138">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="a117f-1139">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="a117f-1139">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="a117f-1140">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="a117f-1140">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-1141">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-1141">Az.Storage</span></span>
* <span data-ttu-id="a117f-1142">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="a117f-1142">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="a117f-1143">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-1143">New-AzStorageAccount</span></span>
* <span data-ttu-id="a117f-1144">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="a117f-1144">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="a117f-1145">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="a117f-1145">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a117f-1146">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-1146">Az.Websites</span></span>
* <span data-ttu-id="a117f-1147">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="a117f-1147">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="a117f-1148">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="a117f-1148">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="a117f-1149">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-1149">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="a117f-1150">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a117f-1150">Az.Cdn</span></span>
* <span data-ttu-id="a117f-1151">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="a117f-1151">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-1152">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1152">Az.Compute</span></span>
* <span data-ttu-id="a117f-1153">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="a117f-1153">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="a117f-1154">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="a117f-1154">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a117f-1155">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a117f-1155">Az.EventHub</span></span>
* <span data-ttu-id="a117f-1156">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="a117f-1156">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="a117f-1157">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="a117f-1157">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-1158">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1158">Az.Network</span></span>
* <span data-ttu-id="a117f-1159">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="a117f-1159">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="a117f-1160">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="a117f-1160">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a117f-1161">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a117f-1161">Az.PolicyInsights</span></span>
* <span data-ttu-id="a117f-1162">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="a117f-1162">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-1163">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1163">Az.RecoveryServices</span></span>
* <span data-ttu-id="a117f-1164">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="a117f-1164">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a117f-1165">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a117f-1165">Az.ServiceBus</span></span>
* <span data-ttu-id="a117f-1166">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="a117f-1166">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a117f-1167">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a117f-1167">Az.ServiceFabric</span></span>
* <span data-ttu-id="a117f-1168">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="a117f-1168">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="a117f-1169">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a117f-1169">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-1170">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-1170">Az.Sql</span></span>
* <span data-ttu-id="a117f-1171">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="a117f-1171">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="a117f-1172">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a117f-1172">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="a117f-1173">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="a117f-1173">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="a117f-1174">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="a117f-1174">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a117f-1175">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-1175">Az.Websites</span></span>
* <span data-ttu-id="a117f-1176">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="a117f-1176">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="a117f-1177">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-1177">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="a117f-1178">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a117f-1178">Az.ApiManagement</span></span>
* <span data-ttu-id="a117f-1179">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="a117f-1179">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="a117f-1180">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="a117f-1180">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="a117f-1181">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="a117f-1181">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="a117f-1182">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="a117f-1182">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="a117f-1183">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="a117f-1183">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="a117f-1184">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="a117f-1184">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="a117f-1185">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="a117f-1185">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="a117f-1186">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="a117f-1186">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="a117f-1187">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a117f-1187">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="a117f-1188">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="a117f-1188">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="a117f-1189">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="a117f-1189">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="a117f-1190">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="a117f-1190">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="a117f-1191">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="a117f-1191">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="a117f-1192">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="a117f-1192">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="a117f-1193">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="a117f-1193">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="a117f-1194">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="a117f-1194">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="a117f-1195">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="a117f-1195">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="a117f-1196">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="a117f-1196">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="a117f-1197">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="a117f-1197">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="a117f-1198">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="a117f-1198">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="a117f-1199">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="a117f-1199">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="a117f-1200">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="a117f-1200">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="a117f-1201">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="a117f-1201">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="a117f-1202">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a117f-1202">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="a117f-1203">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="a117f-1203">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="a117f-1204">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="a117f-1204">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="a117f-1205">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="a117f-1205">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="a117f-1206">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="a117f-1206">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="a117f-1207">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="a117f-1207">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="a117f-1208">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="a117f-1208">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="a117f-1209">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="a117f-1209">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="a117f-1210">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="a117f-1210">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="a117f-1211">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="a117f-1211">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="a117f-1212">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="a117f-1212">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="a117f-1213">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="a117f-1213">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="a117f-1214">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="a117f-1214">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="a117f-1215">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="a117f-1215">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="a117f-1216">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="a117f-1216">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="a117f-1217">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="a117f-1217">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="a117f-1218">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="a117f-1218">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="a117f-1219">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="a117f-1219">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="a117f-1220">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="a117f-1220">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="a117f-1221">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="a117f-1221">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="a117f-1222">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="a117f-1222">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="a117f-1223">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="a117f-1223">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="a117f-1224">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="a117f-1224">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="a117f-1225">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="a117f-1225">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="a117f-1226">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="a117f-1226">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="a117f-1227">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="a117f-1227">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="a117f-1228">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="a117f-1228">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="a117f-1229">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="a117f-1229">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="a117f-1230">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="a117f-1230">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="a117f-1231">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="a117f-1231">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="a117f-1232">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="a117f-1232">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="a117f-1233">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="a117f-1233">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="a117f-1234">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="a117f-1234">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="a117f-1235">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="a117f-1235">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="a117f-1236">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="a117f-1236">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="a117f-1237">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="a117f-1237">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="a117f-1238">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="a117f-1238">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="a117f-1239">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="a117f-1239">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="a117f-1240">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="a117f-1240">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="a117f-1241">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="a117f-1241">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="a117f-1242">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="a117f-1242">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="a117f-1243">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="a117f-1243">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="a117f-1244">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="a117f-1244">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="a117f-1245">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="a117f-1245">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="a117f-1246">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="a117f-1246">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="a117f-1247">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="a117f-1247">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="a117f-1248">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="a117f-1248">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="a117f-1249">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="a117f-1249">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="a117f-1250">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="a117f-1250">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="a117f-1251">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="a117f-1251">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="a117f-1252">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="a117f-1252">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="a117f-1253">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="a117f-1253">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="a117f-1254">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="a117f-1254">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="a117f-1255">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="a117f-1255">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a117f-1256">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a117f-1256">Az.Automation</span></span>
* <span data-ttu-id="a117f-1257">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="a117f-1257">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="a117f-1258">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="a117f-1258">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="a117f-1259">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="a117f-1259">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="a117f-1260">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="a117f-1260">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="a117f-1261">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="a117f-1261">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="a117f-1262">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="a117f-1262">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="a117f-1263">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="a117f-1263">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-1264">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1264">Az.Compute</span></span>
* <span data-ttu-id="a117f-1265">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="a117f-1265">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="a117f-1266">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="a117f-1266">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a117f-1267">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a117f-1267">Az.DataLakeStore</span></span>
* <span data-ttu-id="a117f-1268">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="a117f-1268">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a117f-1269">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a117f-1269">Az.Monitor</span></span>
* <span data-ttu-id="a117f-1270">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="a117f-1270">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-1271">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1271">Az.Network</span></span>
* <span data-ttu-id="a117f-1272">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="a117f-1272">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="a117f-1273">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="a117f-1273">Updated cmdlet:</span></span>
        - <span data-ttu-id="a117f-1274">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="a117f-1274">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="a117f-1275">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a117f-1275">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-1276">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-1276">Az.Resources</span></span>
* <span data-ttu-id="a117f-1277">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="a117f-1277">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-1278">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-1278">Az.Sql</span></span>
* <span data-ttu-id="a117f-1279">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="a117f-1279">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="a117f-1280">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-1280">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a117f-1281">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-1281">Az.Accounts</span></span>
* <span data-ttu-id="a117f-1282">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="a117f-1282">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a117f-1283">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1283">Az.CognitiveServices</span></span>
* <span data-ttu-id="a117f-1284">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="a117f-1284">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="a117f-1285">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="a117f-1285">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-1286">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1286">Az.Compute</span></span>
* <span data-ttu-id="a117f-1287">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="a117f-1287">Proximity placement group feature.</span></span>
    - <span data-ttu-id="a117f-1288">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="a117f-1288">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="a117f-1289">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-1289">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="a117f-1290">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="a117f-1290">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="a117f-1291">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="a117f-1291">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="a117f-1292">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a117f-1292">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="a117f-1293">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="a117f-1293">Breaking changes</span></span>
    - <span data-ttu-id="a117f-1294">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="a117f-1294">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="a117f-1295">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="a117f-1295">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="a117f-1296">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="a117f-1296">Az.DeploymentManager</span></span>
* <span data-ttu-id="a117f-1297">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="a117f-1297">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="a117f-1298">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="a117f-1298">Az.Dns</span></span>
* <span data-ttu-id="a117f-1299">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="a117f-1299">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="a117f-1300">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="a117f-1300">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="a117f-1301">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="a117f-1301">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="a117f-1302">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a117f-1302">Az.FrontDoor</span></span>
* <span data-ttu-id="a117f-1303">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="a117f-1303">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="a117f-1304">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="a117f-1304">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="a117f-1305">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a117f-1305">Az.HDInsight</span></span>
* <span data-ttu-id="a117f-1306">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a117f-1306">Removed two cmdlets:</span></span>
    - <span data-ttu-id="a117f-1307">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="a117f-1307">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="a117f-1308">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="a117f-1308">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="a117f-1309">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="a117f-1309">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="a117f-1310">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="a117f-1310">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="a117f-1311">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="a117f-1311">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="a117f-1312">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="a117f-1312">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a117f-1313">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a117f-1313">Az.Monitor</span></span>
* <span data-ttu-id="a117f-1314">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="a117f-1314">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="a117f-1315">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="a117f-1315">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="a117f-1316">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="a117f-1316">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="a117f-1317">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="a117f-1317">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="a117f-1318">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="a117f-1318">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="a117f-1319">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="a117f-1319">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="a117f-1320">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="a117f-1320">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="a117f-1321">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="a117f-1321">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="a117f-1322">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="a117f-1322">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="a117f-1323">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="a117f-1323">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="a117f-1324">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="a117f-1324">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="a117f-1325">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="a117f-1325">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="a117f-1326">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="a117f-1326">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="a117f-1327">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="a117f-1327">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-1328">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1328">Az.Network</span></span>
* <span data-ttu-id="a117f-1329">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="a117f-1329">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="a117f-1330">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="a117f-1330">New cmdlets</span></span>
        - <span data-ttu-id="a117f-1331">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="a117f-1331">New-AzNatGateway</span></span>
        - <span data-ttu-id="a117f-1332">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="a117f-1332">Get-AzNatGateway</span></span>
        - <span data-ttu-id="a117f-1333">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="a117f-1333">Set-AzNatGateway</span></span>
        - <span data-ttu-id="a117f-1334">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="a117f-1334">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="a117f-1335">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="a117f-1335">Updated cmdlets</span></span>
        - <span data-ttu-id="a117f-1336">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="a117f-1336">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="a117f-1337">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="a117f-1337">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="a117f-1338">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="a117f-1338">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="a117f-1339">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="a117f-1339">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="a117f-1340">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="a117f-1340">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a117f-1341">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a117f-1341">Az.PolicyInsights</span></span>
* <span data-ttu-id="a117f-1342">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="a117f-1342">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="a117f-1343">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="a117f-1343">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="a117f-1344">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="a117f-1344">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-1345">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1345">Az.RecoveryServices</span></span>
* <span data-ttu-id="a117f-1346">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="a117f-1346">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="a117f-1347">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="a117f-1347">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="a117f-1348">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="a117f-1348">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="a117f-1349">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-1349">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="a117f-1350">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="a117f-1350">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="a117f-1351">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="a117f-1351">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="a117f-1352">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="a117f-1352">Az.Relay</span></span>
* <span data-ttu-id="a117f-1353">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="a117f-1353">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a117f-1354">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a117f-1354">Az.ServiceBus</span></span>
* <span data-ttu-id="a117f-1355">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="a117f-1355">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-1356">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-1356">Az.Storage</span></span>
* <span data-ttu-id="a117f-1357">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="a117f-1357">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="a117f-1358">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="a117f-1358">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="a117f-1359">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="a117f-1359">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="a117f-1360">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-1360">New-AzStorageAccount</span></span>
* <span data-ttu-id="a117f-1361">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="a117f-1361">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="a117f-1362">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-1362">New-AzStorageAccount</span></span>
    - <span data-ttu-id="a117f-1363">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-1363">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="a117f-1364">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-1364">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a117f-1365">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-1365">Az.Websites</span></span>
* <span data-ttu-id="a117f-1366">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="a117f-1366">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="a117f-1367">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="a117f-1367">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="a117f-1368">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-1368">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a117f-1369">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a117f-1369">Highlights since the last major release</span></span>
* <span data-ttu-id="a117f-1370">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="a117f-1370">General availability of `Az` module</span></span>
* <span data-ttu-id="a117f-1371">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="a117f-1371">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="a117f-1372">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="a117f-1372">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="a117f-1373">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1373">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="a117f-1374">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="a117f-1374">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a117f-1375">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a117f-1375">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="a117f-1376">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="a117f-1376">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a117f-1377">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-1377">Az.Accounts</span></span>
* <span data-ttu-id="a117f-1378">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="a117f-1378">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="a117f-1379">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a117f-1379">Az.Batch</span></span>
* <span data-ttu-id="a117f-1380">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1380">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a117f-1381">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a117f-1381">Az.Cdn</span></span>
* <span data-ttu-id="a117f-1382">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1382">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a117f-1383">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1383">Az.CognitiveServices</span></span>
* <span data-ttu-id="a117f-1384">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1384">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-1385">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1385">Az.Compute</span></span>
* <span data-ttu-id="a117f-1386">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="a117f-1386">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="a117f-1387">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1387">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a117f-1388">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="a117f-1388">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a117f-1389">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a117f-1389">Az.DataFactory</span></span>
* <span data-ttu-id="a117f-1390">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="a117f-1390">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a117f-1391">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a117f-1391">Az.DataLakeStore</span></span>
* <span data-ttu-id="a117f-1392">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1392">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="a117f-1393">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a117f-1393">Az.EventGrid</span></span>
* <span data-ttu-id="a117f-1394">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="a117f-1394">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a117f-1395">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a117f-1395">Az.EventHub</span></span>
* <span data-ttu-id="a117f-1396">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="a117f-1396">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="a117f-1397">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a117f-1397">Az.HDInsight</span></span>
* <span data-ttu-id="a117f-1398">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1398">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a117f-1399">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a117f-1399">Az.IotHub</span></span>
* <span data-ttu-id="a117f-1400">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1400">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a117f-1401">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a117f-1401">Az.KeyVault</span></span>
* <span data-ttu-id="a117f-1402">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1402">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a117f-1403">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="a117f-1403">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="a117f-1404">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="a117f-1404">Az.MachineLearning</span></span>
* <span data-ttu-id="a117f-1405">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1405">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="a117f-1406">Az.Media</span><span class="sxs-lookup"><span data-stu-id="a117f-1406">Az.Media</span></span>
* <span data-ttu-id="a117f-1407">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1407">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a117f-1408">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a117f-1408">Az.Monitor</span></span>
  * <span data-ttu-id="a117f-1409">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="a117f-1409">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="a117f-1410">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="a117f-1410">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="a117f-1411">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="a117f-1411">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="a117f-1412">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="a117f-1412">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="a117f-1413">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="a117f-1413">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="a117f-1414">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="a117f-1414">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="a117f-1415">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="a117f-1415">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-1416">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1416">Az.Network</span></span>
* <span data-ttu-id="a117f-1417">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1417">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a117f-1418">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="a117f-1418">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="a117f-1419">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="a117f-1419">Az.NotificationHubs</span></span>
* <span data-ttu-id="a117f-1420">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1420">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a117f-1421">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a117f-1421">Az.OperationalInsights</span></span>
* <span data-ttu-id="a117f-1422">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1422">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="a117f-1423">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="a117f-1423">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="a117f-1424">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1424">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-1425">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1425">Az.RecoveryServices</span></span>
* <span data-ttu-id="a117f-1426">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1426">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a117f-1427">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="a117f-1427">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="a117f-1428">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="a117f-1428">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="a117f-1429">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="a117f-1429">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="a117f-1430">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="a117f-1430">Az.RedisCache</span></span>
* <span data-ttu-id="a117f-1431">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1431">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-1432">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-1432">Az.Resources</span></span>
* <span data-ttu-id="a117f-1433">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="a117f-1433">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-1434">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-1434">Az.Sql</span></span>
* <span data-ttu-id="a117f-1435">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="a117f-1435">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="a117f-1436">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1436">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a117f-1437">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="a117f-1437">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="a117f-1438">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="a117f-1438">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="a117f-1439">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="a117f-1439">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="a117f-1440">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="a117f-1440">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="a117f-1441">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="a117f-1441">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a117f-1442">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-1442">Az.Websites</span></span>
* <span data-ttu-id="a117f-1443">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="a117f-1443">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="a117f-1444">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="a117f-1444">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="a117f-1445">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="a117f-1445">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="a117f-1446">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="a117f-1446">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="a117f-1447">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-1447">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a117f-1448">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a117f-1448">Highlights since the last major release</span></span>
* <span data-ttu-id="a117f-1449">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="a117f-1449">General availability of `Az` module</span></span>
* <span data-ttu-id="a117f-1450">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="a117f-1450">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="a117f-1451">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="a117f-1451">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="a117f-1452">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1452">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="a117f-1453">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="a117f-1453">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a117f-1454">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a117f-1454">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="a117f-1455">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="a117f-1455">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a117f-1456">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-1456">Az.Accounts</span></span>
* <span data-ttu-id="a117f-1457">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="a117f-1457">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a117f-1458">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1458">Az.AnalysisServices</span></span>
* <span data-ttu-id="a117f-1459">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="a117f-1459">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="a117f-1460">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="a117f-1460">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a117f-1461">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a117f-1461">Az.Automation</span></span>
* <span data-ttu-id="a117f-1462">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="a117f-1462">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="a117f-1463">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="a117f-1463">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="a117f-1464">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="a117f-1464">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-1465">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1465">Az.Compute</span></span>
* <span data-ttu-id="a117f-1466">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-1466">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="a117f-1467">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="a117f-1467">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="a117f-1468">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a117f-1468">Az.ContainerInstance</span></span>
* <span data-ttu-id="a117f-1469">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="a117f-1469">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a117f-1470">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a117f-1470">Az.DataFactory</span></span>
* <span data-ttu-id="a117f-1471">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="a117f-1471">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="a117f-1472">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a117f-1472">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-1473">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-1473">Az.Resources</span></span>
* <span data-ttu-id="a117f-1474">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="a117f-1474">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="a117f-1475">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="a117f-1475">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="a117f-1476">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="a117f-1476">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="a117f-1477">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="a117f-1477">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="a117f-1478">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="a117f-1478">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="a117f-1479">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="a117f-1479">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-1480">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-1480">Az.Sql</span></span>
* <span data-ttu-id="a117f-1481">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="a117f-1481">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-1482">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-1482">Az.Storage</span></span>
* <span data-ttu-id="a117f-1483">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="a117f-1483">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="a117f-1484">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="a117f-1484">New-AzStorageContext</span></span>
* <span data-ttu-id="a117f-1485">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="a117f-1485">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="a117f-1486">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="a117f-1486">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="a117f-1487">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="a117f-1487">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="a117f-1488">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="a117f-1488">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="a117f-1489">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="a117f-1489">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="a117f-1490">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="a117f-1490">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="a117f-1491">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="a117f-1491">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="a117f-1492">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="a117f-1492">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="a117f-1493">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="a117f-1493">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="a117f-1494">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="a117f-1494">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="a117f-1495">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-1495">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a117f-1496">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a117f-1496">Highlights since the last major release</span></span>
* <span data-ttu-id="a117f-1497">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="a117f-1497">General availability of `Az` module</span></span>
* <span data-ttu-id="a117f-1498">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="a117f-1498">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="a117f-1499">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="a117f-1499">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="a117f-1500">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1500">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="a117f-1501">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="a117f-1501">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a117f-1502">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a117f-1502">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="a117f-1503">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="a117f-1503">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a117f-1504">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a117f-1504">Az.Automation</span></span>
* <span data-ttu-id="a117f-1505">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="a117f-1505">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="a117f-1506">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="a117f-1506">Dynamic grouping</span></span>
    * <span data-ttu-id="a117f-1507">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="a117f-1507">Pre-Post script</span></span>
    * <span data-ttu-id="a117f-1508">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="a117f-1508">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-1509">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1509">Az.Compute</span></span>
* <span data-ttu-id="a117f-1510">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="a117f-1510">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="a117f-1511">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="a117f-1511">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a117f-1512">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a117f-1512">Az.KeyVault</span></span>
* <span data-ttu-id="a117f-1513">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="a117f-1513">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-1514">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1514">Az.Network</span></span>
* <span data-ttu-id="a117f-1515">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="a117f-1515">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="a117f-1516">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="a117f-1516">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-1517">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1517">Az.RecoveryServices</span></span>
* <span data-ttu-id="a117f-1518">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="a117f-1518">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="a117f-1519">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="a117f-1519">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-1520">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-1520">Az.Resources</span></span>
* <span data-ttu-id="a117f-1521">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="a117f-1521">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="a117f-1522">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="a117f-1522">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-1523">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-1523">Az.Sql</span></span>
* <span data-ttu-id="a117f-1524">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="a117f-1524">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-1525">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-1525">Az.Storage</span></span>
* <span data-ttu-id="a117f-1526">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a117f-1526">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="a117f-1527">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="a117f-1527">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="a117f-1528">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="a117f-1528">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="a117f-1529">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="a117f-1529">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="a117f-1530">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="a117f-1530">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="a117f-1531">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="a117f-1531">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="a117f-1532">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="a117f-1532">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a117f-1533">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-1533">Az.Websites</span></span>
* <span data-ttu-id="a117f-1534">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="a117f-1534">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="a117f-1535">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-1535">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a117f-1536">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-1536">Az.Accounts</span></span>
* <span data-ttu-id="a117f-1537">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="a117f-1537">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="a117f-1538">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-1538">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a117f-1539">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a117f-1539">Az.Automation</span></span>
* <span data-ttu-id="a117f-1540">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="a117f-1540">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="a117f-1541">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="a117f-1541">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="a117f-1542">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="a117f-1542">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a117f-1543">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a117f-1543">Az.Cdn</span></span>
* <span data-ttu-id="a117f-1544">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="a117f-1544">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-1545">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1545">Az.Compute</span></span>
* <span data-ttu-id="a117f-1546">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="a117f-1546">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a117f-1547">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a117f-1547">Az.DataFactory</span></span>
* <span data-ttu-id="a117f-1548">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="a117f-1548">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a117f-1549">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a117f-1549">Az.LogicApp</span></span>
* <span data-ttu-id="a117f-1550">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="a117f-1550">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-1551">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1551">Az.Network</span></span>
* <span data-ttu-id="a117f-1552">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1552">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-1553">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1553">Az.RecoveryServices</span></span>
* <span data-ttu-id="a117f-1554">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="a117f-1554">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="a117f-1555">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="a117f-1555">SDK Update</span></span>
* <span data-ttu-id="a117f-1556">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="a117f-1556">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="a117f-1557">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="a117f-1557">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-1558">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-1558">Az.Resources</span></span>
* <span data-ttu-id="a117f-1559">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="a117f-1559">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="a117f-1560">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="a117f-1560">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="a117f-1561">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="a117f-1561">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="a117f-1562">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="a117f-1562">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="a117f-1563">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="a117f-1563">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="a117f-1564">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="a117f-1564">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-1565">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-1565">Az.Sql</span></span>
* <span data-ttu-id="a117f-1566">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="a117f-1566">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="a117f-1567">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="a117f-1567">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-1568">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-1568">Az.Storage</span></span>
* <span data-ttu-id="a117f-1569">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-1569">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="a117f-1570">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-1570">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="a117f-1571">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1571">Az.AnalysisServices</span></span>
* <span data-ttu-id="a117f-1572">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="a117f-1572">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a117f-1573">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a117f-1573">Az.Automation</span></span>
* <span data-ttu-id="a117f-1574">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="a117f-1574">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="a117f-1575">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="a117f-1575">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="a117f-1576">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="a117f-1576">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a117f-1577">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1577">Az.CognitiveServices</span></span>
* <span data-ttu-id="a117f-1578">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="a117f-1578">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-1579">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1579">Az.Compute</span></span>
* <span data-ttu-id="a117f-1580">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="a117f-1580">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="a117f-1581">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="a117f-1581">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="a117f-1582">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="a117f-1582">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="a117f-1583">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="a117f-1583">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a117f-1584">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a117f-1584">Az.DataLakeStore</span></span>
* <span data-ttu-id="a117f-1585">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="a117f-1585">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a117f-1586">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a117f-1586">Az.EventHub</span></span>
* <span data-ttu-id="a117f-1587">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="a117f-1587">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="a117f-1588">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a117f-1588">Az.KeyVault</span></span>
* <span data-ttu-id="a117f-1589">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="a117f-1589">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a117f-1590">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a117f-1590">Az.LogicApp</span></span>
* <span data-ttu-id="a117f-1591">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="a117f-1591">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="a117f-1592">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="a117f-1592">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="a117f-1593">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="a117f-1593">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="a117f-1594">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a117f-1594">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="a117f-1595">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a117f-1595">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="a117f-1596">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a117f-1596">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="a117f-1597">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a117f-1597">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="a117f-1598">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="a117f-1598">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="a117f-1599">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a117f-1599">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="a117f-1600">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a117f-1600">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="a117f-1601">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a117f-1601">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="a117f-1602">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a117f-1602">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="a117f-1603">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="a117f-1603">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a117f-1604">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a117f-1604">Az.Monitor</span></span>
* <span data-ttu-id="a117f-1605">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="a117f-1605">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-1606">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1606">Az.Network</span></span>
* <span data-ttu-id="a117f-1607">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="a117f-1607">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a117f-1608">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a117f-1608">Az.OperationalInsights</span></span>
* <span data-ttu-id="a117f-1609">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="a117f-1609">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="a117f-1610">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a117f-1610">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="a117f-1611">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="a117f-1611">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="a117f-1612">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-1612">Az.Resources</span></span>
* <span data-ttu-id="a117f-1613">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="a117f-1613">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="a117f-1614">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="a117f-1614">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="a117f-1615">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="a117f-1615">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="a117f-1616">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="a117f-1616">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-1617">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-1617">Az.Sql</span></span>
* <span data-ttu-id="a117f-1618">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="a117f-1618">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="a117f-1619">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="a117f-1619">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a117f-1620">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-1620">Az.Websites</span></span>
* <span data-ttu-id="a117f-1621">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="a117f-1621">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="a117f-1622">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-1622">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a117f-1623">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-1623">Az.Accounts</span></span>
* <span data-ttu-id="a117f-1624">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="a117f-1624">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a117f-1625">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1625">Az.AnalysisServices</span></span>
<span data-ttu-id="a117f-1626">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="a117f-1626">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-1627">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1627">Az.Compute</span></span>
* <span data-ttu-id="a117f-1628">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="a117f-1628">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="a117f-1629">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="a117f-1629">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="a117f-1630">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="a117f-1630">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-1631">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1631">Az.RecoveryServices</span></span>
<span data-ttu-id="a117f-1632">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="a117f-1632">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-1633">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-1633">Az.Resources</span></span>
* <span data-ttu-id="a117f-1634">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="a117f-1634">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="a117f-1635">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="a117f-1635">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="a117f-1636">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="a117f-1636">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="a117f-1637">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="a117f-1637">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-1638">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-1638">Az.Sql</span></span>
* <span data-ttu-id="a117f-1639">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="a117f-1639">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="a117f-1640">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="a117f-1640">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="a117f-1641">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="a117f-1641">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="a117f-1642">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-1642">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a117f-1643">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-1643">Az.Accounts</span></span>
* <span data-ttu-id="a117f-1644">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="a117f-1644">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a117f-1645">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1645">Az.AnalysisServices</span></span>
* <span data-ttu-id="a117f-1646">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="a117f-1646">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-1647">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1647">Az.RecoveryServices</span></span>
* <span data-ttu-id="a117f-1648">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="a117f-1648">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="a117f-1649">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-1649">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a117f-1650">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-1650">Az.Accounts</span></span>
* <span data-ttu-id="a117f-1651">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="a117f-1651">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a117f-1652">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a117f-1652">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a117f-1653">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="a117f-1653">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="a117f-1654">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="a117f-1654">Az.Aks</span></span>
* <span data-ttu-id="a117f-1655">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a117f-1655">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a117f-1656">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a117f-1656">Az.Automation</span></span>
* <span data-ttu-id="a117f-1657">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="a117f-1657">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="a117f-1658">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a117f-1658">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a117f-1659">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a117f-1659">Az.Cdn</span></span>
* <span data-ttu-id="a117f-1660">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a117f-1660">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-1661">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1661">Az.Compute</span></span>
* <span data-ttu-id="a117f-1662">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="a117f-1662">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="a117f-1663">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a117f-1663">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="a117f-1664">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="a117f-1664">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="a117f-1665">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="a117f-1665">Az.ContainerRegistry</span></span>
* <span data-ttu-id="a117f-1666">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a117f-1666">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a117f-1667">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a117f-1667">Az.DataFactory</span></span>
* <span data-ttu-id="a117f-1668">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="a117f-1668">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a117f-1669">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a117f-1669">Az.DataLakeStore</span></span>
* <span data-ttu-id="a117f-1670">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="a117f-1670">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="a117f-1671">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="a117f-1671">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="a117f-1672">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a117f-1672">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a117f-1673">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a117f-1673">Az.IotHub</span></span>
* <span data-ttu-id="a117f-1674">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="a117f-1674">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a117f-1675">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a117f-1675">Az.KeyVault</span></span>
* <span data-ttu-id="a117f-1676">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a117f-1676">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-1677">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1677">Az.Network</span></span>
* <span data-ttu-id="a117f-1678">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a117f-1678">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-1679">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-1679">Az.Resources</span></span>
* <span data-ttu-id="a117f-1680">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="a117f-1680">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="a117f-1681">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="a117f-1681">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="a117f-1682">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="a117f-1682">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="a117f-1683">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="a117f-1683">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="a117f-1684">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="a117f-1684">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="a117f-1685">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="a117f-1685">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="a117f-1686">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="a117f-1686">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a117f-1687">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a117f-1687">Az.ServiceFabric</span></span>
* <span data-ttu-id="a117f-1688">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="a117f-1688">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="a117f-1689">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="a117f-1689">Fix some error messages.</span></span>
* <span data-ttu-id="a117f-1690">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="a117f-1690">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="a117f-1691">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="a117f-1691">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="a117f-1692">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="a117f-1692">Az.SignalR</span></span>
* <span data-ttu-id="a117f-1693">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a117f-1693">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-1694">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-1694">Az.Sql</span></span>
* <span data-ttu-id="a117f-1695">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a117f-1695">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a117f-1696">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="a117f-1696">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="a117f-1697">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="a117f-1697">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="a117f-1698">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="a117f-1698">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-1699">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-1699">Az.Storage</span></span>
* <span data-ttu-id="a117f-1700">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a117f-1700">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a117f-1701">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="a117f-1701">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="a117f-1702">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="a117f-1702">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="a117f-1703">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="a117f-1703">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="a117f-1704">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a117f-1704">Az.TrafficManager</span></span>
* <span data-ttu-id="a117f-1705">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a117f-1705">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a117f-1706">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-1706">Az.Websites</span></span>
* <span data-ttu-id="a117f-1707">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a117f-1707">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a117f-1708">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="a117f-1708">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="a117f-1709">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="a117f-1709">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="a117f-1710">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a117f-1710">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a117f-1711">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-1711">Az.Accounts</span></span>
* <span data-ttu-id="a117f-1712">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="a117f-1712">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-1713">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1713">Az.Compute</span></span>
* <span data-ttu-id="a117f-1714">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="a117f-1714">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="a117f-1715">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="a117f-1715">Updated the description of ID in help files</span></span>
* <span data-ttu-id="a117f-1716">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-1716">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a117f-1717">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a117f-1717">Az.DataLakeStore</span></span>
* <span data-ttu-id="a117f-1718">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="a117f-1718">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="a117f-1719">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="a117f-1719">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="a117f-1720">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a117f-1720">Az.EventGrid</span></span>
* <span data-ttu-id="a117f-1721">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="a117f-1721">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="a117f-1722">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="a117f-1722">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="a117f-1723">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="a117f-1723">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="a117f-1724">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="a117f-1724">Event Time-To-Live,</span></span>
        - <span data-ttu-id="a117f-1725">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="a117f-1725">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="a117f-1726">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="a117f-1726">Dead letter endpoint.</span></span>
    - <span data-ttu-id="a117f-1727">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="a117f-1727">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="a117f-1728">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="a117f-1728">Event Time-To-Live,</span></span>
        - <span data-ttu-id="a117f-1729">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="a117f-1729">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="a117f-1730">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="a117f-1730">Dead letter endpoint.</span></span>
* <span data-ttu-id="a117f-1731">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="a117f-1731">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="a117f-1732">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="a117f-1732">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a117f-1733">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a117f-1733">Az.IotHub</span></span>
* <span data-ttu-id="a117f-1734">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="a117f-1734">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a117f-1735">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a117f-1735">Az.LogicApp</span></span>
* <span data-ttu-id="a117f-1736">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="a117f-1736">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-1737">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-1737">Az.Resources</span></span>
* <span data-ttu-id="a117f-1738">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="a117f-1738">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="a117f-1739">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="a117f-1739">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="a117f-1740">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="a117f-1740">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="a117f-1741">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="a117f-1741">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="a117f-1742">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="a117f-1742">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="a117f-1743">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="a117f-1743">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="a117f-1744">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="a117f-1744">Az.SignalR</span></span>
* <span data-ttu-id="a117f-1745">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-1745">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-1746">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-1746">Az.Sql</span></span>
* <span data-ttu-id="a117f-1747">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="a117f-1747">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a117f-1748">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-1748">Az.Storage</span></span>
* <span data-ttu-id="a117f-1749">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="a117f-1749">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="a117f-1750">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="a117f-1750">New-AzStorageContext</span></span>
* <span data-ttu-id="a117f-1751">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="a117f-1751">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="a117f-1752">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="a117f-1752">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a117f-1753">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-1753">Az.Websites</span></span>
* <span data-ttu-id="a117f-1754">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="a117f-1754">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="a117f-1755">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-1755">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="a117f-1756">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a117f-1756">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="a117f-1757">Geral</span><span class="sxs-lookup"><span data-stu-id="a117f-1757">General</span></span>

- <span data-ttu-id="a117f-1758">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="a117f-1758">General Availability of Az Module</span></span>
- <span data-ttu-id="a117f-1759">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="a117f-1759">Online help for each module</span></span>
- <span data-ttu-id="a117f-1760">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="a117f-1760">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="a117f-1761">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="a117f-1761">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="a117f-1762">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-1762">Az.Accounts</span></span>
- <span data-ttu-id="a117f-1763">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a117f-1763">Changed from Az.Profile</span></span>
- <span data-ttu-id="a117f-1764">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="a117f-1764">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="a117f-1765">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a117f-1765">Az.ApiManagement</span></span>
- <span data-ttu-id="a117f-1766">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="a117f-1766">Fixes for #7002</span></span>
- <span data-ttu-id="a117f-1767">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a117f-1767">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="a117f-1768">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a117f-1768">Az.Batch</span></span>
- <span data-ttu-id="a117f-1769">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="a117f-1769">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="a117f-1770">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="a117f-1770">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="a117f-1771">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a117f-1771">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="a117f-1772">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="a117f-1772">Az.Billing</span></span>
- <span data-ttu-id="a117f-1773">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a117f-1773">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="a117f-1774">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1774">Az.CognitivServices</span></span>
- <span data-ttu-id="a117f-1775">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-1775">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="a117f-1776">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="a117f-1776">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="a117f-1777">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a117f-1777">Az.ContainerInstance</span></span>
- <span data-ttu-id="a117f-1778">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="a117f-1778">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="a117f-1779">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="a117f-1779">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="a117f-1780">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a117f-1780">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="a117f-1781">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a117f-1781">Az.DataLakeStore</span></span>
- <span data-ttu-id="a117f-1782">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a117f-1782">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="a117f-1783">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a117f-1783">Az.Monitor</span></span>
- <span data-ttu-id="a117f-1784">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a117f-1784">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="a117f-1785">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a117f-1785">Az.KeyVault</span></span>
- <span data-ttu-id="a117f-1786">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="a117f-1786">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="a117f-1787">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="a117f-1787">Az.MachineLearning</span></span>
- <span data-ttu-id="a117f-1788">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="a117f-1788">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="a117f-1789">Az.Media</span><span class="sxs-lookup"><span data-stu-id="a117f-1789">Az.Media</span></span>
- <span data-ttu-id="a117f-1790">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="a117f-1790">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="a117f-1791">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1791">Az.Network</span></span>
<span data-ttu-id="a117f-1792">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="a117f-1792">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="a117f-1793">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a117f-1793">New cmdlets added:</span></span>
        - <span data-ttu-id="a117f-1794">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a117f-1794">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a117f-1795">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a117f-1795">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a117f-1796">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a117f-1796">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a117f-1797">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a117f-1797">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a117f-1798">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a117f-1798">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a117f-1799">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="a117f-1799">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="a117f-1800">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="a117f-1800">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="a117f-1801">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="a117f-1801">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="a117f-1802">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a117f-1802">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="a117f-1803">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="a117f-1803">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="a117f-1804">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="a117f-1804">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="a117f-1805">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="a117f-1805">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="a117f-1806">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-1806">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="a117f-1807">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-1807">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="a117f-1808">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="a117f-1808">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="a117f-1809">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="a117f-1809">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="a117f-1810">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="a117f-1810">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="a117f-1811">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="a117f-1811">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="a117f-1812">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="a117f-1812">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="a117f-1813">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="a117f-1813">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="a117f-1814">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a117f-1814">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="a117f-1815">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a117f-1815">Az.OperationalInsights</span></span>
- <span data-ttu-id="a117f-1816">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a117f-1816">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="a117f-1817">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a117f-1817">Az.Profile</span></span>
- <span data-ttu-id="a117f-1818">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a117f-1818">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-1819">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1819">Az.RecoveryServices</span></span>
- <span data-ttu-id="a117f-1820">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a117f-1820">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="a117f-1821">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-1821">Az.Resources</span></span>
- <span data-ttu-id="a117f-1822">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a117f-1822">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="a117f-1823">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a117f-1823">Az.ServiceFabric</span></span>
- <span data-ttu-id="a117f-1824">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="a117f-1824">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="a117f-1825">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a117f-1825">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="a117f-1826">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="a117f-1826">Az.SIgnalR</span></span>
- <span data-ttu-id="a117f-1827">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="a117f-1827">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="a117f-1828">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-1828">Az.Sql</span></span>
- <span data-ttu-id="a117f-1829">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="a117f-1829">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="a117f-1830">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="a117f-1830">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="a117f-1831">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a117f-1831">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="a117f-1832">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-1832">Az.Storage</span></span>
- <span data-ttu-id="a117f-1833">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a117f-1833">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="a117f-1834">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-1834">Az.Websites</span></span>
- <span data-ttu-id="a117f-1835">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a117f-1835">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="a117f-1836">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a117f-1836">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="a117f-1837">Geral</span><span class="sxs-lookup"><span data-stu-id="a117f-1837">General</span></span>

* <span data-ttu-id="a117f-1838">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="a117f-1838">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="a117f-1839">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1839">Az.Compute</span></span>

* <span data-ttu-id="a117f-1840">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="a117f-1840">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="a117f-1841">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a117f-1841">Az.DataLakeStore</span></span>

* <span data-ttu-id="a117f-1842">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="a117f-1842">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="a117f-1843">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a117f-1843">Az.FrontDoor</span></span>

* <span data-ttu-id="a117f-1844">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="a117f-1844">Fixed some broken links</span></span>
    - <span data-ttu-id="a117f-1845">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="a117f-1845">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="a117f-1846">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="a117f-1846">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="a117f-1847">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1847">Az.RecoveryServices</span></span>

* <span data-ttu-id="a117f-1848">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-1848">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="a117f-1849">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="a117f-1849">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="a117f-1850">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-1850">Az.Resources</span></span>

* <span data-ttu-id="a117f-1851">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="a117f-1851">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="a117f-1852">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="a117f-1852">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="a117f-1853">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-1853">Az.Sql</span></span>

* <span data-ttu-id="a117f-1854">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="a117f-1854">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="a117f-1855">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="a117f-1855">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="a117f-1856">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="a117f-1856">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="a117f-1857">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-1857">Az.Storage</span></span>

* <span data-ttu-id="a117f-1858">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a117f-1858">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="a117f-1859">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="a117f-1859">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="a117f-1860">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="a117f-1860">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="a117f-1861">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="a117f-1861">Support Static Website configuration</span></span>
    - <span data-ttu-id="a117f-1862">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="a117f-1862">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="a117f-1863">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="a117f-1863">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="a117f-1864">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-1864">Az.Websites</span></span>

* <span data-ttu-id="a117f-1865">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="a117f-1865">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="a117f-1866">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="a117f-1866">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="a117f-1867">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-1867">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="a117f-1868">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a117f-1868">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="a117f-1869">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a117f-1869">Az.ApiManagement</span></span>
* <span data-ttu-id="a117f-1870">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a117f-1870">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="a117f-1871">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a117f-1871">Az.Automation</span></span>
* <span data-ttu-id="a117f-1872">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="a117f-1872">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="a117f-1873">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="a117f-1873">Added Update Management cmdlets</span></span>
* <span data-ttu-id="a117f-1874">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="a117f-1874">Added Source Control cmdlets</span></span>
* <span data-ttu-id="a117f-1875">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="a117f-1875">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="a117f-1876">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="a117f-1876">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="a117f-1877">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1877">Az.Compute</span></span>
* <span data-ttu-id="a117f-1878">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="a117f-1878">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="a117f-1879">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a117f-1879">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="a117f-1880">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a117f-1880">Az.ContainerInstance</span></span>
* <span data-ttu-id="a117f-1881">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a117f-1881">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="a117f-1882">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="a117f-1882">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="a117f-1883">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="a117f-1883">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="a117f-1884">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1884">Az.Network</span></span>
* <span data-ttu-id="a117f-1885">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="a117f-1885">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="a117f-1886">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="a117f-1886">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="a117f-1887">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="a117f-1887">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="a117f-1888">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="a117f-1888">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="a117f-1889">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="a117f-1889">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="a117f-1890">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="a117f-1890">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="a117f-1891">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="a117f-1891">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="a117f-1892">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="a117f-1892">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="a117f-1893">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="a117f-1893">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="a117f-1894">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a117f-1894">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="a117f-1895">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="a117f-1895">Az.Relay</span></span>
* <span data-ttu-id="a117f-1896">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="a117f-1896">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="a117f-1897">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-1897">Az.Resources</span></span>
* <span data-ttu-id="a117f-1898">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="a117f-1898">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="a117f-1899">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="a117f-1899">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="a117f-1900">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="a117f-1900">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="a117f-1901">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a117f-1901">Az.ServiceFabric</span></span>
* <span data-ttu-id="a117f-1902">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="a117f-1902">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="a117f-1903">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-1903">Az.Sql</span></span>
* <span data-ttu-id="a117f-1904">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="a117f-1904">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="a117f-1905">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a117f-1905">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a117f-1906">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a117f-1906">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a117f-1907">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a117f-1907">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a117f-1908">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a117f-1908">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a117f-1909">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a117f-1909">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="a117f-1910">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a117f-1910">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="a117f-1911">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a117f-1911">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="a117f-1912">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a117f-1912">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="a117f-1913">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="a117f-1913">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="a117f-1914">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="a117f-1914">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="a117f-1915">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="a117f-1915">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="a117f-1916">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="a117f-1916">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="a117f-1917">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="a117f-1917">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="a117f-1918">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="a117f-1918">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="a117f-1919">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="a117f-1919">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="a117f-1920">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="a117f-1920">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="a117f-1921">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a117f-1921">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="a117f-1922">Geral</span><span class="sxs-lookup"><span data-stu-id="a117f-1922">General</span></span>
* <span data-ttu-id="a117f-1923">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="a117f-1923">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="a117f-1924">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a117f-1924">Az.Profile</span></span>
* <span data-ttu-id="a117f-1925">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="a117f-1925">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="a117f-1926">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="a117f-1926">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="a117f-1927">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="a117f-1927">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="a117f-1928">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="a117f-1928">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="a117f-1929">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="a117f-1929">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="a117f-1930">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="a117f-1930">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="a117f-1931">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="a117f-1931">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="a117f-1932">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1932">Az.CognitiveServices</span></span>
* <span data-ttu-id="a117f-1933">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="a117f-1933">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-1934">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1934">Az.Compute</span></span>
* <span data-ttu-id="a117f-1935">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="a117f-1935">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="a117f-1936">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="a117f-1936">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="a117f-1937">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="a117f-1937">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a117f-1938">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a117f-1938">Az.DataLakeStore</span></span>
* <span data-ttu-id="a117f-1939">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="a117f-1939">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="a117f-1940">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="a117f-1940">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="a117f-1941">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="a117f-1941">Az.Insights</span></span>
* <span data-ttu-id="a117f-1942">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="a117f-1942">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="a117f-1943">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="a117f-1943">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="a117f-1944">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="a117f-1944">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="a117f-1945">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="a117f-1945">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-1946">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1946">Az.Network</span></span>
* <span data-ttu-id="a117f-1947">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="a117f-1947">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="a117f-1948">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="a117f-1948">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="a117f-1949">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="a117f-1949">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="a117f-1950">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="a117f-1950">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="a117f-1951">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="a117f-1951">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="a117f-1952">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="a117f-1952">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="a117f-1953">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="a117f-1953">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a117f-1954">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a117f-1954">Az.PolicyInsights</span></span>
* <span data-ttu-id="a117f-1955">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="a117f-1955">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-1956">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-1956">Az.Resources</span></span>
* <span data-ttu-id="a117f-1957">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="a117f-1957">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="a117f-1958">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="a117f-1958">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a117f-1959">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a117f-1959">Az.ServiceBus</span></span>
* <span data-ttu-id="a117f-1960">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="a117f-1960">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a117f-1961">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a117f-1961">Az.ServiceFabric</span></span>
* <span data-ttu-id="a117f-1962">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="a117f-1962">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="a117f-1963">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="a117f-1963">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="a117f-1964">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="a117f-1964">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="a117f-1965">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="a117f-1965">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="a117f-1966">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="a117f-1966">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="a117f-1967">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="a117f-1967">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="a117f-1968">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a117f-1968">Az.Profile</span></span>
* <span data-ttu-id="a117f-1969">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="a117f-1969">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="a117f-1970">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="a117f-1970">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-1971">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1971">Az.Compute</span></span>
* <span data-ttu-id="a117f-1972">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="a117f-1972">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="a117f-1973">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="a117f-1973">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a117f-1974">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a117f-1974">Az.DataLakeStore</span></span>
* <span data-ttu-id="a117f-1975">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="a117f-1975">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="a117f-1976">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-1976">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="a117f-1977">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="a117f-1977">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="a117f-1978">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="a117f-1978">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="a117f-1979">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="a117f-1979">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-1980">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-1980">Az.Network</span></span>
* <span data-ttu-id="a117f-1981">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="a117f-1981">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="a117f-1982">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="a117f-1982">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-1983">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-1983">Az.Resources</span></span>
* <span data-ttu-id="a117f-1984">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="a117f-1984">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="a117f-1985">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="a117f-1985">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="a117f-1986">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="a117f-1986">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="a117f-1987">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="a117f-1987">Azure.Storage</span></span>
* <span data-ttu-id="a117f-1988">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="a117f-1988">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="a117f-1989">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="a117f-1989">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="a117f-1990">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="a117f-1990">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="a117f-1991">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="a117f-1991">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="a117f-1992">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="a117f-1992">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="a117f-1993">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a117f-1993">Az.CognitiveServices</span></span>
* <span data-ttu-id="a117f-1994">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="a117f-1994">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a117f-1995">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a117f-1995">Az.Compute</span></span>
* <span data-ttu-id="a117f-1996">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="a117f-1996">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="a117f-1997">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="a117f-1997">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="a117f-1998">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="a117f-1998">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="a117f-1999">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="a117f-1999">Az.DataFactoryV2</span></span>
* <span data-ttu-id="a117f-2000">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="a117f-2000">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a117f-2001">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a117f-2001">Az.Network</span></span>
* <span data-ttu-id="a117f-2002">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="a117f-2002">Added NetworkProfile functionality.</span></span> <span data-ttu-id="a117f-2003">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="a117f-2003">new cmdlets added</span></span>
    - <span data-ttu-id="a117f-2004">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a117f-2004">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="a117f-2005">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a117f-2005">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="a117f-2006">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a117f-2006">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="a117f-2007">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a117f-2007">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="a117f-2008">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-2008">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="a117f-2009">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-2009">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="a117f-2010">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="a117f-2010">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="a117f-2011">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="a117f-2011">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="a117f-2012">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="a117f-2012">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="a117f-2013">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="a117f-2013">Az.RedisCache</span></span>
* <span data-ttu-id="a117f-2014">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="a117f-2014">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="a117f-2015">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="a117f-2015">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="a117f-2016">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a117f-2016">Az.Resources</span></span>
* <span data-ttu-id="a117f-2017">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="a117f-2017">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="a117f-2018">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="a117f-2018">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="a117f-2019">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a117f-2019">Az.Sql</span></span>
* <span data-ttu-id="a117f-2020">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="a117f-2020">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a117f-2021">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a117f-2021">Az.Websites</span></span>
* <span data-ttu-id="a117f-2022">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="a117f-2022">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="a117f-2023">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="a117f-2023">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="a117f-2024">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a117f-2024">0.2.0 - September 2018</span></span>
 <span data-ttu-id="a117f-2025">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="a117f-2025">Initial Release</span></span>
