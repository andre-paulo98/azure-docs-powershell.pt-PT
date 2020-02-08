---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/09/2020
ms.openlocfilehash: 694439934afb41b465a89188d59bc964db3c0032
ms.sourcegitcommit: 9181f20c2c5eaa271150de9e25b9cb30ba5e6cb0
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/04/2020
ms.locfileid: "77002678"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="d454a-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="d454a-103">Azure PowerShell release notes</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="d454a-104">3.4.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="d454a-104">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="d454a-105">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="d454a-105">Highlights since the last major release</span></span>
* <span data-ttu-id="d454a-106">Versão inicial Az.CosmosDB 0.1.0 lançada</span><span class="sxs-lookup"><span data-stu-id="d454a-106">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="d454a-107">Foi adicionado suporte para Az.Network ConnectionMonitor V2</span><span class="sxs-lookup"><span data-stu-id="d454a-107">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="d454a-108">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-108">Az.Accounts</span></span>
* <span data-ttu-id="d454a-109">Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível</span><span class="sxs-lookup"><span data-stu-id="d454a-109">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="d454a-110">Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5</span><span class="sxs-lookup"><span data-stu-id="d454a-110">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="d454a-111">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d454a-111">Az.ApiManagement</span></span>
* <span data-ttu-id="d454a-112">**Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="d454a-112">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="d454a-113">**New-AzApiManagementProduct**\* e **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="d454a-113">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="d454a-114">Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472</span><span class="sxs-lookup"><span data-stu-id="d454a-114">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="d454a-115">**Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet</span><span class="sxs-lookup"><span data-stu-id="d454a-115">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-116">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-116">Az.Compute</span></span>
* <span data-ttu-id="d454a-117">Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.</span><span class="sxs-lookup"><span data-stu-id="d454a-117">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="d454a-118">Foi adicionado o cmdlet Update-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="d454a-118">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="d454a-119">Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d454a-119">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="d454a-120">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-120">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="d454a-121">Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="d454a-121">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="d454a-122">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="d454a-122">Az.DataFactory</span></span>
* <span data-ttu-id="d454a-123">Atualização do SDK .NET do ADF para a versão 4.7.0</span><span class="sxs-lookup"><span data-stu-id="d454a-123">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="d454a-124">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="d454a-124">Az.DeploymentManager</span></span>
* <span data-ttu-id="d454a-125">Adiciona operações LIST para os recursos</span><span class="sxs-lookup"><span data-stu-id="d454a-125">Adds LIST operations for resources</span></span>
* <span data-ttu-id="d454a-126">Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="d454a-126">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="d454a-127">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="d454a-127">Az.HDInsight</span></span>
* <span data-ttu-id="d454a-128">Foi corrigido o erro do documento de New-AzHDInsightCluster.</span><span class="sxs-lookup"><span data-stu-id="d454a-128">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="d454a-129">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d454a-129">Az.KeyVault</span></span>
* <span data-ttu-id="d454a-130">Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.</span><span class="sxs-lookup"><span data-stu-id="d454a-130">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-131">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-131">Az.Network</span></span>
* <span data-ttu-id="d454a-132">Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="d454a-132">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="d454a-133">Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão</span><span class="sxs-lookup"><span data-stu-id="d454a-133">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="d454a-134">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="d454a-134">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="d454a-135">Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="d454a-135">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="d454a-136">Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"</span><span class="sxs-lookup"><span data-stu-id="d454a-136">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="d454a-137">Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.</span><span class="sxs-lookup"><span data-stu-id="d454a-137">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="d454a-138">Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d454a-138">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="d454a-139">Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="d454a-139">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="d454a-140">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d454a-140">New cmdlets added:</span></span>
        - <span data-ttu-id="d454a-141">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="d454a-141">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="d454a-142">Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="d454a-142">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="d454a-143">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="d454a-143">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="d454a-144">Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2</span><span class="sxs-lookup"><span data-stu-id="d454a-144">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="d454a-145">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="d454a-145">Az.PolicyInsights</span></span>
* <span data-ttu-id="d454a-146">Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar</span><span class="sxs-lookup"><span data-stu-id="d454a-146">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="d454a-147">Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation</span><span class="sxs-lookup"><span data-stu-id="d454a-147">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="d454a-148">Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política</span><span class="sxs-lookup"><span data-stu-id="d454a-148">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="d454a-149">Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="d454a-149">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-150">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-150">Az.RecoveryServices</span></span>
* <span data-ttu-id="d454a-151">Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.</span><span class="sxs-lookup"><span data-stu-id="d454a-151">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="d454a-152">O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.</span><span class="sxs-lookup"><span data-stu-id="d454a-152">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-153">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-153">Az.Resources</span></span>
* <span data-ttu-id="d454a-154">-Scope foi tornado opcional nos cmdlets \*-AzPolicyAssignment com subscrição de contexto predefinida</span><span class="sxs-lookup"><span data-stu-id="d454a-154">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="d454a-155">Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves</span><span class="sxs-lookup"><span data-stu-id="d454a-155">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-156">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-156">Az.Sql</span></span>
<span data-ttu-id="d454a-157">Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.</span><span class="sxs-lookup"><span data-stu-id="d454a-157">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-158">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-158">Az.Storage</span></span>
* <span data-ttu-id="d454a-159">Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d454a-159">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="d454a-160">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-160">New-AzStorageAccount</span></span>
* <span data-ttu-id="d454a-161">Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation</span><span class="sxs-lookup"><span data-stu-id="d454a-161">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="d454a-162">Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="d454a-162">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="d454a-163">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-163">Az.Websites</span></span>
* <span data-ttu-id="d454a-164">Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState</span><span class="sxs-lookup"><span data-stu-id="d454a-164">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="d454a-165">Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido</span><span class="sxs-lookup"><span data-stu-id="d454a-165">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="d454a-166">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="d454a-166">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="d454a-167">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-167">Az.Accounts</span></span>
* <span data-ttu-id="d454a-168">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="d454a-168">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="d454a-169">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="d454a-169">Az.Cdn</span></span>
* <span data-ttu-id="d454a-170">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="d454a-170">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-171">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-171">Az.Compute</span></span>
* <span data-ttu-id="d454a-172">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="d454a-172">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="d454a-173">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="d454a-173">Az.ContainerInstance</span></span>
* <span data-ttu-id="d454a-174">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="d454a-174">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="d454a-175">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="d454a-175">Az.DataBoxEdge</span></span>
* <span data-ttu-id="d454a-176">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="d454a-176">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="d454a-177">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="d454a-177">Get the Edge Storage Container</span></span>
* <span data-ttu-id="d454a-178">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="d454a-178">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="d454a-179">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="d454a-179">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="d454a-180">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="d454a-180">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="d454a-181">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="d454a-181">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="d454a-182">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="d454a-182">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="d454a-183">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="d454a-183">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="d454a-184">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="d454a-184">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="d454a-185">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="d454a-185">Get the Edge Storage Account</span></span>
* <span data-ttu-id="d454a-186">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="d454a-186">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="d454a-187">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="d454a-187">Create new Edge Storage Account</span></span>
* <span data-ttu-id="d454a-188">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="d454a-188">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="d454a-189">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="d454a-189">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="d454a-190">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="d454a-190">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="d454a-191">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="d454a-191">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="d454a-192">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="d454a-192">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="d454a-193">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="d454a-193">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="d454a-194">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="d454a-194">Az.DataFactory</span></span>
* <span data-ttu-id="d454a-195">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="d454a-195">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="d454a-196">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="d454a-196">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="d454a-197">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="d454a-197">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="d454a-198">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="d454a-198">Az.DevTestLabs</span></span>
* <span data-ttu-id="d454a-199">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="d454a-199">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="d454a-200">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="d454a-200">Az.EventHub</span></span>
* <span data-ttu-id="d454a-201">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="d454a-201">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="d454a-202">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="d454a-202">Az.HDInsight</span></span>
* <span data-ttu-id="d454a-203">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="d454a-203">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="d454a-204">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="d454a-204">Az.MachineLearning</span></span>
* <span data-ttu-id="d454a-205">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="d454a-205">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="d454a-206">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="d454a-206">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="d454a-207">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="d454a-207">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="d454a-208">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="d454a-208">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="d454a-209">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="d454a-209">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="d454a-210">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="d454a-210">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="d454a-211">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="d454a-211">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="d454a-212">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="d454a-212">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-213">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-213">Az.Network</span></span>
* <span data-ttu-id="d454a-214">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="d454a-214">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-215">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-215">Az.RecoveryServices</span></span>
* <span data-ttu-id="d454a-216">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-216">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="d454a-217">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-217">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="d454a-218">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-218">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="d454a-219">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-219">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-220">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-220">Az.Resources</span></span>
* <span data-ttu-id="d454a-221">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="d454a-221">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-222">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-222">Az.Sql</span></span>
* <span data-ttu-id="d454a-223">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="d454a-223">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="d454a-224">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="d454a-224">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="d454a-225">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="d454a-225">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="d454a-226">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="d454a-226">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-227">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-227">Az.Storage</span></span>
* <span data-ttu-id="d454a-228">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="d454a-228">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="d454a-229">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="d454a-229">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="d454a-230">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="d454a-230">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span> 
    - <span data-ttu-id="d454a-231">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-231">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="d454a-232">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-232">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="d454a-233">Geral</span><span class="sxs-lookup"><span data-stu-id="d454a-233">General</span></span>
* <span data-ttu-id="d454a-234">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="d454a-234">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="d454a-235">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-235">Az.Accounts</span></span>
* <span data-ttu-id="d454a-236">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="d454a-236">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="d454a-237">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="d454a-237">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="d454a-238">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="d454a-238">Az.Batch</span></span>
* <span data-ttu-id="d454a-239">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="d454a-239">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="d454a-240">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="d454a-240">Az.DataFactory</span></span>
* <span data-ttu-id="d454a-241">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="d454a-241">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="d454a-242">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="d454a-242">Az.FrontDoor</span></span>
* <span data-ttu-id="d454a-243">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="d454a-243">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="d454a-244">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="d454a-244">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="d454a-245">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="d454a-245">Az.HealthcareApis</span></span>
* <span data-ttu-id="d454a-246">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="d454a-246">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="d454a-247">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d454a-247">Az.KeyVault</span></span>
* <span data-ttu-id="d454a-248">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="d454a-248">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="d454a-249">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="d454a-249">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="d454a-250">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="d454a-250">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="d454a-251">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="d454a-251">Az.Monitor</span></span>
* <span data-ttu-id="d454a-252">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="d454a-252">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="d454a-253">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="d454a-253">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="d454a-254">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="d454a-254">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-255">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-255">Az.Network</span></span>
* <span data-ttu-id="d454a-256">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="d454a-256">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-257">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-257">Az.Resources</span></span>
* <span data-ttu-id="d454a-258">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="d454a-258">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="d454a-259">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="d454a-259">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-260">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-260">Az.Sql</span></span>
* <span data-ttu-id="d454a-261">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="d454a-261">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-262">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-262">Az.Storage</span></span>
* <span data-ttu-id="d454a-263">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="d454a-263">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="d454a-264">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="d454a-264">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="d454a-265">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="d454a-265">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="d454a-266">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="d454a-266">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="d454a-267">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="d454a-267">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="d454a-268">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="d454a-268">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="d454a-269">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="d454a-269">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span> 
    - <span data-ttu-id="d454a-270">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="d454a-270">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="d454a-271">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="d454a-271">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="d454a-272">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="d454a-272">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="d454a-273">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="d454a-273">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="d454a-274">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="d454a-274">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="d454a-275">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="d454a-275">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="d454a-276">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-276">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="d454a-277">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="d454a-277">Highlights since the last major release</span></span>
* <span data-ttu-id="d454a-278">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="d454a-278">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="d454a-279">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="d454a-279">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-280">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-280">Az.Compute</span></span>
* <span data-ttu-id="d454a-281">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="d454a-281">VM Reapply feature</span></span>
    - <span data-ttu-id="d454a-282">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="d454a-282">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="d454a-283">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="d454a-283">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="d454a-284">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="d454a-284">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="d454a-285">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="d454a-285">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="d454a-286">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="d454a-286">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="d454a-287">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="d454a-287">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="d454a-288">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="d454a-288">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="d454a-289">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="d454a-289">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="d454a-290">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="d454a-290">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="d454a-291">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="d454a-291">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="d454a-292">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="d454a-292">Az.DataBoxEdge</span></span>
* <span data-ttu-id="d454a-293">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="d454a-293">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="d454a-294">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="d454a-294">Get the Order</span></span>
* <span data-ttu-id="d454a-295">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="d454a-295">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="d454a-296">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="d454a-296">Create new Order</span></span>
* <span data-ttu-id="d454a-297">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="d454a-297">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="d454a-298">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="d454a-298">Remove the Order</span></span>
* <span data-ttu-id="d454a-299">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="d454a-299">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="d454a-300">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="d454a-300">Now creates Local Share</span></span>
* <span data-ttu-id="d454a-301">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="d454a-301">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="d454a-302">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="d454a-302">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="d454a-303">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="d454a-303">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="d454a-304">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="d454a-304">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="d454a-305">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="d454a-305">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="d454a-306">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="d454a-306">Gets the information about Triggers</span></span>
* <span data-ttu-id="d454a-307">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="d454a-307">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="d454a-308">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="d454a-308">Create new Triggers</span></span>
* <span data-ttu-id="d454a-309">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="d454a-309">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="d454a-310">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="d454a-310">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="d454a-311">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="d454a-311">Az.DataFactory</span></span>
* <span data-ttu-id="d454a-312">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="d454a-312">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="d454a-313">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="d454a-313">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="d454a-314">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d454a-314">Az.DataLakeStore</span></span>
* <span data-ttu-id="d454a-315">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="d454a-315">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="d454a-316">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="d454a-316">Az.EventHub</span></span>
* <span data-ttu-id="d454a-317">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="d454a-317">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="d454a-318">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="d454a-318">Az.FrontDoor</span></span>
* <span data-ttu-id="d454a-319">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="d454a-319">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="d454a-320">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="d454a-320">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="d454a-321">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="d454a-321">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="d454a-322">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="d454a-322">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-323">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-323">Az.Network</span></span>
* <span data-ttu-id="d454a-324">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="d454a-324">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="d454a-325">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="d454a-325">Az.PrivateDns</span></span>
* <span data-ttu-id="d454a-326">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="d454a-326">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-327">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-327">Az.RecoveryServices</span></span>
* <span data-ttu-id="d454a-328">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="d454a-328">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="d454a-329">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="d454a-329">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="d454a-330">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="d454a-330">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="d454a-331">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="d454a-331">Az.RedisCache</span></span>
* <span data-ttu-id="d454a-332">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="d454a-332">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="d454a-333">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="d454a-333">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="d454a-334">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="d454a-334">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-335">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-335">Az.Resources</span></span>
- <span data-ttu-id="d454a-336">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="d454a-336">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="d454a-337">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="d454a-337">Updated create policy definition help example</span></span>
- <span data-ttu-id="d454a-338">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="d454a-338">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="d454a-339">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="d454a-339">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="d454a-340">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="d454a-340">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-341">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-341">Az.Sql</span></span>
* <span data-ttu-id="d454a-342">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="d454a-342">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="d454a-343">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="d454a-343">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="d454a-344">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-344">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="d454a-345">Geral</span><span class="sxs-lookup"><span data-stu-id="d454a-345">General</span></span>
* <span data-ttu-id="d454a-346">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="d454a-346">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="d454a-347">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-347">Az.Accounts</span></span>
* <span data-ttu-id="d454a-348">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="d454a-348">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="d454a-349">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="d454a-349">Az.Advisor</span></span>
* <span data-ttu-id="d454a-350">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="d454a-350">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="d454a-351">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="d454a-351">Az.Batch</span></span>
* <span data-ttu-id="d454a-352">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="d454a-352">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="d454a-353">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="d454a-353">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="d454a-354">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="d454a-354">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="d454a-355">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="d454a-355">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="d454a-356">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="d454a-356">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="d454a-357">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="d454a-357">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="d454a-358">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="d454a-358">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="d454a-359">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="d454a-359">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="d454a-360">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="d454a-360">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="d454a-361">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="d454a-361">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="d454a-362">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="d454a-362">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="d454a-363">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="d454a-363">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="d454a-364">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="d454a-364">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="d454a-365">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="d454a-365">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="d454a-366">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="d454a-366">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="d454a-367">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="d454a-367">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="d454a-368">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="d454a-368">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="d454a-369">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="d454a-369">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="d454a-370">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="d454a-370">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="d454a-371">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="d454a-371">This operation is no longer supported.</span></span>
* <span data-ttu-id="d454a-372">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="d454a-372">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="d454a-373">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="d454a-373">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="d454a-374">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="d454a-374">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="d454a-375">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="d454a-375">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span> 
  - <span data-ttu-id="d454a-376">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="d454a-376">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="d454a-377">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="d454a-377">New non-verified images are also now returned.</span></span> <span data-ttu-id="d454a-378">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="d454a-378">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="d454a-379">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="d454a-379">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="d454a-380">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="d454a-380">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="d454a-381">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="d454a-381">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="d454a-382">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="d454a-382">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="d454a-383">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="d454a-383">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="d454a-384">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="d454a-384">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="d454a-385">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="d454a-385">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="d454a-386">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="d454a-386">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="d454a-387">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="d454a-387">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="d454a-388">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="d454a-388">Az.Cdn</span></span>
* <span data-ttu-id="d454a-389">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="d454a-389">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="d454a-390">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="d454a-390">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-391">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-391">Az.Compute</span></span>
* <span data-ttu-id="d454a-392">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="d454a-392">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="d454a-393">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="d454a-393">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="d454a-394">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span><span class="sxs-lookup"><span data-stu-id="d454a-394">DiskEncryptionSetId parameter is added to the following cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span></span>        
        <span data-ttu-id="d454a-395">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="d454a-395">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="d454a-396">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-396">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="d454a-397">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-397">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="d454a-398">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="d454a-398">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="d454a-399">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="d454a-399">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="d454a-400">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="d454a-400">Breaking changes</span></span>
    - <span data-ttu-id="d454a-401">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="d454a-401">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="d454a-402">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="d454a-402">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="d454a-403">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="d454a-403">Az.DataFactory</span></span>
* <span data-ttu-id="d454a-404">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="d454a-404">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="d454a-405">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d454a-405">Az.DataLakeStore</span></span>
* <span data-ttu-id="d454a-406">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="d454a-406">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="d454a-407">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="d454a-407">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="d454a-408">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="d454a-408">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="d454a-409">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="d454a-409">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="d454a-410">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="d454a-410">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="d454a-411">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="d454a-411">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="d454a-412">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="d454a-412">Az.FrontDoor</span></span>
* <span data-ttu-id="d454a-413">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="d454a-413">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="d454a-414">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="d454a-414">Az.HDInsight</span></span>
* <span data-ttu-id="d454a-415">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="d454a-415">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="d454a-416">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="d454a-416">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="d454a-417">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="d454a-417">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="d454a-418">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d454a-418">Removed five cmdlets:</span></span>
    - <span data-ttu-id="d454a-419">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="d454a-419">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="d454a-420">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="d454a-420">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="d454a-421">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="d454a-421">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="d454a-422">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="d454a-422">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="d454a-423">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="d454a-423">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="d454a-424">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d454a-424">Added three cmdlets:</span></span>
    - <span data-ttu-id="d454a-425">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="d454a-425">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="d454a-426">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="d454a-426">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="d454a-427">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="d454a-427">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="d454a-428">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="d454a-428">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="d454a-429">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="d454a-429">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="d454a-430">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="d454a-430">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="d454a-431">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d454a-431">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="d454a-432">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="d454a-432">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="d454a-433">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="d454a-433">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="d454a-434">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="d454a-434">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="d454a-435">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="d454a-435">Added some scenario test cases.</span></span>
* <span data-ttu-id="d454a-436">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="d454a-436">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="d454a-437">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="d454a-437">Az.IotHub</span></span>
* <span data-ttu-id="d454a-438">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="d454a-438">Breaking changes:</span></span>
    - <span data-ttu-id="d454a-439">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="d454a-439">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="d454a-440">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="d454a-440">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="d454a-441">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="d454a-441">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="d454a-442">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="d454a-442">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="d454a-443">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="d454a-443">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="d454a-444">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="d454a-444">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="d454a-445">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="d454a-445">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="d454a-446">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="d454a-446">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="d454a-447">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="d454a-447">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="d454a-448">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="d454a-448">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="d454a-449">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="d454a-449">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="d454a-450">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="d454a-450">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-451">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-451">Az.RecoveryServices</span></span>
* <span data-ttu-id="d454a-452">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-452">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="d454a-453">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-453">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="d454a-454">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-454">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="d454a-455">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-455">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="d454a-456">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-456">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="d454a-457">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-457">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="d454a-458">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-458">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="d454a-459">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-459">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="d454a-460">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="d454a-460">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-461">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-461">Az.Resources</span></span>
* <span data-ttu-id="d454a-462">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="d454a-462">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-463">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-463">Az.Network</span></span>
* <span data-ttu-id="d454a-464">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="d454a-464">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="d454a-465">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="d454a-465">Updated cmdlet:</span></span>
        - <span data-ttu-id="d454a-466">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-466">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="d454a-467">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-467">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="d454a-468">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-468">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="d454a-469">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-469">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="d454a-470">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-470">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="d454a-471">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="d454a-471">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="d454a-472">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="d454a-472">New cmdlet:</span></span>
        - <span data-ttu-id="d454a-473">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="d454a-473">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="d454a-474">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="d454a-474">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="d454a-475">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="d454a-475">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="d454a-476">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-476">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="d454a-477">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="d454a-477">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="d454a-478">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="d454a-478">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="d454a-479">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="d454a-479">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="d454a-480">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="d454a-480">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="d454a-481">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d454a-481">New cmdlets added:</span></span>
        - <span data-ttu-id="d454a-482">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="d454a-482">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="d454a-483">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="d454a-483">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="d454a-484">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="d454a-484">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="d454a-485">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="d454a-485">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="d454a-486">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="d454a-486">Set-AzVirtualHub</span></span>
* <span data-ttu-id="d454a-487">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="d454a-487">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="d454a-488">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="d454a-488">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="d454a-489">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="d454a-489">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="d454a-490">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="d454a-490">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="d454a-491">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="d454a-491">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="d454a-492">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="d454a-492">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="d454a-493">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-493">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="d454a-494">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d454a-494">New cmdlets added:</span></span>
        - <span data-ttu-id="d454a-495">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-495">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="d454a-496">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="d454a-496">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="d454a-497">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="d454a-497">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="d454a-498">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="d454a-498">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="d454a-499">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="d454a-499">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="d454a-500">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="d454a-500">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="d454a-501">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="d454a-501">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="d454a-502">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="d454a-502">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="d454a-503">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d454a-503">New cmdlets added:</span></span>
        - <span data-ttu-id="d454a-504">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="d454a-504">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="d454a-505">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="d454a-505">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="d454a-506">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="d454a-506">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="d454a-507">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="d454a-507">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="d454a-508">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="d454a-508">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="d454a-509">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="d454a-509">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="d454a-510">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="d454a-510">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="d454a-511">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="d454a-511">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="d454a-512">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="d454a-512">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="d454a-513">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="d454a-513">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="d454a-514">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="d454a-514">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="d454a-515">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="d454a-515">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="d454a-516">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="d454a-516">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="d454a-517">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="d454a-517">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="d454a-518">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="d454a-518">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="d454a-519">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="d454a-519">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="d454a-520">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="d454a-520">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="d454a-521">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d454a-521">New cmdlets added:</span></span>
        - <span data-ttu-id="d454a-522">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="d454a-522">New-AzIpGroup</span></span>
        - <span data-ttu-id="d454a-523">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="d454a-523">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="d454a-524">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="d454a-524">Get-AzIpGroup</span></span>
        - <span data-ttu-id="d454a-525">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="d454a-525">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="d454a-526">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d454a-526">Az.ServiceFabric</span></span>
* <span data-ttu-id="d454a-527">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="d454a-527">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-528">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-528">Az.Sql</span></span>
* <span data-ttu-id="d454a-529">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="d454a-529">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="d454a-530">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="d454a-530">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="d454a-531">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="d454a-531">Removed deprecated aliases:</span></span>
* <span data-ttu-id="d454a-532">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="d454a-532">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="d454a-533">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="d454a-533">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="d454a-534">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="d454a-534">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="d454a-535">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="d454a-535">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="d454a-536">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="d454a-536">Deprecate Advanced Threat Detection Settings cmdlets</span></span> 
* <span data-ttu-id="d454a-537">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="d454a-537">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-538">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-538">Az.Storage</span></span>
* <span data-ttu-id="d454a-539">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="d454a-539">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="d454a-540">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-540">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="d454a-541">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-541">Set-AzStorageAccount</span></span>
* <span data-ttu-id="d454a-542">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="d454a-542">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="d454a-543">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="d454a-543">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="d454a-544">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="d454a-544">Close-AzStorageFileHandle</span></span>
    
## <a name="280---october-2019"></a><span data-ttu-id="d454a-545">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-545">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="d454a-546">Geral</span><span class="sxs-lookup"><span data-stu-id="d454a-546">General</span></span>
* <span data-ttu-id="d454a-547">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="d454a-547">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="d454a-548">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-548">Az.Accounts</span></span>
* <span data-ttu-id="d454a-549">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="d454a-549">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="d454a-550">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d454a-550">Az.ApiManagement</span></span>
* <span data-ttu-id="d454a-551">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="d454a-551">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="d454a-552">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="d454a-552">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="d454a-553">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="d454a-553">Az.Automation</span></span>
* <span data-ttu-id="d454a-554">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="d454a-554">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="d454a-555">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="d454a-555">Az.Batch</span></span>
* <span data-ttu-id="d454a-556">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="d454a-556">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-557">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-557">Az.Compute</span></span>
* <span data-ttu-id="d454a-558">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="d454a-558">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="d454a-559">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="d454a-559">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="d454a-560">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="d454a-560">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="d454a-561">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="d454a-561">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="d454a-562">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="d454a-562">Az.DataFactory</span></span>
* <span data-ttu-id="d454a-563">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="d454a-563">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="d454a-564">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="d454a-564">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="d454a-565">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="d454a-565">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="d454a-566">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d454a-566">Az.DataLakeStore</span></span>
* <span data-ttu-id="d454a-567">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="d454a-567">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="d454a-568">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="d454a-568">Az.HealthcareApis</span></span>
* <span data-ttu-id="d454a-569">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="d454a-569">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="d454a-570">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="d454a-570">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="d454a-571">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="d454a-571">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="d454a-572">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="d454a-572">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="d454a-573">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="d454a-573">Az.IotHub</span></span>
* <span data-ttu-id="d454a-574">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="d454a-574">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="d454a-575">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="d454a-575">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="d454a-576">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="d454a-576">Az.Monitor</span></span>
* <span data-ttu-id="d454a-577">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="d454a-577">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="d454a-578">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="d454a-578">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="d454a-579">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="d454a-579">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="d454a-580">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d454a-580">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-581">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-581">Az.Network</span></span>
* <span data-ttu-id="d454a-582">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="d454a-582">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="d454a-583">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="d454a-583">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="d454a-584">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d454a-584">New cmdlets added:</span></span>
        - <span data-ttu-id="d454a-585">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="d454a-585">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="d454a-586">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-586">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="d454a-587">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="d454a-587">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="d454a-588">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="d454a-588">Updated cmdlets:</span></span>
        - <span data-ttu-id="d454a-589">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-589">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="d454a-590">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-590">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="d454a-591">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-591">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="d454a-592">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="d454a-592">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="d454a-593">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="d454a-593">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="d454a-594">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="d454a-594">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="d454a-595">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="d454a-595">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="d454a-596">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="d454a-596">Az.RedisCache</span></span>
* <span data-ttu-id="d454a-597">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="d454a-597">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-598">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-598">Az.Sql</span></span>
* <span data-ttu-id="d454a-599">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="d454a-599">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-600">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-600">Az.Storage</span></span>
* <span data-ttu-id="d454a-601">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="d454a-601">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="d454a-602">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="d454a-602">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="d454a-603">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="d454a-603">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="d454a-604">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="d454a-604">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="d454a-605">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-605">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="d454a-606">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="d454a-606">Az.StorageSync</span></span>
* <span data-ttu-id="d454a-607">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="d454a-607">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="d454a-608">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-608">Az.Websites</span></span>
* <span data-ttu-id="d454a-609">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="d454a-609">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="d454a-610">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-610">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="d454a-611">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d454a-611">Az.ApiManagement</span></span>
* <span data-ttu-id="d454a-612">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="d454a-612">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="d454a-613">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="d454a-613">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="d454a-614">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="d454a-614">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="d454a-615">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="d454a-615">Az.Automation</span></span>
* <span data-ttu-id="d454a-616">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="d454a-616">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="d454a-617">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="d454a-617">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="d454a-618">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="d454a-618">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-619">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-619">Az.Compute</span></span>
* <span data-ttu-id="d454a-620">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-620">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="d454a-621">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-621">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="d454a-622">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="d454a-622">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="d454a-623">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="d454a-623">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="d454a-624">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="d454a-624">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="d454a-625">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="d454a-625">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="d454a-626">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="d454a-626">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="d454a-627">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="d454a-627">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="d454a-628">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="d454a-628">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="d454a-629">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="d454a-629">Az.DataFactory</span></span>
* <span data-ttu-id="d454a-630">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="d454a-630">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="d454a-631">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="d454a-631">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="d454a-632">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="d454a-632">Az.HDInsight</span></span>
* <span data-ttu-id="d454a-633">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="d454a-633">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="d454a-634">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="d454a-634">Az.IotHub</span></span>
* <span data-ttu-id="d454a-635">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="d454a-635">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="d454a-636">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="d454a-636">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="d454a-637">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="d454a-637">New cmdlets are:</span></span>
    - <span data-ttu-id="d454a-638">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="d454a-638">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="d454a-639">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="d454a-639">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="d454a-640">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="d454a-640">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="d454a-641">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="d454a-641">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="d454a-642">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="d454a-642">Az.Monitor</span></span>
* <span data-ttu-id="d454a-643">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="d454a-643">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="d454a-644">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="d454a-644">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="d454a-645">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="d454a-645">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="d454a-646">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="d454a-646">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="d454a-647">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="d454a-647">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="d454a-648">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="d454a-648">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="d454a-649">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="d454a-649">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="d454a-650">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="d454a-650">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="d454a-651">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="d454a-651">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="d454a-652">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="d454a-652">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="d454a-653">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="d454a-653">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="d454a-654">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="d454a-654">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="d454a-655">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="d454a-655">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="d454a-656">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="d454a-656">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="d454a-657">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="d454a-657">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="d454a-658">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="d454a-658">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="d454a-659">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="d454a-659">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="d454a-660">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="d454a-660">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="d454a-661">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="d454a-661">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="d454a-662">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="d454a-662">Overall improved help files</span></span>
* <span data-ttu-id="d454a-663">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="d454a-663">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-664">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-664">Az.Network</span></span>
* <span data-ttu-id="d454a-665">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="d454a-665">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="d454a-666">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="d454a-666">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="d454a-667">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="d454a-667">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="d454a-668">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="d454a-668">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="d454a-669">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="d454a-669">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="d454a-670">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="d454a-670">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="d454a-671">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="d454a-671">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="d454a-672">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="d454a-672">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="d454a-673">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="d454a-673">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="d454a-674">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="d454a-674">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="d454a-675">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="d454a-675">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="d454a-676">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="d454a-676">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="d454a-677">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="d454a-677">New cmdlets</span></span>
        - <span data-ttu-id="d454a-678">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="d454a-678">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="d454a-679">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-679">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="d454a-680">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="d454a-680">Updated cmdlet:</span></span>
        - <span data-ttu-id="d454a-681">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="d454a-681">New-VpnSite</span></span>
        - <span data-ttu-id="d454a-682">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="d454a-682">Update-VpnSite</span></span>
        - <span data-ttu-id="d454a-683">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-683">New-VpnConnection</span></span>
        - <span data-ttu-id="d454a-684">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-684">Update-VpnConnection</span></span>
* <span data-ttu-id="d454a-685">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="d454a-685">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-686">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-686">Az.RecoveryServices</span></span>
* <span data-ttu-id="d454a-687">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="d454a-687">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="d454a-688">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="d454a-688">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-689">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-689">Az.Resources</span></span>
* <span data-ttu-id="d454a-690">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="d454a-690">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="d454a-691">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d454a-691">Az.ServiceFabric</span></span>
* <span data-ttu-id="d454a-692">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="d454a-692">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="d454a-693">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="d454a-693">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="d454a-694">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="d454a-694">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="d454a-695">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="d454a-695">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="d454a-696">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="d454a-696">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="d454a-697">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="d454a-697">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="d454a-698">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="d454a-698">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="d454a-699">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="d454a-699">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="d454a-700">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="d454a-700">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="d454a-701">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="d454a-701">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="d454a-702">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="d454a-702">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="d454a-703">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="d454a-703">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="d454a-704">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="d454a-704">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="d454a-705">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="d454a-705">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="d454a-706">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="d454a-706">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="d454a-707">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="d454a-707">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="d454a-708">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="d454a-708">Az.SignalR</span></span>
* <span data-ttu-id="d454a-709">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="d454a-709">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-710">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-710">Az.Sql</span></span>
* <span data-ttu-id="d454a-711">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="d454a-711">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="d454a-712">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="d454a-712">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="d454a-713">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="d454a-713">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="d454a-714">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="d454a-714">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="d454a-715">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="d454a-715">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-716">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-716">Az.Storage</span></span>
* <span data-ttu-id="d454a-717">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="d454a-717">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="d454a-718">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="d454a-718">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="d454a-719">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="d454a-719">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="d454a-720">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="d454a-720">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="d454a-721">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="d454a-721">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="d454a-722">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="d454a-722">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="d454a-723">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="d454a-723">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="d454a-724">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="d454a-724">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="d454a-725">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="d454a-725">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="d454a-726">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="d454a-726">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="d454a-727">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="d454a-727">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="d454a-728">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-728">Az.Websites</span></span>
* <span data-ttu-id="d454a-729">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="d454a-729">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="d454a-730">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="d454a-730">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="d454a-731">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="d454a-731">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="d454a-732">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-732">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="d454a-733">Geral</span><span class="sxs-lookup"><span data-stu-id="d454a-733">General</span></span>
* <span data-ttu-id="d454a-734">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="d454a-734">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="d454a-735">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-735">Az.Accounts</span></span>
* <span data-ttu-id="d454a-736">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="d454a-736">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="d454a-737">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="d454a-737">Az.Aks</span></span>
* <span data-ttu-id="d454a-738">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="d454a-738">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="d454a-739">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="d454a-739">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="d454a-740">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d454a-740">Az.ApiManagement</span></span>
* <span data-ttu-id="d454a-741">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="d454a-741">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="d454a-742">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="d454a-742">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="d454a-743">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="d454a-743">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="d454a-744">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="d454a-744">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="d454a-745">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="d454a-745">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="d454a-746">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="d454a-746">Az.Batch</span></span>
* <span data-ttu-id="d454a-747">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="d454a-747">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="d454a-748">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="d454a-748">Az.Cdn</span></span>
* <span data-ttu-id="d454a-749">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="d454a-749">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-750">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-750">Az.Compute</span></span>
* <span data-ttu-id="d454a-751">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-751">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="d454a-752">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="d454a-752">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="d454a-753">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="d454a-753">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="d454a-754">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="d454a-754">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="d454a-755">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="d454a-755">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="d454a-756">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="d454a-756">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="d454a-757">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="d454a-757">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="d454a-758">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="d454a-758">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="d454a-759">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="d454a-759">Az.DataFactory</span></span>
* <span data-ttu-id="d454a-760">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="d454a-760">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="d454a-761">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="d454a-761">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="d454a-762">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="d454a-762">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="d454a-763">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="d454a-763">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="d454a-764">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d454a-764">Az.DataLakeStore</span></span>
* <span data-ttu-id="d454a-765">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="d454a-765">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="d454a-766">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="d454a-766">Az.EventHub</span></span>
* <span data-ttu-id="d454a-767">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="d454a-767">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="d454a-768">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="d454a-768">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="d454a-769">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="d454a-769">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="d454a-770">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="d454a-770">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="d454a-771">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="d454a-771">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="d454a-772">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="d454a-772">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="d454a-773">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="d454a-773">Az.Monitor</span></span>
* <span data-ttu-id="d454a-774">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="d454a-774">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-775">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-775">Az.Network</span></span>
* <span data-ttu-id="d454a-776">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="d454a-776">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="d454a-777">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="d454a-777">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="d454a-778">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="d454a-778">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="d454a-779">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="d454a-779">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="d454a-780">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="d454a-780">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="d454a-781">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="d454a-781">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="d454a-782">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="d454a-782">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="d454a-783">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="d454a-783">Az.OperationalInsights</span></span>
* <span data-ttu-id="d454a-784">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="d454a-784">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="d454a-785">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="d454a-785">Added example</span></span>
    - <span data-ttu-id="d454a-786">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="d454a-786">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="d454a-787">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="d454a-787">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="d454a-788">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="d454a-788">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-789">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-789">Az.RecoveryServices</span></span>
* <span data-ttu-id="d454a-790">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="d454a-790">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-791">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-791">Az.Resources</span></span>
* <span data-ttu-id="d454a-792">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="d454a-792">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="d454a-793">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="d454a-793">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="d454a-794">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="d454a-794">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="d454a-795">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="d454a-795">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="d454a-796">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d454a-796">Az.ServiceBus</span></span>
* <span data-ttu-id="d454a-797">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="d454a-797">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="d454a-798">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="d454a-798">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="d454a-799">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="d454a-799">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="d454a-800">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d454a-800">Az.ServiceFabric</span></span>
* <span data-ttu-id="d454a-801">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="d454a-801">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="d454a-802">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="d454a-802">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="d454a-803">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="d454a-803">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="d454a-804">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="d454a-804">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="d454a-805">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="d454a-805">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="d454a-806">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="d454a-806">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-807">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-807">Az.Sql</span></span>
* <span data-ttu-id="d454a-808">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="d454a-808">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-809">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-809">Az.Storage</span></span>
* <span data-ttu-id="d454a-810">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="d454a-810">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="d454a-811">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="d454a-811">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="d454a-812">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="d454a-812">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="d454a-813">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="d454a-813">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="d454a-814">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="d454a-814">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="d454a-815">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="d454a-815">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="d454a-816">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-816">Az.Websites</span></span>
* <span data-ttu-id="d454a-817">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="d454a-817">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="d454a-818">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-818">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="d454a-819">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-819">Az.Accounts</span></span>
* <span data-ttu-id="d454a-820">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="d454a-820">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="d454a-821">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="d454a-821">Az.ApplicationInsights</span></span>
* <span data-ttu-id="d454a-822">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="d454a-822">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="d454a-823">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="d454a-823">Az.Automation</span></span>
* <span data-ttu-id="d454a-824">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="d454a-824">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="d454a-825">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="d454a-825">Az.CognitiveServices</span></span>
* <span data-ttu-id="d454a-826">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="d454a-826">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-827">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-827">Az.Compute</span></span>
* <span data-ttu-id="d454a-828">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="d454a-828">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="d454a-829">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="d454a-829">Az.ContainerRegistry</span></span>
* <span data-ttu-id="d454a-830">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="d454a-830">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="d454a-831">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="d454a-831">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="d454a-832">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="d454a-832">Az.DataFactory</span></span>
* <span data-ttu-id="d454a-833">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="d454a-833">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="d454a-834">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="d454a-834">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="d454a-835">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="d454a-835">Az.EventHub</span></span>
* <span data-ttu-id="d454a-836">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="d454a-836">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="d454a-837">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="d454a-837">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="d454a-838">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d454a-838">Az.KeyVault</span></span>
* <span data-ttu-id="d454a-839">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="d454a-839">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="d454a-840">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="d454a-840">Az.LogicApp</span></span>
* <span data-ttu-id="d454a-841">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="d454a-841">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="d454a-842">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="d454a-842">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="d454a-843">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="d454a-843">Az.ManagedServices</span></span>
* <span data-ttu-id="d454a-844">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="d454a-844">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-845">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-845">Az.Network</span></span>
* <span data-ttu-id="d454a-846">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="d454a-846">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="d454a-847">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="d454a-847">New cmdlets</span></span>
        - <span data-ttu-id="d454a-848">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="d454a-848">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="d454a-849">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="d454a-849">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="d454a-850">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-850">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="d454a-851">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-851">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="d454a-852">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-852">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="d454a-853">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-853">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="d454a-854">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="d454a-854">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="d454a-855">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="d454a-855">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="d454a-856">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="d454a-856">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="d454a-857">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-857">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="d454a-858">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="d454a-858">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="d454a-859">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="d454a-859">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="d454a-860">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="d454a-860">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="d454a-861">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="d454a-861">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="d454a-862">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="d454a-862">Updated cmdlets</span></span>
        - <span data-ttu-id="d454a-863">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-863">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="d454a-864">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-864">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="d454a-865">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-865">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="d454a-866">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-866">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="d454a-867">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="d454a-867">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="d454a-868">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="d454a-868">Updated cmdlet:</span></span>
        - <span data-ttu-id="d454a-869">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-869">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="d454a-870">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-870">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="d454a-871">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-871">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="d454a-872">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="d454a-872">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="d454a-873">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="d454a-873">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="d454a-874">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="d454a-874">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="d454a-875">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="d454a-875">Az.OperationalInsights</span></span>
* <span data-ttu-id="d454a-876">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="d454a-876">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="d454a-877">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="d454a-877">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-878">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-878">Az.RecoveryServices</span></span>
* <span data-ttu-id="d454a-879">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="d454a-879">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="d454a-880">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="d454a-880">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="d454a-881">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="d454a-881">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="d454a-882">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="d454a-882">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="d454a-883">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="d454a-883">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="d454a-884">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="d454a-884">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="d454a-885">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="d454a-885">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="d454a-886">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="d454a-886">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="d454a-887">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="d454a-887">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="d454a-888">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="d454a-888">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-889">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-889">Az.Resources</span></span>
- <span data-ttu-id="d454a-890">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="d454a-890">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="d454a-891">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="d454a-891">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="d454a-892">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d454a-892">Az.ServiceBus</span></span>
* <span data-ttu-id="d454a-893">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="d454a-893">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="d454a-894">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="d454a-894">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-895">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-895">Az.Sql</span></span>
* <span data-ttu-id="d454a-896">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="d454a-896">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="d454a-897">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="d454a-897">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="d454a-898">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="d454a-898">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-899">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-899">Az.Storage</span></span>
* <span data-ttu-id="d454a-900">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="d454a-900">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="d454a-901">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="d454a-901">Az.StorageSync</span></span>
* <span data-ttu-id="d454a-902">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="d454a-902">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="d454a-903">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="d454a-903">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="d454a-904">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-904">Az.Websites</span></span>
* <span data-ttu-id="d454a-905">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="d454a-905">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="d454a-906">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="d454a-906">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="d454a-907">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="d454a-907">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="d454a-908">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-908">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="d454a-909">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-909">Az.Accounts</span></span>
* <span data-ttu-id="d454a-910">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="d454a-910">Add support for profile cmdlets</span></span>
* <span data-ttu-id="d454a-911">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="d454a-911">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="d454a-912">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="d454a-912">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="d454a-913">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="d454a-913">Az.Advisor</span></span>
* <span data-ttu-id="d454a-914">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="d454a-914">GA release of Az.Advisor</span></span>
* <span data-ttu-id="d454a-915">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="d454a-915">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="d454a-916">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d454a-916">Az.ApiManagement</span></span>
* <span data-ttu-id="d454a-917">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="d454a-917">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="d454a-918">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="d454a-918">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="d454a-919">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="d454a-919">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="d454a-920">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="d454a-920">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="d454a-921">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="d454a-921">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="d454a-922">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="d454a-922">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="d454a-923">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="d454a-923">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="d454a-924">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="d454a-924">Az.Automation</span></span>
* <span data-ttu-id="d454a-925">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="d454a-925">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-926">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-926">Az.Compute</span></span>
* <span data-ttu-id="d454a-927">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-927">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="d454a-928">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="d454a-928">Az.DataFactory</span></span>
* <span data-ttu-id="d454a-929">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="d454a-929">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="d454a-930">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="d454a-930">Az.EventGrid</span></span>
* <span data-ttu-id="d454a-931">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="d454a-931">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="d454a-932">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="d454a-932">Az.IotHub</span></span>
* <span data-ttu-id="d454a-933">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="d454a-933">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-934">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-934">Az.Network</span></span>
* <span data-ttu-id="d454a-935">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="d454a-935">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="d454a-936">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="d454a-936">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="d454a-937">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="d454a-937">Az.PolicyInsights</span></span>
* <span data-ttu-id="d454a-938">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="d454a-938">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="d454a-939">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="d454a-939">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="d454a-940">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="d454a-940">Az.OperationalInsights</span></span>
* <span data-ttu-id="d454a-941">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="d454a-941">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-942">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-942">Az.RecoveryServices</span></span>
* <span data-ttu-id="d454a-943">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="d454a-943">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-944">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-944">Az.Resources</span></span>
    - <span data-ttu-id="d454a-945">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="d454a-945">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="d454a-946">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="d454a-946">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="d454a-947">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="d454a-947">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="d454a-948">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="d454a-948">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="d454a-949">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d454a-949">Az.ServiceBus</span></span>
* <span data-ttu-id="d454a-950">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="d454a-950">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-951">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-951">Az.Sql</span></span>
* <span data-ttu-id="d454a-952">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="d454a-952">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="d454a-953">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="d454a-953">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="d454a-954">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="d454a-954">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="d454a-955">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="d454a-955">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="d454a-956">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="d454a-956">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="d454a-957">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="d454a-957">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="d454a-958">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="d454a-958">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="d454a-959">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="d454a-959">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="d454a-960">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="d454a-960">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-961">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-961">Az.Storage</span></span>
* <span data-ttu-id="d454a-962">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="d454a-962">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="d454a-963">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="d454a-963">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="d454a-964">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="d454a-964">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="d454a-965">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="d454a-965">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="d454a-966">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="d454a-966">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="d454a-967">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-967">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="d454a-968">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-968">Set-AzStorageAccount</span></span>
* <span data-ttu-id="d454a-969">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="d454a-969">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="d454a-970">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="d454a-970">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="d454a-971">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="d454a-971">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="d454a-972">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="d454a-972">Az.StorageSync</span></span>
* <span data-ttu-id="d454a-973">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="d454a-973">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="d454a-974">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-974">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="d454a-975">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-975">Az.Accounts</span></span>
* <span data-ttu-id="d454a-976">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="d454a-976">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="d454a-977">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="d454a-977">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="d454a-978">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="d454a-978">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="d454a-979">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="d454a-979">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="d454a-980">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="d454a-980">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-981">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-981">Az.Compute</span></span>
* <span data-ttu-id="d454a-982">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="d454a-982">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="d454a-983">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="d454a-983">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="d454a-984">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="d454a-984">Az.Dns</span></span>
* <span data-ttu-id="d454a-985">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="d454a-985">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="d454a-986">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="d454a-986">Az.EventGrid</span></span>
* <span data-ttu-id="d454a-987">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="d454a-987">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="d454a-988">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d454a-988">New cmdlets:</span></span>
    - <span data-ttu-id="d454a-989">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="d454a-989">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="d454a-990">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="d454a-990">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="d454a-991">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="d454a-991">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="d454a-992">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-992">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="d454a-993">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="d454a-993">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="d454a-994">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="d454a-994">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="d454a-995">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="d454a-995">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="d454a-996">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="d454a-996">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="d454a-997">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="d454a-997">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="d454a-998">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="d454a-998">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="d454a-999">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="d454a-999">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="d454a-1000">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="d454a-1000">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="d454a-1001">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="d454a-1001">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="d454a-1002">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="d454a-1002">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="d454a-1003">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="d454a-1003">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="d454a-1004">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="d454a-1004">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="d454a-1005">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="d454a-1005">Updated cmdlets:</span></span>
    - <span data-ttu-id="d454a-1006">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="d454a-1006">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="d454a-1007">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="d454a-1007">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="d454a-1008">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="d454a-1008">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="d454a-1009">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="d454a-1009">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="d454a-1010">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="d454a-1010">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="d454a-1011">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="d454a-1011">Event subscription expiration date,</span></span>
            - <span data-ttu-id="d454a-1012">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="d454a-1012">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="d454a-1013">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="d454a-1013">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="d454a-1014">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="d454a-1014">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="d454a-1015">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="d454a-1015">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="d454a-1016">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="d454a-1016">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="d454a-1017">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="d454a-1017">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="d454a-1018">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="d454a-1018">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="d454a-1019">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="d454a-1019">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="d454a-1020">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="d454a-1020">Az.FrontDoor</span></span>
* <span data-ttu-id="d454a-1021">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="d454a-1021">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="d454a-1022">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="d454a-1022">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="d454a-1023">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="d454a-1023">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="d454a-1024">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="d454a-1024">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-1025">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1025">Az.Network</span></span>
* <span data-ttu-id="d454a-1026">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="d454a-1026">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="d454a-1027">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="d454a-1027">New cmdlets</span></span>
        - <span data-ttu-id="d454a-1028">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="d454a-1028">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="d454a-1029">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="d454a-1029">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="d454a-1030">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="d454a-1030">New cmdlets</span></span> 
        - <span data-ttu-id="d454a-1031">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="d454a-1031">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="d454a-1032">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="d454a-1032">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="d454a-1033">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="d454a-1033">New cmdlets</span></span> 
        - <span data-ttu-id="d454a-1034">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="d454a-1034">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="d454a-1035">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="d454a-1035">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="d454a-1036">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="d454a-1036">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="d454a-1037">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-1037">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="d454a-1038">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-1038">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="d454a-1039">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="d454a-1039">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="d454a-1040">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="d454a-1040">New cmdlets</span></span>
        - <span data-ttu-id="d454a-1041">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="d454a-1041">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="d454a-1042">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="d454a-1042">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="d454a-1043">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="d454a-1043">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="d454a-1044">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-1044">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="d454a-1045">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="d454a-1045">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="d454a-1046">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="d454a-1046">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="d454a-1047">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="d454a-1047">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="d454a-1048">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="d454a-1048">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="d454a-1049">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="d454a-1049">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="d454a-1050">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="d454a-1050">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="d454a-1051">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="d454a-1051">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="d454a-1052">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="d454a-1052">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="d454a-1053">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="d454a-1053">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="d454a-1054">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="d454a-1054">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="d454a-1055">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="d454a-1055">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="d454a-1056">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="d454a-1056">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="d454a-1057">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="d454a-1057">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="d454a-1058">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="d454a-1058">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="d454a-1059">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="d454a-1059">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="d454a-1060">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="d454a-1060">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="d454a-1061">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="d454a-1061">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="d454a-1062">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="d454a-1062">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="d454a-1063">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="d454a-1063">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="d454a-1064">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="d454a-1064">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="d454a-1065">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="d454a-1065">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="d454a-1066">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="d454a-1066">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="d454a-1067">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="d454a-1067">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="d454a-1068">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="d454a-1068">Az.OperationalInsights</span></span>
* <span data-ttu-id="d454a-1069">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="d454a-1069">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-1070">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1070">Az.Resources</span></span>
* <span data-ttu-id="d454a-1071">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="d454a-1071">Support for additional Template Export options</span></span>
    - <span data-ttu-id="d454a-1072">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="d454a-1072">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="d454a-1073">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="d454a-1073">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="d454a-1074">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="d454a-1074">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="d454a-1075">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d454a-1075">Az.ServiceFabric</span></span>
* <span data-ttu-id="d454a-1076">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="d454a-1076">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-1077">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-1077">Az.Sql</span></span>
* <span data-ttu-id="d454a-1078">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="d454a-1078">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="d454a-1079">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="d454a-1079">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="d454a-1080">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="d454a-1080">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="d454a-1081">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="d454a-1081">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="d454a-1082">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="d454a-1082">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="d454a-1083">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="d454a-1083">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="d454a-1084">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="d454a-1084">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="d454a-1085">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="d454a-1085">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-1086">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-1086">Az.Storage</span></span>
* <span data-ttu-id="d454a-1087">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="d454a-1087">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="d454a-1088">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-1088">New-AzStorageAccount</span></span>
* <span data-ttu-id="d454a-1089">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="d454a-1089">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="d454a-1090">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="d454a-1090">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="d454a-1091">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-1091">Az.Websites</span></span>
* <span data-ttu-id="d454a-1092">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="d454a-1092">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="d454a-1093">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="d454a-1093">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="d454a-1094">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-1094">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="d454a-1095">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="d454a-1095">Az.Cdn</span></span>
* <span data-ttu-id="d454a-1096">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="d454a-1096">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-1097">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1097">Az.Compute</span></span>
* <span data-ttu-id="d454a-1098">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="d454a-1098">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="d454a-1099">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="d454a-1099">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="d454a-1100">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="d454a-1100">Az.EventHub</span></span>
* <span data-ttu-id="d454a-1101">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="d454a-1101">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="d454a-1102">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="d454a-1102">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-1103">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1103">Az.Network</span></span>
* <span data-ttu-id="d454a-1104">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="d454a-1104">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="d454a-1105">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="d454a-1105">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="d454a-1106">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="d454a-1106">Az.PolicyInsights</span></span>
* <span data-ttu-id="d454a-1107">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="d454a-1107">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-1108">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1108">Az.RecoveryServices</span></span>
* <span data-ttu-id="d454a-1109">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="d454a-1109">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="d454a-1110">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d454a-1110">Az.ServiceBus</span></span>
* <span data-ttu-id="d454a-1111">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="d454a-1111">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="d454a-1112">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d454a-1112">Az.ServiceFabric</span></span>
* <span data-ttu-id="d454a-1113">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="d454a-1113">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="d454a-1114">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d454a-1114">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-1115">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-1115">Az.Sql</span></span>
* <span data-ttu-id="d454a-1116">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="d454a-1116">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="d454a-1117">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="d454a-1117">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="d454a-1118">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="d454a-1118">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="d454a-1119">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="d454a-1119">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="d454a-1120">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-1120">Az.Websites</span></span>
* <span data-ttu-id="d454a-1121">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="d454a-1121">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="d454a-1122">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-1122">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="d454a-1123">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d454a-1123">Az.ApiManagement</span></span>
* <span data-ttu-id="d454a-1124">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="d454a-1124">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="d454a-1125">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="d454a-1125">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="d454a-1126">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="d454a-1126">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="d454a-1127">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="d454a-1127">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="d454a-1128">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="d454a-1128">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="d454a-1129">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="d454a-1129">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="d454a-1130">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="d454a-1130">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="d454a-1131">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="d454a-1131">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="d454a-1132">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d454a-1132">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="d454a-1133">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="d454a-1133">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="d454a-1134">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="d454a-1134">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="d454a-1135">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="d454a-1135">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="d454a-1136">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="d454a-1136">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="d454a-1137">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="d454a-1137">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="d454a-1138">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="d454a-1138">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="d454a-1139">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="d454a-1139">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="d454a-1140">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="d454a-1140">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="d454a-1141">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="d454a-1141">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="d454a-1142">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="d454a-1142">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="d454a-1143">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="d454a-1143">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="d454a-1144">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="d454a-1144">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="d454a-1145">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="d454a-1145">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="d454a-1146">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="d454a-1146">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="d454a-1147">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d454a-1147">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="d454a-1148">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="d454a-1148">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="d454a-1149">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="d454a-1149">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="d454a-1150">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="d454a-1150">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="d454a-1151">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="d454a-1151">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="d454a-1152">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="d454a-1152">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="d454a-1153">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="d454a-1153">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="d454a-1154">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="d454a-1154">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="d454a-1155">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="d454a-1155">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="d454a-1156">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="d454a-1156">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="d454a-1157">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="d454a-1157">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="d454a-1158">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="d454a-1158">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="d454a-1159">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="d454a-1159">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="d454a-1160">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="d454a-1160">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="d454a-1161">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="d454a-1161">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="d454a-1162">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="d454a-1162">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="d454a-1163">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="d454a-1163">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="d454a-1164">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="d454a-1164">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="d454a-1165">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="d454a-1165">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="d454a-1166">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="d454a-1166">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="d454a-1167">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="d454a-1167">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="d454a-1168">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="d454a-1168">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="d454a-1169">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="d454a-1169">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="d454a-1170">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="d454a-1170">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="d454a-1171">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="d454a-1171">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="d454a-1172">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="d454a-1172">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="d454a-1173">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="d454a-1173">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="d454a-1174">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="d454a-1174">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="d454a-1175">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="d454a-1175">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="d454a-1176">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="d454a-1176">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="d454a-1177">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="d454a-1177">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="d454a-1178">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="d454a-1178">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="d454a-1179">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="d454a-1179">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="d454a-1180">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="d454a-1180">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="d454a-1181">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="d454a-1181">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="d454a-1182">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="d454a-1182">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="d454a-1183">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="d454a-1183">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="d454a-1184">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="d454a-1184">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="d454a-1185">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="d454a-1185">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="d454a-1186">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="d454a-1186">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="d454a-1187">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="d454a-1187">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="d454a-1188">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="d454a-1188">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="d454a-1189">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="d454a-1189">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="d454a-1190">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="d454a-1190">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="d454a-1191">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="d454a-1191">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="d454a-1192">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="d454a-1192">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="d454a-1193">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="d454a-1193">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="d454a-1194">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="d454a-1194">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="d454a-1195">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="d454a-1195">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="d454a-1196">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="d454a-1196">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="d454a-1197">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="d454a-1197">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="d454a-1198">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="d454a-1198">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="d454a-1199">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="d454a-1199">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="d454a-1200">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="d454a-1200">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="d454a-1201">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="d454a-1201">Az.Automation</span></span>
* <span data-ttu-id="d454a-1202">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="d454a-1202">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="d454a-1203">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="d454a-1203">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="d454a-1204">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="d454a-1204">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="d454a-1205">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="d454a-1205">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="d454a-1206">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="d454a-1206">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="d454a-1207">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="d454a-1207">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="d454a-1208">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="d454a-1208">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-1209">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1209">Az.Compute</span></span>
* <span data-ttu-id="d454a-1210">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="d454a-1210">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="d454a-1211">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="d454a-1211">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="d454a-1212">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d454a-1212">Az.DataLakeStore</span></span>
* <span data-ttu-id="d454a-1213">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="d454a-1213">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="d454a-1214">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="d454a-1214">Az.Monitor</span></span>
* <span data-ttu-id="d454a-1215">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="d454a-1215">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-1216">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1216">Az.Network</span></span>
* <span data-ttu-id="d454a-1217">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="d454a-1217">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="d454a-1218">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="d454a-1218">Updated cmdlet:</span></span>
        - <span data-ttu-id="d454a-1219">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="d454a-1219">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="d454a-1220">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d454a-1220">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-1221">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1221">Az.Resources</span></span>
* <span data-ttu-id="d454a-1222">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="d454a-1222">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-1223">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-1223">Az.Sql</span></span>
* <span data-ttu-id="d454a-1224">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="d454a-1224">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="d454a-1225">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-1225">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="d454a-1226">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-1226">Az.Accounts</span></span>
* <span data-ttu-id="d454a-1227">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="d454a-1227">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="d454a-1228">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1228">Az.CognitiveServices</span></span>
* <span data-ttu-id="d454a-1229">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="d454a-1229">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="d454a-1230">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="d454a-1230">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-1231">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1231">Az.Compute</span></span>
* <span data-ttu-id="d454a-1232">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="d454a-1232">Proximity placement group feature.</span></span>
    - <span data-ttu-id="d454a-1233">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="d454a-1233">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="d454a-1234">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-1234">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="d454a-1235">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="d454a-1235">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="d454a-1236">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="d454a-1236">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="d454a-1237">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="d454a-1237">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="d454a-1238">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="d454a-1238">Breaking changes</span></span>
    - <span data-ttu-id="d454a-1239">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="d454a-1239">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="d454a-1240">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="d454a-1240">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="d454a-1241">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="d454a-1241">Az.DeploymentManager</span></span>
* <span data-ttu-id="d454a-1242">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="d454a-1242">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="d454a-1243">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="d454a-1243">Az.Dns</span></span>
* <span data-ttu-id="d454a-1244">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="d454a-1244">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="d454a-1245">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="d454a-1245">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="d454a-1246">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="d454a-1246">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="d454a-1247">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="d454a-1247">Az.FrontDoor</span></span>
* <span data-ttu-id="d454a-1248">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="d454a-1248">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="d454a-1249">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="d454a-1249">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="d454a-1250">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="d454a-1250">Az.HDInsight</span></span>
* <span data-ttu-id="d454a-1251">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d454a-1251">Removed two cmdlets:</span></span>
    - <span data-ttu-id="d454a-1252">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="d454a-1252">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="d454a-1253">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="d454a-1253">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="d454a-1254">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="d454a-1254">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="d454a-1255">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="d454a-1255">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="d454a-1256">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="d454a-1256">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="d454a-1257">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="d454a-1257">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="d454a-1258">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="d454a-1258">Az.Monitor</span></span>
* <span data-ttu-id="d454a-1259">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="d454a-1259">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="d454a-1260">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="d454a-1260">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="d454a-1261">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="d454a-1261">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="d454a-1262">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="d454a-1262">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="d454a-1263">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="d454a-1263">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="d454a-1264">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="d454a-1264">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="d454a-1265">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="d454a-1265">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="d454a-1266">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="d454a-1266">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="d454a-1267">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="d454a-1267">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="d454a-1268">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="d454a-1268">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="d454a-1269">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="d454a-1269">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="d454a-1270">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="d454a-1270">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="d454a-1271">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="d454a-1271">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="d454a-1272">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="d454a-1272">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-1273">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1273">Az.Network</span></span>
* <span data-ttu-id="d454a-1274">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="d454a-1274">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="d454a-1275">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="d454a-1275">New cmdlets</span></span>
        - <span data-ttu-id="d454a-1276">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="d454a-1276">New-AzNatGateway</span></span>
        - <span data-ttu-id="d454a-1277">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="d454a-1277">Get-AzNatGateway</span></span>
        - <span data-ttu-id="d454a-1278">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="d454a-1278">Set-AzNatGateway</span></span>
        - <span data-ttu-id="d454a-1279">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="d454a-1279">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="d454a-1280">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="d454a-1280">Updated cmdlets</span></span>
        - <span data-ttu-id="d454a-1281">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="d454a-1281">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="d454a-1282">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="d454a-1282">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="d454a-1283">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="d454a-1283">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="d454a-1284">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="d454a-1284">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="d454a-1285">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="d454a-1285">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="d454a-1286">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="d454a-1286">Az.PolicyInsights</span></span>
* <span data-ttu-id="d454a-1287">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="d454a-1287">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="d454a-1288">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="d454a-1288">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="d454a-1289">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="d454a-1289">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-1290">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1290">Az.RecoveryServices</span></span>
* <span data-ttu-id="d454a-1291">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="d454a-1291">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="d454a-1292">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="d454a-1292">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="d454a-1293">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="d454a-1293">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="d454a-1294">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-1294">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="d454a-1295">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="d454a-1295">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="d454a-1296">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="d454a-1296">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="d454a-1297">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="d454a-1297">Az.Relay</span></span>
* <span data-ttu-id="d454a-1298">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="d454a-1298">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="d454a-1299">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d454a-1299">Az.ServiceBus</span></span>
* <span data-ttu-id="d454a-1300">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="d454a-1300">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-1301">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-1301">Az.Storage</span></span>
* <span data-ttu-id="d454a-1302">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="d454a-1302">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="d454a-1303">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="d454a-1303">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="d454a-1304">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="d454a-1304">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="d454a-1305">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-1305">New-AzStorageAccount</span></span>
* <span data-ttu-id="d454a-1306">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="d454a-1306">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="d454a-1307">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-1307">New-AzStorageAccount</span></span>
    - <span data-ttu-id="d454a-1308">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-1308">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="d454a-1309">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-1309">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="d454a-1310">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-1310">Az.Websites</span></span>
* <span data-ttu-id="d454a-1311">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="d454a-1311">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="d454a-1312">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="d454a-1312">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="d454a-1313">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-1313">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="d454a-1314">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="d454a-1314">Highlights since the last major release</span></span>
* <span data-ttu-id="d454a-1315">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="d454a-1315">General availability of `Az` module</span></span>
* <span data-ttu-id="d454a-1316">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="d454a-1316">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="d454a-1317">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="d454a-1317">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="d454a-1318">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1318">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="d454a-1319">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="d454a-1319">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="d454a-1320">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="d454a-1320">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="d454a-1321">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="d454a-1321">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="d454a-1322">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-1322">Az.Accounts</span></span>
* <span data-ttu-id="d454a-1323">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="d454a-1323">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="d454a-1324">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="d454a-1324">Az.Batch</span></span>
* <span data-ttu-id="d454a-1325">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1325">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="d454a-1326">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="d454a-1326">Az.Cdn</span></span>
* <span data-ttu-id="d454a-1327">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1327">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="d454a-1328">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1328">Az.CognitiveServices</span></span>
* <span data-ttu-id="d454a-1329">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1329">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-1330">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1330">Az.Compute</span></span>
* <span data-ttu-id="d454a-1331">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="d454a-1331">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="d454a-1332">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1332">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="d454a-1333">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="d454a-1333">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="d454a-1334">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="d454a-1334">Az.DataFactory</span></span>
* <span data-ttu-id="d454a-1335">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="d454a-1335">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="d454a-1336">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d454a-1336">Az.DataLakeStore</span></span>
* <span data-ttu-id="d454a-1337">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1337">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="d454a-1338">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="d454a-1338">Az.EventGrid</span></span>
* <span data-ttu-id="d454a-1339">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="d454a-1339">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="d454a-1340">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="d454a-1340">Az.EventHub</span></span>
* <span data-ttu-id="d454a-1341">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="d454a-1341">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="d454a-1342">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="d454a-1342">Az.HDInsight</span></span>
* <span data-ttu-id="d454a-1343">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1343">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="d454a-1344">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="d454a-1344">Az.IotHub</span></span>
* <span data-ttu-id="d454a-1345">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1345">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="d454a-1346">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d454a-1346">Az.KeyVault</span></span>
* <span data-ttu-id="d454a-1347">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1347">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="d454a-1348">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="d454a-1348">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="d454a-1349">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="d454a-1349">Az.MachineLearning</span></span>
* <span data-ttu-id="d454a-1350">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1350">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="d454a-1351">Az.Media</span><span class="sxs-lookup"><span data-stu-id="d454a-1351">Az.Media</span></span>
* <span data-ttu-id="d454a-1352">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1352">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="d454a-1353">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="d454a-1353">Az.Monitor</span></span>
  * <span data-ttu-id="d454a-1354">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="d454a-1354">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="d454a-1355">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="d454a-1355">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="d454a-1356">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="d454a-1356">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="d454a-1357">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="d454a-1357">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="d454a-1358">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="d454a-1358">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="d454a-1359">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="d454a-1359">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="d454a-1360">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="d454a-1360">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-1361">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1361">Az.Network</span></span>
* <span data-ttu-id="d454a-1362">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1362">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="d454a-1363">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="d454a-1363">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="d454a-1364">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="d454a-1364">Az.NotificationHubs</span></span>
* <span data-ttu-id="d454a-1365">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1365">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="d454a-1366">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="d454a-1366">Az.OperationalInsights</span></span>
* <span data-ttu-id="d454a-1367">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1367">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="d454a-1368">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="d454a-1368">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="d454a-1369">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1369">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-1370">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1370">Az.RecoveryServices</span></span>
* <span data-ttu-id="d454a-1371">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1371">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="d454a-1372">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="d454a-1372">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="d454a-1373">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="d454a-1373">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="d454a-1374">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="d454a-1374">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="d454a-1375">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="d454a-1375">Az.RedisCache</span></span>
* <span data-ttu-id="d454a-1376">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1376">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-1377">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1377">Az.Resources</span></span>
* <span data-ttu-id="d454a-1378">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="d454a-1378">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-1379">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-1379">Az.Sql</span></span>
* <span data-ttu-id="d454a-1380">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="d454a-1380">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="d454a-1381">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1381">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="d454a-1382">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="d454a-1382">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="d454a-1383">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="d454a-1383">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="d454a-1384">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="d454a-1384">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="d454a-1385">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="d454a-1385">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="d454a-1386">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="d454a-1386">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="d454a-1387">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-1387">Az.Websites</span></span>
* <span data-ttu-id="d454a-1388">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="d454a-1388">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="d454a-1389">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="d454a-1389">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="d454a-1390">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="d454a-1390">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="d454a-1391">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="d454a-1391">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="d454a-1392">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-1392">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="d454a-1393">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="d454a-1393">Highlights since the last major release</span></span>
* <span data-ttu-id="d454a-1394">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="d454a-1394">General availability of `Az` module</span></span>
* <span data-ttu-id="d454a-1395">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="d454a-1395">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="d454a-1396">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="d454a-1396">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="d454a-1397">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1397">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="d454a-1398">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="d454a-1398">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="d454a-1399">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="d454a-1399">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="d454a-1400">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="d454a-1400">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="d454a-1401">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-1401">Az.Accounts</span></span>
* <span data-ttu-id="d454a-1402">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="d454a-1402">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="d454a-1403">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1403">Az.AnalysisServices</span></span>
* <span data-ttu-id="d454a-1404">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="d454a-1404">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="d454a-1405">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="d454a-1405">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="d454a-1406">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="d454a-1406">Az.Automation</span></span>
* <span data-ttu-id="d454a-1407">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="d454a-1407">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="d454a-1408">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="d454a-1408">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="d454a-1409">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="d454a-1409">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-1410">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1410">Az.Compute</span></span>
* <span data-ttu-id="d454a-1411">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-1411">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="d454a-1412">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="d454a-1412">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="d454a-1413">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="d454a-1413">Az.ContainerInstance</span></span>
* <span data-ttu-id="d454a-1414">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="d454a-1414">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="d454a-1415">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="d454a-1415">Az.DataFactory</span></span>
* <span data-ttu-id="d454a-1416">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="d454a-1416">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="d454a-1417">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d454a-1417">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-1418">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1418">Az.Resources</span></span>
* <span data-ttu-id="d454a-1419">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="d454a-1419">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="d454a-1420">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="d454a-1420">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="d454a-1421">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="d454a-1421">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="d454a-1422">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="d454a-1422">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="d454a-1423">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="d454a-1423">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="d454a-1424">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="d454a-1424">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-1425">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-1425">Az.Sql</span></span>
* <span data-ttu-id="d454a-1426">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="d454a-1426">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-1427">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-1427">Az.Storage</span></span>
* <span data-ttu-id="d454a-1428">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="d454a-1428">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="d454a-1429">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="d454a-1429">New-AzStorageContext</span></span>
* <span data-ttu-id="d454a-1430">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="d454a-1430">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="d454a-1431">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="d454a-1431">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="d454a-1432">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="d454a-1432">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="d454a-1433">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="d454a-1433">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="d454a-1434">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="d454a-1434">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="d454a-1435">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="d454a-1435">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="d454a-1436">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="d454a-1436">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="d454a-1437">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="d454a-1437">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="d454a-1438">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="d454a-1438">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="d454a-1439">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="d454a-1439">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="d454a-1440">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-1440">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="d454a-1441">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="d454a-1441">Highlights since the last major release</span></span>
* <span data-ttu-id="d454a-1442">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="d454a-1442">General availability of `Az` module</span></span>
* <span data-ttu-id="d454a-1443">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="d454a-1443">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="d454a-1444">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="d454a-1444">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="d454a-1445">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1445">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="d454a-1446">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="d454a-1446">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="d454a-1447">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="d454a-1447">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="d454a-1448">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="d454a-1448">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="d454a-1449">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="d454a-1449">Az.Automation</span></span>
* <span data-ttu-id="d454a-1450">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="d454a-1450">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="d454a-1451">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="d454a-1451">Dynamic grouping</span></span>
    * <span data-ttu-id="d454a-1452">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="d454a-1452">Pre-Post script</span></span>
    * <span data-ttu-id="d454a-1453">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="d454a-1453">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-1454">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1454">Az.Compute</span></span>
* <span data-ttu-id="d454a-1455">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="d454a-1455">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="d454a-1456">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="d454a-1456">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="d454a-1457">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d454a-1457">Az.KeyVault</span></span>
* <span data-ttu-id="d454a-1458">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="d454a-1458">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-1459">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1459">Az.Network</span></span>
* <span data-ttu-id="d454a-1460">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="d454a-1460">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="d454a-1461">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="d454a-1461">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-1462">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1462">Az.RecoveryServices</span></span>
* <span data-ttu-id="d454a-1463">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="d454a-1463">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="d454a-1464">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="d454a-1464">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-1465">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1465">Az.Resources</span></span>
* <span data-ttu-id="d454a-1466">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="d454a-1466">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="d454a-1467">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="d454a-1467">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-1468">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-1468">Az.Sql</span></span>
* <span data-ttu-id="d454a-1469">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="d454a-1469">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-1470">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-1470">Az.Storage</span></span>
* <span data-ttu-id="d454a-1471">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d454a-1471">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="d454a-1472">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="d454a-1472">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="d454a-1473">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="d454a-1473">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="d454a-1474">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="d454a-1474">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="d454a-1475">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="d454a-1475">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="d454a-1476">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="d454a-1476">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="d454a-1477">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="d454a-1477">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="d454a-1478">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-1478">Az.Websites</span></span>
* <span data-ttu-id="d454a-1479">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="d454a-1479">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="d454a-1480">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-1480">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="d454a-1481">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-1481">Az.Accounts</span></span>
* <span data-ttu-id="d454a-1482">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="d454a-1482">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="d454a-1483">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-1483">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="d454a-1484">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="d454a-1484">Az.Automation</span></span>
* <span data-ttu-id="d454a-1485">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="d454a-1485">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="d454a-1486">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="d454a-1486">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="d454a-1487">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="d454a-1487">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="d454a-1488">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="d454a-1488">Az.Cdn</span></span>
* <span data-ttu-id="d454a-1489">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="d454a-1489">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-1490">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1490">Az.Compute</span></span>
* <span data-ttu-id="d454a-1491">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="d454a-1491">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="d454a-1492">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="d454a-1492">Az.DataFactory</span></span>
* <span data-ttu-id="d454a-1493">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="d454a-1493">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="d454a-1494">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="d454a-1494">Az.LogicApp</span></span>
* <span data-ttu-id="d454a-1495">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="d454a-1495">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-1496">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1496">Az.Network</span></span>
* <span data-ttu-id="d454a-1497">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1497">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-1498">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1498">Az.RecoveryServices</span></span>
* <span data-ttu-id="d454a-1499">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="d454a-1499">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="d454a-1500">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="d454a-1500">SDK Update</span></span>
* <span data-ttu-id="d454a-1501">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="d454a-1501">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="d454a-1502">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="d454a-1502">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-1503">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1503">Az.Resources</span></span>
* <span data-ttu-id="d454a-1504">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="d454a-1504">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="d454a-1505">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="d454a-1505">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="d454a-1506">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="d454a-1506">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="d454a-1507">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="d454a-1507">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="d454a-1508">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="d454a-1508">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="d454a-1509">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="d454a-1509">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-1510">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-1510">Az.Sql</span></span>
* <span data-ttu-id="d454a-1511">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="d454a-1511">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="d454a-1512">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="d454a-1512">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-1513">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-1513">Az.Storage</span></span>
* <span data-ttu-id="d454a-1514">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-1514">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="d454a-1515">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-1515">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="d454a-1516">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1516">Az.AnalysisServices</span></span>
* <span data-ttu-id="d454a-1517">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="d454a-1517">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="d454a-1518">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="d454a-1518">Az.Automation</span></span>
* <span data-ttu-id="d454a-1519">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d454a-1519">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="d454a-1520">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="d454a-1520">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="d454a-1521">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="d454a-1521">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="d454a-1522">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1522">Az.CognitiveServices</span></span>
* <span data-ttu-id="d454a-1523">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="d454a-1523">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-1524">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1524">Az.Compute</span></span>
* <span data-ttu-id="d454a-1525">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="d454a-1525">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="d454a-1526">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="d454a-1526">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="d454a-1527">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="d454a-1527">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="d454a-1528">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="d454a-1528">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="d454a-1529">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d454a-1529">Az.DataLakeStore</span></span>
* <span data-ttu-id="d454a-1530">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="d454a-1530">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="d454a-1531">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="d454a-1531">Az.EventHub</span></span>
* <span data-ttu-id="d454a-1532">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="d454a-1532">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="d454a-1533">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d454a-1533">Az.KeyVault</span></span>
* <span data-ttu-id="d454a-1534">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="d454a-1534">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="d454a-1535">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="d454a-1535">Az.LogicApp</span></span>
* <span data-ttu-id="d454a-1536">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="d454a-1536">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="d454a-1537">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="d454a-1537">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="d454a-1538">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="d454a-1538">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="d454a-1539">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="d454a-1539">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="d454a-1540">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="d454a-1540">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="d454a-1541">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="d454a-1541">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="d454a-1542">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="d454a-1542">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="d454a-1543">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="d454a-1543">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="d454a-1544">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="d454a-1544">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="d454a-1545">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="d454a-1545">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="d454a-1546">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="d454a-1546">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="d454a-1547">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="d454a-1547">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="d454a-1548">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="d454a-1548">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="d454a-1549">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="d454a-1549">Az.Monitor</span></span>
* <span data-ttu-id="d454a-1550">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="d454a-1550">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-1551">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1551">Az.Network</span></span>
* <span data-ttu-id="d454a-1552">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="d454a-1552">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="d454a-1553">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="d454a-1553">Az.OperationalInsights</span></span>
* <span data-ttu-id="d454a-1554">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="d454a-1554">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="d454a-1555">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d454a-1555">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="d454a-1556">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="d454a-1556">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="d454a-1557">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1557">Az.Resources</span></span>
* <span data-ttu-id="d454a-1558">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="d454a-1558">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="d454a-1559">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="d454a-1559">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="d454a-1560">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="d454a-1560">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="d454a-1561">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="d454a-1561">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-1562">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-1562">Az.Sql</span></span>
* <span data-ttu-id="d454a-1563">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="d454a-1563">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="d454a-1564">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="d454a-1564">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="d454a-1565">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-1565">Az.Websites</span></span>
* <span data-ttu-id="d454a-1566">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="d454a-1566">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="d454a-1567">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-1567">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="d454a-1568">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-1568">Az.Accounts</span></span>
* <span data-ttu-id="d454a-1569">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="d454a-1569">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="d454a-1570">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1570">Az.AnalysisServices</span></span>
<span data-ttu-id="d454a-1571">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="d454a-1571">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-1572">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1572">Az.Compute</span></span>
* <span data-ttu-id="d454a-1573">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="d454a-1573">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="d454a-1574">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="d454a-1574">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="d454a-1575">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="d454a-1575">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-1576">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1576">Az.RecoveryServices</span></span>
<span data-ttu-id="d454a-1577">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="d454a-1577">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-1578">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1578">Az.Resources</span></span>
* <span data-ttu-id="d454a-1579">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="d454a-1579">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="d454a-1580">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="d454a-1580">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="d454a-1581">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="d454a-1581">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="d454a-1582">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="d454a-1582">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-1583">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-1583">Az.Sql</span></span>
* <span data-ttu-id="d454a-1584">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="d454a-1584">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="d454a-1585">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="d454a-1585">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="d454a-1586">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="d454a-1586">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="d454a-1587">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-1587">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="d454a-1588">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-1588">Az.Accounts</span></span>
* <span data-ttu-id="d454a-1589">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="d454a-1589">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="d454a-1590">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1590">Az.AnalysisServices</span></span>
* <span data-ttu-id="d454a-1591">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="d454a-1591">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-1592">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1592">Az.RecoveryServices</span></span>
* <span data-ttu-id="d454a-1593">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="d454a-1593">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="d454a-1594">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-1594">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="d454a-1595">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-1595">Az.Accounts</span></span>
* <span data-ttu-id="d454a-1596">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="d454a-1596">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="d454a-1597">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="d454a-1597">Update incorrect online help URLs</span></span>
* <span data-ttu-id="d454a-1598">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="d454a-1598">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="d454a-1599">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="d454a-1599">Az.Aks</span></span>
* <span data-ttu-id="d454a-1600">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="d454a-1600">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="d454a-1601">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="d454a-1601">Az.Automation</span></span>
* <span data-ttu-id="d454a-1602">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="d454a-1602">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="d454a-1603">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="d454a-1603">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="d454a-1604">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="d454a-1604">Az.Cdn</span></span>
* <span data-ttu-id="d454a-1605">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="d454a-1605">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-1606">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1606">Az.Compute</span></span>
* <span data-ttu-id="d454a-1607">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="d454a-1607">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="d454a-1608">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="d454a-1608">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="d454a-1609">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="d454a-1609">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="d454a-1610">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="d454a-1610">Az.ContainerRegistry</span></span>
* <span data-ttu-id="d454a-1611">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="d454a-1611">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="d454a-1612">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="d454a-1612">Az.DataFactory</span></span>
* <span data-ttu-id="d454a-1613">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="d454a-1613">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="d454a-1614">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d454a-1614">Az.DataLakeStore</span></span>
* <span data-ttu-id="d454a-1615">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="d454a-1615">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="d454a-1616">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="d454a-1616">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="d454a-1617">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="d454a-1617">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="d454a-1618">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="d454a-1618">Az.IotHub</span></span>
* <span data-ttu-id="d454a-1619">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="d454a-1619">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="d454a-1620">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d454a-1620">Az.KeyVault</span></span>
* <span data-ttu-id="d454a-1621">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="d454a-1621">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-1622">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1622">Az.Network</span></span>
* <span data-ttu-id="d454a-1623">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="d454a-1623">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-1624">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1624">Az.Resources</span></span>
* <span data-ttu-id="d454a-1625">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="d454a-1625">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="d454a-1626">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="d454a-1626">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="d454a-1627">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="d454a-1627">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="d454a-1628">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="d454a-1628">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="d454a-1629">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="d454a-1629">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="d454a-1630">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="d454a-1630">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="d454a-1631">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="d454a-1631">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="d454a-1632">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d454a-1632">Az.ServiceFabric</span></span>
* <span data-ttu-id="d454a-1633">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="d454a-1633">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="d454a-1634">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="d454a-1634">Fix some error messages.</span></span>
* <span data-ttu-id="d454a-1635">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="d454a-1635">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="d454a-1636">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="d454a-1636">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="d454a-1637">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="d454a-1637">Az.SignalR</span></span>
* <span data-ttu-id="d454a-1638">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="d454a-1638">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-1639">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-1639">Az.Sql</span></span>
* <span data-ttu-id="d454a-1640">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="d454a-1640">Update incorrect online help URLs</span></span>
* <span data-ttu-id="d454a-1641">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="d454a-1641">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="d454a-1642">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="d454a-1642">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="d454a-1643">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="d454a-1643">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-1644">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-1644">Az.Storage</span></span>
* <span data-ttu-id="d454a-1645">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="d454a-1645">Update incorrect online help URLs</span></span>
* <span data-ttu-id="d454a-1646">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="d454a-1646">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="d454a-1647">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="d454a-1647">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="d454a-1648">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="d454a-1648">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="d454a-1649">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="d454a-1649">Az.TrafficManager</span></span>
* <span data-ttu-id="d454a-1650">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="d454a-1650">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="d454a-1651">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-1651">Az.Websites</span></span>
* <span data-ttu-id="d454a-1652">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="d454a-1652">Update incorrect online help URLs</span></span>
* <span data-ttu-id="d454a-1653">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="d454a-1653">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="d454a-1654">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="d454a-1654">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="d454a-1655">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="d454a-1655">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="d454a-1656">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-1656">Az.Accounts</span></span>
* <span data-ttu-id="d454a-1657">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="d454a-1657">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-1658">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1658">Az.Compute</span></span>
* <span data-ttu-id="d454a-1659">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="d454a-1659">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="d454a-1660">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="d454a-1660">Updated the description of ID in help files</span></span>
* <span data-ttu-id="d454a-1661">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-1661">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="d454a-1662">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d454a-1662">Az.DataLakeStore</span></span>
* <span data-ttu-id="d454a-1663">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="d454a-1663">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="d454a-1664">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="d454a-1664">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="d454a-1665">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="d454a-1665">Az.EventGrid</span></span>
* <span data-ttu-id="d454a-1666">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="d454a-1666">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="d454a-1667">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="d454a-1667">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="d454a-1668">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="d454a-1668">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="d454a-1669">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="d454a-1669">Event Time-To-Live,</span></span>
        - <span data-ttu-id="d454a-1670">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="d454a-1670">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="d454a-1671">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="d454a-1671">Dead letter endpoint.</span></span>
    - <span data-ttu-id="d454a-1672">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="d454a-1672">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="d454a-1673">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="d454a-1673">Event Time-To-Live,</span></span>
        - <span data-ttu-id="d454a-1674">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="d454a-1674">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="d454a-1675">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="d454a-1675">Dead letter endpoint.</span></span>
* <span data-ttu-id="d454a-1676">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="d454a-1676">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="d454a-1677">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="d454a-1677">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="d454a-1678">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="d454a-1678">Az.IotHub</span></span>
* <span data-ttu-id="d454a-1679">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="d454a-1679">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="d454a-1680">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="d454a-1680">Az.LogicApp</span></span>
* <span data-ttu-id="d454a-1681">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="d454a-1681">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-1682">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1682">Az.Resources</span></span>
* <span data-ttu-id="d454a-1683">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="d454a-1683">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="d454a-1684">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="d454a-1684">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="d454a-1685">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="d454a-1685">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="d454a-1686">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="d454a-1686">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="d454a-1687">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="d454a-1687">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="d454a-1688">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="d454a-1688">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="d454a-1689">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="d454a-1689">Az.SignalR</span></span>
* <span data-ttu-id="d454a-1690">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-1690">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-1691">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-1691">Az.Sql</span></span>
* <span data-ttu-id="d454a-1692">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="d454a-1692">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="d454a-1693">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-1693">Az.Storage</span></span>
* <span data-ttu-id="d454a-1694">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="d454a-1694">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="d454a-1695">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="d454a-1695">New-AzStorageContext</span></span>
* <span data-ttu-id="d454a-1696">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="d454a-1696">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="d454a-1697">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="d454a-1697">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="d454a-1698">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-1698">Az.Websites</span></span>
* <span data-ttu-id="d454a-1699">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="d454a-1699">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="d454a-1700">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-1700">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="d454a-1701">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="d454a-1701">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="d454a-1702">Geral</span><span class="sxs-lookup"><span data-stu-id="d454a-1702">General</span></span>

- <span data-ttu-id="d454a-1703">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="d454a-1703">General Availability of Az Module</span></span>
- <span data-ttu-id="d454a-1704">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="d454a-1704">Online help for each module</span></span>
- <span data-ttu-id="d454a-1705">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="d454a-1705">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="d454a-1706">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="d454a-1706">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="d454a-1707">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-1707">Az.Accounts</span></span>
- <span data-ttu-id="d454a-1708">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="d454a-1708">Changed from Az.Profile</span></span>
- <span data-ttu-id="d454a-1709">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="d454a-1709">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="d454a-1710">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d454a-1710">Az.ApiManagement</span></span>
- <span data-ttu-id="d454a-1711">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="d454a-1711">Fixes for #7002</span></span>
- <span data-ttu-id="d454a-1712">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="d454a-1712">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="d454a-1713">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="d454a-1713">Az.Batch</span></span>
- <span data-ttu-id="d454a-1714">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="d454a-1714">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="d454a-1715">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="d454a-1715">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="d454a-1716">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="d454a-1716">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="d454a-1717">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="d454a-1717">Az.Billing</span></span>
- <span data-ttu-id="d454a-1718">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="d454a-1718">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="d454a-1719">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1719">Az.CognitivServices</span></span>
- <span data-ttu-id="d454a-1720">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-1720">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="d454a-1721">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="d454a-1721">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="d454a-1722">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="d454a-1722">Az.ContainerInstance</span></span>
- <span data-ttu-id="d454a-1723">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="d454a-1723">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="d454a-1724">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="d454a-1724">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="d454a-1725">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="d454a-1725">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="d454a-1726">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d454a-1726">Az.DataLakeStore</span></span>
- <span data-ttu-id="d454a-1727">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="d454a-1727">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="d454a-1728">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="d454a-1728">Az.Monitor</span></span>
- <span data-ttu-id="d454a-1729">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="d454a-1729">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="d454a-1730">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="d454a-1730">Az.KeyVault</span></span>
- <span data-ttu-id="d454a-1731">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="d454a-1731">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="d454a-1732">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="d454a-1732">Az.MachineLearning</span></span>
- <span data-ttu-id="d454a-1733">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="d454a-1733">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="d454a-1734">Az.Media</span><span class="sxs-lookup"><span data-stu-id="d454a-1734">Az.Media</span></span>
- <span data-ttu-id="d454a-1735">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="d454a-1735">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="d454a-1736">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1736">Az.Network</span></span>
<span data-ttu-id="d454a-1737">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="d454a-1737">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="d454a-1738">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="d454a-1738">New cmdlets added:</span></span>
        - <span data-ttu-id="d454a-1739">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="d454a-1739">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="d454a-1740">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="d454a-1740">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="d454a-1741">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="d454a-1741">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="d454a-1742">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="d454a-1742">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="d454a-1743">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="d454a-1743">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="d454a-1744">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="d454a-1744">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="d454a-1745">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="d454a-1745">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="d454a-1746">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="d454a-1746">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="d454a-1747">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="d454a-1747">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="d454a-1748">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="d454a-1748">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="d454a-1749">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="d454a-1749">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="d454a-1750">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="d454a-1750">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="d454a-1751">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-1751">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="d454a-1752">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-1752">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="d454a-1753">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="d454a-1753">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="d454a-1754">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="d454a-1754">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="d454a-1755">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="d454a-1755">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="d454a-1756">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="d454a-1756">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="d454a-1757">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="d454a-1757">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="d454a-1758">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="d454a-1758">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="d454a-1759">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="d454a-1759">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="d454a-1760">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="d454a-1760">Az.OperationalInsights</span></span>
- <span data-ttu-id="d454a-1761">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="d454a-1761">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="d454a-1762">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="d454a-1762">Az.Profile</span></span>
- <span data-ttu-id="d454a-1763">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="d454a-1763">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-1764">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1764">Az.RecoveryServices</span></span>
- <span data-ttu-id="d454a-1765">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="d454a-1765">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="d454a-1766">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1766">Az.Resources</span></span>
- <span data-ttu-id="d454a-1767">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="d454a-1767">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="d454a-1768">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d454a-1768">Az.ServiceFabric</span></span>
- <span data-ttu-id="d454a-1769">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="d454a-1769">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="d454a-1770">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="d454a-1770">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="d454a-1771">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="d454a-1771">Az.SIgnalR</span></span>
- <span data-ttu-id="d454a-1772">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="d454a-1772">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="d454a-1773">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-1773">Az.Sql</span></span>
- <span data-ttu-id="d454a-1774">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="d454a-1774">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="d454a-1775">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="d454a-1775">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="d454a-1776">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="d454a-1776">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="d454a-1777">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-1777">Az.Storage</span></span>
- <span data-ttu-id="d454a-1778">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="d454a-1778">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="d454a-1779">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-1779">Az.Websites</span></span>
- <span data-ttu-id="d454a-1780">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="d454a-1780">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="d454a-1781">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="d454a-1781">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="d454a-1782">Geral</span><span class="sxs-lookup"><span data-stu-id="d454a-1782">General</span></span>

* <span data-ttu-id="d454a-1783">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="d454a-1783">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="d454a-1784">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1784">Az.Compute</span></span>

* <span data-ttu-id="d454a-1785">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="d454a-1785">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="d454a-1786">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d454a-1786">Az.DataLakeStore</span></span>

* <span data-ttu-id="d454a-1787">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="d454a-1787">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="d454a-1788">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="d454a-1788">Az.FrontDoor</span></span>

* <span data-ttu-id="d454a-1789">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="d454a-1789">Fixed some broken links</span></span>
    - <span data-ttu-id="d454a-1790">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="d454a-1790">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="d454a-1791">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="d454a-1791">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="d454a-1792">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1792">Az.RecoveryServices</span></span>

* <span data-ttu-id="d454a-1793">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-1793">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="d454a-1794">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="d454a-1794">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="d454a-1795">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1795">Az.Resources</span></span>

* <span data-ttu-id="d454a-1796">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="d454a-1796">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="d454a-1797">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="d454a-1797">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="d454a-1798">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-1798">Az.Sql</span></span>

* <span data-ttu-id="d454a-1799">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="d454a-1799">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="d454a-1800">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="d454a-1800">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="d454a-1801">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="d454a-1801">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="d454a-1802">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-1802">Az.Storage</span></span>

* <span data-ttu-id="d454a-1803">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="d454a-1803">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="d454a-1804">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="d454a-1804">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="d454a-1805">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="d454a-1805">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="d454a-1806">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="d454a-1806">Support Static Website configuration</span></span>
    - <span data-ttu-id="d454a-1807">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="d454a-1807">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="d454a-1808">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="d454a-1808">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="d454a-1809">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-1809">Az.Websites</span></span>

* <span data-ttu-id="d454a-1810">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="d454a-1810">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="d454a-1811">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="d454a-1811">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="d454a-1812">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-1812">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="d454a-1813">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="d454a-1813">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="d454a-1814">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d454a-1814">Az.ApiManagement</span></span>
* <span data-ttu-id="d454a-1815">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="d454a-1815">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="d454a-1816">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="d454a-1816">Az.Automation</span></span>
* <span data-ttu-id="d454a-1817">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="d454a-1817">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="d454a-1818">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="d454a-1818">Added Update Management cmdlets</span></span>
* <span data-ttu-id="d454a-1819">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="d454a-1819">Added Source Control cmdlets</span></span>
* <span data-ttu-id="d454a-1820">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="d454a-1820">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="d454a-1821">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="d454a-1821">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="d454a-1822">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1822">Az.Compute</span></span>
* <span data-ttu-id="d454a-1823">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="d454a-1823">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="d454a-1824">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="d454a-1824">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="d454a-1825">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="d454a-1825">Az.ContainerInstance</span></span>
* <span data-ttu-id="d454a-1826">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="d454a-1826">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="d454a-1827">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="d454a-1827">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="d454a-1828">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="d454a-1828">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="d454a-1829">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1829">Az.Network</span></span>
* <span data-ttu-id="d454a-1830">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="d454a-1830">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="d454a-1831">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="d454a-1831">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="d454a-1832">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="d454a-1832">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="d454a-1833">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="d454a-1833">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="d454a-1834">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="d454a-1834">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="d454a-1835">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="d454a-1835">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="d454a-1836">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="d454a-1836">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="d454a-1837">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="d454a-1837">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="d454a-1838">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="d454a-1838">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="d454a-1839">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="d454a-1839">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="d454a-1840">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="d454a-1840">Az.Relay</span></span>
* <span data-ttu-id="d454a-1841">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="d454a-1841">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="d454a-1842">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1842">Az.Resources</span></span>
* <span data-ttu-id="d454a-1843">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="d454a-1843">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="d454a-1844">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="d454a-1844">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="d454a-1845">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="d454a-1845">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="d454a-1846">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d454a-1846">Az.ServiceFabric</span></span>
* <span data-ttu-id="d454a-1847">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="d454a-1847">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="d454a-1848">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-1848">Az.Sql</span></span>
* <span data-ttu-id="d454a-1849">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="d454a-1849">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="d454a-1850">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="d454a-1850">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="d454a-1851">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="d454a-1851">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="d454a-1852">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="d454a-1852">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="d454a-1853">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="d454a-1853">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="d454a-1854">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="d454a-1854">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="d454a-1855">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="d454a-1855">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="d454a-1856">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="d454a-1856">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="d454a-1857">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="d454a-1857">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="d454a-1858">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="d454a-1858">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="d454a-1859">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="d454a-1859">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="d454a-1860">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="d454a-1860">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="d454a-1861">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="d454a-1861">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="d454a-1862">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="d454a-1862">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="d454a-1863">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="d454a-1863">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="d454a-1864">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="d454a-1864">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="d454a-1865">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="d454a-1865">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="d454a-1866">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="d454a-1866">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="d454a-1867">Geral</span><span class="sxs-lookup"><span data-stu-id="d454a-1867">General</span></span>
* <span data-ttu-id="d454a-1868">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="d454a-1868">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="d454a-1869">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="d454a-1869">Az.Profile</span></span>
* <span data-ttu-id="d454a-1870">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="d454a-1870">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="d454a-1871">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="d454a-1871">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="d454a-1872">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="d454a-1872">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="d454a-1873">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="d454a-1873">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="d454a-1874">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="d454a-1874">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="d454a-1875">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="d454a-1875">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="d454a-1876">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="d454a-1876">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="d454a-1877">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1877">Az.CognitiveServices</span></span>
* <span data-ttu-id="d454a-1878">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="d454a-1878">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-1879">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1879">Az.Compute</span></span>
* <span data-ttu-id="d454a-1880">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="d454a-1880">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="d454a-1881">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="d454a-1881">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="d454a-1882">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="d454a-1882">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="d454a-1883">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d454a-1883">Az.DataLakeStore</span></span>
* <span data-ttu-id="d454a-1884">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="d454a-1884">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="d454a-1885">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="d454a-1885">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="d454a-1886">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="d454a-1886">Az.Insights</span></span>
* <span data-ttu-id="d454a-1887">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="d454a-1887">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="d454a-1888">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="d454a-1888">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="d454a-1889">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="d454a-1889">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="d454a-1890">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="d454a-1890">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-1891">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1891">Az.Network</span></span>
* <span data-ttu-id="d454a-1892">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="d454a-1892">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="d454a-1893">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="d454a-1893">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="d454a-1894">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="d454a-1894">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="d454a-1895">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="d454a-1895">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="d454a-1896">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="d454a-1896">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="d454a-1897">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="d454a-1897">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="d454a-1898">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="d454a-1898">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="d454a-1899">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="d454a-1899">Az.PolicyInsights</span></span>
* <span data-ttu-id="d454a-1900">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="d454a-1900">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-1901">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1901">Az.Resources</span></span>
* <span data-ttu-id="d454a-1902">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="d454a-1902">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="d454a-1903">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="d454a-1903">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="d454a-1904">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d454a-1904">Az.ServiceBus</span></span>
* <span data-ttu-id="d454a-1905">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="d454a-1905">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="d454a-1906">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d454a-1906">Az.ServiceFabric</span></span>
* <span data-ttu-id="d454a-1907">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="d454a-1907">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="d454a-1908">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="d454a-1908">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="d454a-1909">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="d454a-1909">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="d454a-1910">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="d454a-1910">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="d454a-1911">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="d454a-1911">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="d454a-1912">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="d454a-1912">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="d454a-1913">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="d454a-1913">Az.Profile</span></span>
* <span data-ttu-id="d454a-1914">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="d454a-1914">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="d454a-1915">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="d454a-1915">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-1916">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1916">Az.Compute</span></span>
* <span data-ttu-id="d454a-1917">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="d454a-1917">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="d454a-1918">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="d454a-1918">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="d454a-1919">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d454a-1919">Az.DataLakeStore</span></span>
* <span data-ttu-id="d454a-1920">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="d454a-1920">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="d454a-1921">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-1921">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="d454a-1922">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="d454a-1922">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="d454a-1923">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="d454a-1923">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="d454a-1924">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="d454a-1924">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-1925">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1925">Az.Network</span></span>
* <span data-ttu-id="d454a-1926">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="d454a-1926">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="d454a-1927">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="d454a-1927">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-1928">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1928">Az.Resources</span></span>
* <span data-ttu-id="d454a-1929">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="d454a-1929">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="d454a-1930">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="d454a-1930">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="d454a-1931">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="d454a-1931">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="d454a-1932">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="d454a-1932">Azure.Storage</span></span>
* <span data-ttu-id="d454a-1933">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="d454a-1933">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="d454a-1934">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="d454a-1934">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="d454a-1935">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="d454a-1935">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="d454a-1936">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="d454a-1936">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="d454a-1937">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="d454a-1937">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="d454a-1938">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="d454a-1938">Az.CognitiveServices</span></span>
* <span data-ttu-id="d454a-1939">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="d454a-1939">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="d454a-1940">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="d454a-1940">Az.Compute</span></span>
* <span data-ttu-id="d454a-1941">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="d454a-1941">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="d454a-1942">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="d454a-1942">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="d454a-1943">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="d454a-1943">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="d454a-1944">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="d454a-1944">Az.DataFactoryV2</span></span>
* <span data-ttu-id="d454a-1945">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="d454a-1945">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="d454a-1946">Az.Network</span><span class="sxs-lookup"><span data-stu-id="d454a-1946">Az.Network</span></span>
* <span data-ttu-id="d454a-1947">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="d454a-1947">Added NetworkProfile functionality.</span></span> <span data-ttu-id="d454a-1948">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="d454a-1948">new cmdlets added</span></span>
    - <span data-ttu-id="d454a-1949">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d454a-1949">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="d454a-1950">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d454a-1950">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="d454a-1951">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d454a-1951">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="d454a-1952">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d454a-1952">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="d454a-1953">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-1953">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="d454a-1954">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-1954">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="d454a-1955">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="d454a-1955">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="d454a-1956">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="d454a-1956">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="d454a-1957">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="d454a-1957">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="d454a-1958">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="d454a-1958">Az.RedisCache</span></span>
* <span data-ttu-id="d454a-1959">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="d454a-1959">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="d454a-1960">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="d454a-1960">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="d454a-1961">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="d454a-1961">Az.Resources</span></span>
* <span data-ttu-id="d454a-1962">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="d454a-1962">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="d454a-1963">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="d454a-1963">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="d454a-1964">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="d454a-1964">Az.Sql</span></span>
* <span data-ttu-id="d454a-1965">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="d454a-1965">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="d454a-1966">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="d454a-1966">Az.Websites</span></span>
* <span data-ttu-id="d454a-1967">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="d454a-1967">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="d454a-1968">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="d454a-1968">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="d454a-1969">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="d454a-1969">0.2.0 - September 2018</span></span>
 <span data-ttu-id="d454a-1970">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="d454a-1970">Initial Release</span></span>
