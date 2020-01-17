---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/09/2020
ms.openlocfilehash: 3806a1c609a71c53c0bddc5bafd51d845c0c296e
ms.sourcegitcommit: 16904e0a72c55fb81248e0252769defb86c50f36
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/10/2020
ms.locfileid: "75831649"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="183c8-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="183c8-103">Azure PowerShell release notes</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="183c8-104">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="183c8-104">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="183c8-105">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-105">Az.Accounts</span></span>
* <span data-ttu-id="183c8-106">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="183c8-106">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="183c8-107">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="183c8-107">Az.Cdn</span></span>
* <span data-ttu-id="183c8-108">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="183c8-108">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-109">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-109">Az.Compute</span></span>
* <span data-ttu-id="183c8-110">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="183c8-110">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="183c8-111">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="183c8-111">Az.ContainerInstance</span></span>
* <span data-ttu-id="183c8-112">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="183c8-112">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="183c8-113">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="183c8-113">Az.DataBoxEdge</span></span>
* <span data-ttu-id="183c8-114">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="183c8-114">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="183c8-115">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="183c8-115">Get the Edge Storage Container</span></span>
* <span data-ttu-id="183c8-116">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="183c8-116">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="183c8-117">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="183c8-117">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="183c8-118">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="183c8-118">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="183c8-119">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="183c8-119">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="183c8-120">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="183c8-120">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="183c8-121">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="183c8-121">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="183c8-122">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="183c8-122">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="183c8-123">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="183c8-123">Get the Edge Storage Account</span></span>
* <span data-ttu-id="183c8-124">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="183c8-124">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="183c8-125">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="183c8-125">Create new Edge Storage Account</span></span>
* <span data-ttu-id="183c8-126">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="183c8-126">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="183c8-127">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="183c8-127">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="183c8-128">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="183c8-128">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="183c8-129">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="183c8-129">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="183c8-130">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="183c8-130">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="183c8-131">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="183c8-131">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="183c8-132">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="183c8-132">Az.DataFactory</span></span>
* <span data-ttu-id="183c8-133">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="183c8-133">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="183c8-134">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="183c8-134">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="183c8-135">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="183c8-135">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="183c8-136">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="183c8-136">Az.DevTestLabs</span></span>
* <span data-ttu-id="183c8-137">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="183c8-137">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="183c8-138">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="183c8-138">Az.EventHub</span></span>
* <span data-ttu-id="183c8-139">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="183c8-139">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="183c8-140">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="183c8-140">Az.HDInsight</span></span>
* <span data-ttu-id="183c8-141">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="183c8-141">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="183c8-142">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="183c8-142">Az.MachineLearning</span></span>
* <span data-ttu-id="183c8-143">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="183c8-143">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="183c8-144">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="183c8-144">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="183c8-145">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="183c8-145">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="183c8-146">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="183c8-146">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="183c8-147">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="183c8-147">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="183c8-148">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="183c8-148">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="183c8-149">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="183c8-149">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="183c8-150">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="183c8-150">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-151">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-151">Az.Network</span></span>
* <span data-ttu-id="183c8-152">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="183c8-152">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-153">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-153">Az.RecoveryServices</span></span>
* <span data-ttu-id="183c8-154">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com leys geridos pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-154">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed leys for Azure to Azure provider.</span></span>
* <span data-ttu-id="183c8-155">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-155">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="183c8-156">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-156">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="183c8-157">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-157">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-158">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-158">Az.Resources</span></span>
* <span data-ttu-id="183c8-159">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="183c8-159">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-160">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-160">Az.Sql</span></span>
* <span data-ttu-id="183c8-161">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="183c8-161">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="183c8-162">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="183c8-162">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="183c8-163">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="183c8-163">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="183c8-164">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="183c8-164">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="183c8-165">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-165">Az.Storage</span></span>
* <span data-ttu-id="183c8-166">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="183c8-166">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="183c8-167">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="183c8-167">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="183c8-168">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="183c8-168">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span> 
    - <span data-ttu-id="183c8-169">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="183c8-169">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="183c8-170">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-170">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="183c8-171">Geral</span><span class="sxs-lookup"><span data-stu-id="183c8-171">General</span></span>
* <span data-ttu-id="183c8-172">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="183c8-172">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="183c8-173">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-173">Az.Accounts</span></span>
* <span data-ttu-id="183c8-174">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="183c8-174">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="183c8-175">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="183c8-175">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="183c8-176">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="183c8-176">Az.Batch</span></span>
* <span data-ttu-id="183c8-177">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="183c8-177">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="183c8-178">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="183c8-178">Az.DataFactory</span></span>
* <span data-ttu-id="183c8-179">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="183c8-179">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="183c8-180">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="183c8-180">Az.FrontDoor</span></span>
* <span data-ttu-id="183c8-181">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="183c8-181">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="183c8-182">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="183c8-182">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="183c8-183">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="183c8-183">Az.HealthcareApis</span></span>
* <span data-ttu-id="183c8-184">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="183c8-184">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="183c8-185">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="183c8-185">Az.KeyVault</span></span>
* <span data-ttu-id="183c8-186">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="183c8-186">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="183c8-187">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="183c8-187">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="183c8-188">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="183c8-188">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="183c8-189">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="183c8-189">Az.Monitor</span></span>
* <span data-ttu-id="183c8-190">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="183c8-190">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="183c8-191">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="183c8-191">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="183c8-192">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="183c8-192">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-193">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-193">Az.Network</span></span>
* <span data-ttu-id="183c8-194">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="183c8-194">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-195">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-195">Az.Resources</span></span>
* <span data-ttu-id="183c8-196">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="183c8-196">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="183c8-197">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="183c8-197">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-198">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-198">Az.Sql</span></span>
* <span data-ttu-id="183c8-199">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="183c8-199">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="183c8-200">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-200">Az.Storage</span></span>
* <span data-ttu-id="183c8-201">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="183c8-201">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="183c8-202">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="183c8-202">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="183c8-203">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="183c8-203">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="183c8-204">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="183c8-204">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="183c8-205">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="183c8-205">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="183c8-206">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="183c8-206">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="183c8-207">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="183c8-207">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span> 
    - <span data-ttu-id="183c8-208">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="183c8-208">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="183c8-209">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="183c8-209">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="183c8-210">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="183c8-210">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="183c8-211">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="183c8-211">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="183c8-212">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="183c8-212">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="183c8-213">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="183c8-213">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="183c8-214">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-214">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="183c8-215">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="183c8-215">Highlights since the last major release</span></span>
* <span data-ttu-id="183c8-216">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="183c8-216">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="183c8-217">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="183c8-217">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-218">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-218">Az.Compute</span></span>
* <span data-ttu-id="183c8-219">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="183c8-219">VM Reapply feature</span></span>
    - <span data-ttu-id="183c8-220">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="183c8-220">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="183c8-221">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="183c8-221">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="183c8-222">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="183c8-222">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="183c8-223">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="183c8-223">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="183c8-224">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="183c8-224">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="183c8-225">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="183c8-225">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="183c8-226">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="183c8-226">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="183c8-227">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="183c8-227">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="183c8-228">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="183c8-228">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="183c8-229">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="183c8-229">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="183c8-230">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="183c8-230">Az.DataBoxEdge</span></span>
* <span data-ttu-id="183c8-231">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="183c8-231">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="183c8-232">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="183c8-232">Get the Order</span></span>
* <span data-ttu-id="183c8-233">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="183c8-233">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="183c8-234">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="183c8-234">Create new Order</span></span>
* <span data-ttu-id="183c8-235">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="183c8-235">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="183c8-236">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="183c8-236">Remove the Order</span></span>
* <span data-ttu-id="183c8-237">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="183c8-237">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="183c8-238">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="183c8-238">Now creates Local Share</span></span>
* <span data-ttu-id="183c8-239">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="183c8-239">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="183c8-240">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="183c8-240">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="183c8-241">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="183c8-241">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="183c8-242">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="183c8-242">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="183c8-243">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="183c8-243">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="183c8-244">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="183c8-244">Gets the information about Triggers</span></span>
* <span data-ttu-id="183c8-245">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="183c8-245">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="183c8-246">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="183c8-246">Create new Triggers</span></span>
* <span data-ttu-id="183c8-247">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="183c8-247">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="183c8-248">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="183c8-248">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="183c8-249">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="183c8-249">Az.DataFactory</span></span>
* <span data-ttu-id="183c8-250">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="183c8-250">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="183c8-251">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="183c8-251">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="183c8-252">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="183c8-252">Az.DataLakeStore</span></span>
* <span data-ttu-id="183c8-253">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="183c8-253">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="183c8-254">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="183c8-254">Az.EventHub</span></span>
* <span data-ttu-id="183c8-255">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="183c8-255">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="183c8-256">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="183c8-256">Az.FrontDoor</span></span>
* <span data-ttu-id="183c8-257">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="183c8-257">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="183c8-258">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="183c8-258">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="183c8-259">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="183c8-259">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="183c8-260">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="183c8-260">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-261">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-261">Az.Network</span></span>
* <span data-ttu-id="183c8-262">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="183c8-262">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="183c8-263">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="183c8-263">Az.PrivateDns</span></span>
* <span data-ttu-id="183c8-264">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="183c8-264">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-265">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-265">Az.RecoveryServices</span></span>
* <span data-ttu-id="183c8-266">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="183c8-266">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="183c8-267">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="183c8-267">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="183c8-268">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="183c8-268">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="183c8-269">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="183c8-269">Az.RedisCache</span></span>
* <span data-ttu-id="183c8-270">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="183c8-270">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="183c8-271">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="183c8-271">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="183c8-272">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="183c8-272">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-273">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-273">Az.Resources</span></span>
- <span data-ttu-id="183c8-274">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="183c8-274">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="183c8-275">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="183c8-275">Updated create policy definition help example</span></span>
- <span data-ttu-id="183c8-276">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="183c8-276">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="183c8-277">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="183c8-277">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="183c8-278">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="183c8-278">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-279">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-279">Az.Sql</span></span>
* <span data-ttu-id="183c8-280">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="183c8-280">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="183c8-281">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="183c8-281">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="183c8-282">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-282">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="183c8-283">Geral</span><span class="sxs-lookup"><span data-stu-id="183c8-283">General</span></span>
* <span data-ttu-id="183c8-284">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="183c8-284">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="183c8-285">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-285">Az.Accounts</span></span>
* <span data-ttu-id="183c8-286">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="183c8-286">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="183c8-287">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="183c8-287">Az.Advisor</span></span>
* <span data-ttu-id="183c8-288">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="183c8-288">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="183c8-289">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="183c8-289">Az.Batch</span></span>
* <span data-ttu-id="183c8-290">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="183c8-290">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="183c8-291">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="183c8-291">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="183c8-292">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="183c8-292">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="183c8-293">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="183c8-293">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="183c8-294">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="183c8-294">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="183c8-295">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="183c8-295">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="183c8-296">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="183c8-296">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="183c8-297">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="183c8-297">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="183c8-298">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="183c8-298">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="183c8-299">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="183c8-299">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="183c8-300">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="183c8-300">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="183c8-301">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="183c8-301">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="183c8-302">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="183c8-302">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="183c8-303">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="183c8-303">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="183c8-304">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="183c8-304">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="183c8-305">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="183c8-305">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="183c8-306">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="183c8-306">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="183c8-307">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="183c8-307">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="183c8-308">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="183c8-308">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="183c8-309">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="183c8-309">This operation is no longer supported.</span></span>
* <span data-ttu-id="183c8-310">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="183c8-310">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="183c8-311">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="183c8-311">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="183c8-312">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="183c8-312">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="183c8-313">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="183c8-313">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span> 
  - <span data-ttu-id="183c8-314">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="183c8-314">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="183c8-315">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="183c8-315">New non-verified images are also now returned.</span></span> <span data-ttu-id="183c8-316">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="183c8-316">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="183c8-317">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="183c8-317">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="183c8-318">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="183c8-318">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="183c8-319">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="183c8-319">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="183c8-320">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="183c8-320">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="183c8-321">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="183c8-321">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="183c8-322">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="183c8-322">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="183c8-323">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="183c8-323">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="183c8-324">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="183c8-324">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="183c8-325">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="183c8-325">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="183c8-326">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="183c8-326">Az.Cdn</span></span>
* <span data-ttu-id="183c8-327">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="183c8-327">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="183c8-328">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="183c8-328">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-329">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-329">Az.Compute</span></span>
* <span data-ttu-id="183c8-330">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="183c8-330">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="183c8-331">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="183c8-331">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="183c8-332">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span><span class="sxs-lookup"><span data-stu-id="183c8-332">DiskEncryptionSetId parameter is added to the following cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span></span>        
        <span data-ttu-id="183c8-333">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="183c8-333">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="183c8-334">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-334">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="183c8-335">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-335">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="183c8-336">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="183c8-336">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="183c8-337">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="183c8-337">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="183c8-338">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="183c8-338">Breaking changes</span></span>
    - <span data-ttu-id="183c8-339">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="183c8-339">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="183c8-340">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="183c8-340">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="183c8-341">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="183c8-341">Az.DataFactory</span></span>
* <span data-ttu-id="183c8-342">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="183c8-342">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="183c8-343">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="183c8-343">Az.DataLakeStore</span></span>
* <span data-ttu-id="183c8-344">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="183c8-344">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="183c8-345">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="183c8-345">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="183c8-346">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="183c8-346">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="183c8-347">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="183c8-347">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="183c8-348">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="183c8-348">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="183c8-349">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="183c8-349">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="183c8-350">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="183c8-350">Az.FrontDoor</span></span>
* <span data-ttu-id="183c8-351">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="183c8-351">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="183c8-352">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="183c8-352">Az.HDInsight</span></span>
* <span data-ttu-id="183c8-353">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="183c8-353">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="183c8-354">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="183c8-354">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="183c8-355">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="183c8-355">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="183c8-356">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="183c8-356">Removed five cmdlets:</span></span>
    - <span data-ttu-id="183c8-357">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="183c8-357">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="183c8-358">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="183c8-358">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="183c8-359">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="183c8-359">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="183c8-360">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="183c8-360">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="183c8-361">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="183c8-361">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="183c8-362">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="183c8-362">Added three cmdlets:</span></span>
    - <span data-ttu-id="183c8-363">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="183c8-363">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="183c8-364">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="183c8-364">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="183c8-365">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="183c8-365">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="183c8-366">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="183c8-366">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="183c8-367">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="183c8-367">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="183c8-368">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="183c8-368">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="183c8-369">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="183c8-369">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="183c8-370">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="183c8-370">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="183c8-371">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="183c8-371">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="183c8-372">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="183c8-372">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="183c8-373">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="183c8-373">Added some scenario test cases.</span></span>
* <span data-ttu-id="183c8-374">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="183c8-374">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="183c8-375">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="183c8-375">Az.IotHub</span></span>
* <span data-ttu-id="183c8-376">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="183c8-376">Breaking changes:</span></span>
    - <span data-ttu-id="183c8-377">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="183c8-377">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="183c8-378">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="183c8-378">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="183c8-379">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="183c8-379">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="183c8-380">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="183c8-380">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="183c8-381">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="183c8-381">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="183c8-382">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="183c8-382">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="183c8-383">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="183c8-383">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="183c8-384">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="183c8-384">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="183c8-385">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="183c8-385">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="183c8-386">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="183c8-386">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="183c8-387">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="183c8-387">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="183c8-388">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="183c8-388">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-389">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-389">Az.RecoveryServices</span></span>
* <span data-ttu-id="183c8-390">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-390">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="183c8-391">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-391">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="183c8-392">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-392">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="183c8-393">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-393">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="183c8-394">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-394">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="183c8-395">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-395">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="183c8-396">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-396">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="183c8-397">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-397">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="183c8-398">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="183c8-398">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-399">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-399">Az.Resources</span></span>
* <span data-ttu-id="183c8-400">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="183c8-400">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-401">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-401">Az.Network</span></span>
* <span data-ttu-id="183c8-402">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="183c8-402">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="183c8-403">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="183c8-403">Updated cmdlet:</span></span>
        - <span data-ttu-id="183c8-404">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-404">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="183c8-405">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-405">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="183c8-406">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-406">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="183c8-407">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-407">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="183c8-408">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-408">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="183c8-409">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="183c8-409">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="183c8-410">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="183c8-410">New cmdlet:</span></span>
        - <span data-ttu-id="183c8-411">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="183c8-411">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="183c8-412">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="183c8-412">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="183c8-413">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="183c8-413">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="183c8-414">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-414">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="183c8-415">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="183c8-415">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="183c8-416">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="183c8-416">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="183c8-417">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="183c8-417">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="183c8-418">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="183c8-418">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="183c8-419">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="183c8-419">New cmdlets added:</span></span>
        - <span data-ttu-id="183c8-420">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="183c8-420">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="183c8-421">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="183c8-421">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="183c8-422">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="183c8-422">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="183c8-423">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="183c8-423">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="183c8-424">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="183c8-424">Set-AzVirtualHub</span></span>
* <span data-ttu-id="183c8-425">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="183c8-425">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="183c8-426">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="183c8-426">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="183c8-427">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="183c8-427">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="183c8-428">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="183c8-428">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="183c8-429">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="183c8-429">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="183c8-430">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="183c8-430">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="183c8-431">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-431">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="183c8-432">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="183c8-432">New cmdlets added:</span></span>
        - <span data-ttu-id="183c8-433">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-433">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="183c8-434">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="183c8-434">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="183c8-435">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="183c8-435">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="183c8-436">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="183c8-436">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="183c8-437">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="183c8-437">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="183c8-438">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="183c8-438">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="183c8-439">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="183c8-439">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="183c8-440">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="183c8-440">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="183c8-441">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="183c8-441">New cmdlets added:</span></span>
        - <span data-ttu-id="183c8-442">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="183c8-442">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="183c8-443">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="183c8-443">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="183c8-444">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="183c8-444">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="183c8-445">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="183c8-445">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="183c8-446">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="183c8-446">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="183c8-447">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="183c8-447">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="183c8-448">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="183c8-448">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="183c8-449">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="183c8-449">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="183c8-450">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="183c8-450">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="183c8-451">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="183c8-451">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="183c8-452">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="183c8-452">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="183c8-453">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="183c8-453">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="183c8-454">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="183c8-454">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="183c8-455">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="183c8-455">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="183c8-456">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="183c8-456">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="183c8-457">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="183c8-457">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="183c8-458">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="183c8-458">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="183c8-459">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="183c8-459">New cmdlets added:</span></span>
        - <span data-ttu-id="183c8-460">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="183c8-460">New-AzIpGroup</span></span>
        - <span data-ttu-id="183c8-461">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="183c8-461">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="183c8-462">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="183c8-462">Get-AzIpGroup</span></span>
        - <span data-ttu-id="183c8-463">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="183c8-463">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="183c8-464">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="183c8-464">Az.ServiceFabric</span></span>
* <span data-ttu-id="183c8-465">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="183c8-465">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-466">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-466">Az.Sql</span></span>
* <span data-ttu-id="183c8-467">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="183c8-467">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="183c8-468">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="183c8-468">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="183c8-469">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="183c8-469">Removed deprecated aliases:</span></span>
* <span data-ttu-id="183c8-470">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="183c8-470">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="183c8-471">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="183c8-471">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="183c8-472">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="183c8-472">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="183c8-473">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="183c8-473">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="183c8-474">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="183c8-474">Deprecate Advanced Threat Detection Settings cmdlets</span></span> 
* <span data-ttu-id="183c8-475">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="183c8-475">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="183c8-476">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-476">Az.Storage</span></span>
* <span data-ttu-id="183c8-477">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="183c8-477">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="183c8-478">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="183c8-478">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="183c8-479">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="183c8-479">Set-AzStorageAccount</span></span>
* <span data-ttu-id="183c8-480">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="183c8-480">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="183c8-481">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="183c8-481">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="183c8-482">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="183c8-482">Close-AzStorageFileHandle</span></span>
    
## <a name="280---october-2019"></a><span data-ttu-id="183c8-483">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-483">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="183c8-484">Geral</span><span class="sxs-lookup"><span data-stu-id="183c8-484">General</span></span>
* <span data-ttu-id="183c8-485">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="183c8-485">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="183c8-486">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-486">Az.Accounts</span></span>
* <span data-ttu-id="183c8-487">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="183c8-487">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="183c8-488">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="183c8-488">Az.ApiManagement</span></span>
* <span data-ttu-id="183c8-489">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="183c8-489">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="183c8-490">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="183c8-490">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="183c8-491">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="183c8-491">Az.Automation</span></span>
* <span data-ttu-id="183c8-492">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="183c8-492">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="183c8-493">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="183c8-493">Az.Batch</span></span>
* <span data-ttu-id="183c8-494">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="183c8-494">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-495">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-495">Az.Compute</span></span>
* <span data-ttu-id="183c8-496">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="183c8-496">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="183c8-497">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="183c8-497">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="183c8-498">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="183c8-498">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="183c8-499">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="183c8-499">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="183c8-500">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="183c8-500">Az.DataFactory</span></span>
* <span data-ttu-id="183c8-501">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="183c8-501">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="183c8-502">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="183c8-502">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="183c8-503">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="183c8-503">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="183c8-504">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="183c8-504">Az.DataLakeStore</span></span>
* <span data-ttu-id="183c8-505">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="183c8-505">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="183c8-506">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="183c8-506">Az.HealthcareApis</span></span>
* <span data-ttu-id="183c8-507">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="183c8-507">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="183c8-508">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="183c8-508">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="183c8-509">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="183c8-509">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="183c8-510">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="183c8-510">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="183c8-511">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="183c8-511">Az.IotHub</span></span>
* <span data-ttu-id="183c8-512">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="183c8-512">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="183c8-513">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="183c8-513">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="183c8-514">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="183c8-514">Az.Monitor</span></span>
* <span data-ttu-id="183c8-515">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="183c8-515">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="183c8-516">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="183c8-516">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="183c8-517">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="183c8-517">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="183c8-518">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="183c8-518">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-519">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-519">Az.Network</span></span>
* <span data-ttu-id="183c8-520">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="183c8-520">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="183c8-521">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="183c8-521">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="183c8-522">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="183c8-522">New cmdlets added:</span></span>
        - <span data-ttu-id="183c8-523">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="183c8-523">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="183c8-524">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-524">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="183c8-525">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="183c8-525">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="183c8-526">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="183c8-526">Updated cmdlets:</span></span>
        - <span data-ttu-id="183c8-527">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-527">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="183c8-528">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-528">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="183c8-529">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-529">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="183c8-530">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="183c8-530">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="183c8-531">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="183c8-531">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="183c8-532">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="183c8-532">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="183c8-533">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="183c8-533">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="183c8-534">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="183c8-534">Az.RedisCache</span></span>
* <span data-ttu-id="183c8-535">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="183c8-535">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-536">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-536">Az.Sql</span></span>
* <span data-ttu-id="183c8-537">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="183c8-537">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="183c8-538">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-538">Az.Storage</span></span>
* <span data-ttu-id="183c8-539">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="183c8-539">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="183c8-540">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="183c8-540">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="183c8-541">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="183c8-541">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="183c8-542">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="183c8-542">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="183c8-543">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="183c8-543">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="183c8-544">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="183c8-544">Az.StorageSync</span></span>
* <span data-ttu-id="183c8-545">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="183c8-545">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="183c8-546">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="183c8-546">Az.Websites</span></span>
* <span data-ttu-id="183c8-547">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="183c8-547">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="183c8-548">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-548">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="183c8-549">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="183c8-549">Az.ApiManagement</span></span>
* <span data-ttu-id="183c8-550">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="183c8-550">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="183c8-551">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="183c8-551">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="183c8-552">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="183c8-552">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="183c8-553">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="183c8-553">Az.Automation</span></span>
* <span data-ttu-id="183c8-554">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="183c8-554">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="183c8-555">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="183c8-555">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="183c8-556">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="183c8-556">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-557">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-557">Az.Compute</span></span>
* <span data-ttu-id="183c8-558">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-558">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="183c8-559">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-559">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="183c8-560">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="183c8-560">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="183c8-561">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="183c8-561">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="183c8-562">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="183c8-562">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="183c8-563">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="183c8-563">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="183c8-564">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="183c8-564">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="183c8-565">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="183c8-565">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="183c8-566">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="183c8-566">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="183c8-567">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="183c8-567">Az.DataFactory</span></span>
* <span data-ttu-id="183c8-568">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="183c8-568">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="183c8-569">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="183c8-569">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="183c8-570">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="183c8-570">Az.HDInsight</span></span>
* <span data-ttu-id="183c8-571">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="183c8-571">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="183c8-572">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="183c8-572">Az.IotHub</span></span>
* <span data-ttu-id="183c8-573">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="183c8-573">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="183c8-574">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="183c8-574">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="183c8-575">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="183c8-575">New cmdlets are:</span></span>
    - <span data-ttu-id="183c8-576">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="183c8-576">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="183c8-577">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="183c8-577">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="183c8-578">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="183c8-578">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="183c8-579">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="183c8-579">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="183c8-580">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="183c8-580">Az.Monitor</span></span>
* <span data-ttu-id="183c8-581">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="183c8-581">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="183c8-582">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="183c8-582">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="183c8-583">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="183c8-583">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="183c8-584">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="183c8-584">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="183c8-585">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="183c8-585">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="183c8-586">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="183c8-586">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="183c8-587">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="183c8-587">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="183c8-588">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="183c8-588">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="183c8-589">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="183c8-589">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="183c8-590">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="183c8-590">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="183c8-591">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="183c8-591">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="183c8-592">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="183c8-592">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="183c8-593">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="183c8-593">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="183c8-594">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="183c8-594">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="183c8-595">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="183c8-595">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="183c8-596">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="183c8-596">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="183c8-597">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="183c8-597">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="183c8-598">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="183c8-598">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="183c8-599">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="183c8-599">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="183c8-600">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="183c8-600">Overall improved help files</span></span>
* <span data-ttu-id="183c8-601">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="183c8-601">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-602">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-602">Az.Network</span></span>
* <span data-ttu-id="183c8-603">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="183c8-603">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="183c8-604">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="183c8-604">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="183c8-605">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="183c8-605">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="183c8-606">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="183c8-606">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="183c8-607">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="183c8-607">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="183c8-608">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="183c8-608">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="183c8-609">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="183c8-609">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="183c8-610">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="183c8-610">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="183c8-611">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="183c8-611">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="183c8-612">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="183c8-612">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="183c8-613">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="183c8-613">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="183c8-614">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="183c8-614">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="183c8-615">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="183c8-615">New cmdlets</span></span>
        - <span data-ttu-id="183c8-616">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="183c8-616">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="183c8-617">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-617">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="183c8-618">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="183c8-618">Updated cmdlet:</span></span>
        - <span data-ttu-id="183c8-619">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="183c8-619">New-VpnSite</span></span>
        - <span data-ttu-id="183c8-620">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="183c8-620">Update-VpnSite</span></span>
        - <span data-ttu-id="183c8-621">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-621">New-VpnConnection</span></span>
        - <span data-ttu-id="183c8-622">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-622">Update-VpnConnection</span></span>
* <span data-ttu-id="183c8-623">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="183c8-623">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-624">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-624">Az.RecoveryServices</span></span>
* <span data-ttu-id="183c8-625">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="183c8-625">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="183c8-626">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="183c8-626">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-627">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-627">Az.Resources</span></span>
* <span data-ttu-id="183c8-628">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="183c8-628">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="183c8-629">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="183c8-629">Az.ServiceFabric</span></span>
* <span data-ttu-id="183c8-630">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="183c8-630">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="183c8-631">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="183c8-631">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="183c8-632">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="183c8-632">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="183c8-633">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="183c8-633">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="183c8-634">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="183c8-634">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="183c8-635">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="183c8-635">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="183c8-636">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="183c8-636">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="183c8-637">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="183c8-637">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="183c8-638">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="183c8-638">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="183c8-639">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="183c8-639">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="183c8-640">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="183c8-640">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="183c8-641">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="183c8-641">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="183c8-642">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="183c8-642">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="183c8-643">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="183c8-643">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="183c8-644">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="183c8-644">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="183c8-645">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="183c8-645">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="183c8-646">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="183c8-646">Az.SignalR</span></span>
* <span data-ttu-id="183c8-647">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="183c8-647">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-648">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-648">Az.Sql</span></span>
* <span data-ttu-id="183c8-649">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="183c8-649">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="183c8-650">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="183c8-650">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="183c8-651">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="183c8-651">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="183c8-652">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="183c8-652">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="183c8-653">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="183c8-653">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="183c8-654">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-654">Az.Storage</span></span>
* <span data-ttu-id="183c8-655">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="183c8-655">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="183c8-656">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="183c8-656">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="183c8-657">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="183c8-657">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="183c8-658">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="183c8-658">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="183c8-659">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="183c8-659">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="183c8-660">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="183c8-660">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="183c8-661">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="183c8-661">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="183c8-662">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="183c8-662">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="183c8-663">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="183c8-663">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="183c8-664">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="183c8-664">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="183c8-665">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="183c8-665">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="183c8-666">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="183c8-666">Az.Websites</span></span>
* <span data-ttu-id="183c8-667">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="183c8-667">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="183c8-668">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="183c8-668">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="183c8-669">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="183c8-669">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="183c8-670">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-670">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="183c8-671">Geral</span><span class="sxs-lookup"><span data-stu-id="183c8-671">General</span></span>
* <span data-ttu-id="183c8-672">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="183c8-672">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="183c8-673">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-673">Az.Accounts</span></span>
* <span data-ttu-id="183c8-674">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="183c8-674">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="183c8-675">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="183c8-675">Az.Aks</span></span>
* <span data-ttu-id="183c8-676">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="183c8-676">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="183c8-677">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="183c8-677">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="183c8-678">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="183c8-678">Az.ApiManagement</span></span>
* <span data-ttu-id="183c8-679">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="183c8-679">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="183c8-680">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="183c8-680">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="183c8-681">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="183c8-681">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="183c8-682">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="183c8-682">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="183c8-683">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="183c8-683">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="183c8-684">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="183c8-684">Az.Batch</span></span>
* <span data-ttu-id="183c8-685">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="183c8-685">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="183c8-686">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="183c8-686">Az.Cdn</span></span>
* <span data-ttu-id="183c8-687">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="183c8-687">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-688">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-688">Az.Compute</span></span>
* <span data-ttu-id="183c8-689">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-689">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="183c8-690">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="183c8-690">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="183c8-691">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="183c8-691">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="183c8-692">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="183c8-692">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="183c8-693">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="183c8-693">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="183c8-694">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="183c8-694">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="183c8-695">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="183c8-695">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="183c8-696">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="183c8-696">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="183c8-697">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="183c8-697">Az.DataFactory</span></span>
* <span data-ttu-id="183c8-698">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="183c8-698">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="183c8-699">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="183c8-699">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="183c8-700">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="183c8-700">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="183c8-701">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="183c8-701">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="183c8-702">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="183c8-702">Az.DataLakeStore</span></span>
* <span data-ttu-id="183c8-703">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="183c8-703">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="183c8-704">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="183c8-704">Az.EventHub</span></span>
* <span data-ttu-id="183c8-705">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="183c8-705">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="183c8-706">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="183c8-706">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="183c8-707">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="183c8-707">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="183c8-708">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="183c8-708">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="183c8-709">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="183c8-709">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="183c8-710">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="183c8-710">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="183c8-711">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="183c8-711">Az.Monitor</span></span>
* <span data-ttu-id="183c8-712">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="183c8-712">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-713">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-713">Az.Network</span></span>
* <span data-ttu-id="183c8-714">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="183c8-714">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="183c8-715">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="183c8-715">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="183c8-716">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="183c8-716">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="183c8-717">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="183c8-717">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="183c8-718">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="183c8-718">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="183c8-719">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="183c8-719">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="183c8-720">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="183c8-720">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="183c8-721">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="183c8-721">Az.OperationalInsights</span></span>
* <span data-ttu-id="183c8-722">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="183c8-722">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="183c8-723">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="183c8-723">Added example</span></span>
    - <span data-ttu-id="183c8-724">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="183c8-724">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="183c8-725">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="183c8-725">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="183c8-726">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="183c8-726">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-727">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-727">Az.RecoveryServices</span></span>
* <span data-ttu-id="183c8-728">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="183c8-728">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-729">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-729">Az.Resources</span></span>
* <span data-ttu-id="183c8-730">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="183c8-730">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="183c8-731">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="183c8-731">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="183c8-732">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="183c8-732">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="183c8-733">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="183c8-733">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="183c8-734">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="183c8-734">Az.ServiceBus</span></span>
* <span data-ttu-id="183c8-735">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="183c8-735">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="183c8-736">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="183c8-736">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="183c8-737">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="183c8-737">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="183c8-738">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="183c8-738">Az.ServiceFabric</span></span>
* <span data-ttu-id="183c8-739">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="183c8-739">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="183c8-740">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="183c8-740">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="183c8-741">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="183c8-741">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="183c8-742">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="183c8-742">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="183c8-743">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="183c8-743">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="183c8-744">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="183c8-744">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-745">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-745">Az.Sql</span></span>
* <span data-ttu-id="183c8-746">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="183c8-746">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="183c8-747">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-747">Az.Storage</span></span>
* <span data-ttu-id="183c8-748">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="183c8-748">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="183c8-749">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="183c8-749">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="183c8-750">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="183c8-750">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="183c8-751">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="183c8-751">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="183c8-752">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="183c8-752">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="183c8-753">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="183c8-753">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="183c8-754">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="183c8-754">Az.Websites</span></span>
* <span data-ttu-id="183c8-755">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="183c8-755">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="183c8-756">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-756">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="183c8-757">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-757">Az.Accounts</span></span>
* <span data-ttu-id="183c8-758">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="183c8-758">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="183c8-759">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="183c8-759">Az.ApplicationInsights</span></span>
* <span data-ttu-id="183c8-760">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="183c8-760">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="183c8-761">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="183c8-761">Az.Automation</span></span>
* <span data-ttu-id="183c8-762">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="183c8-762">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="183c8-763">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="183c8-763">Az.CognitiveServices</span></span>
* <span data-ttu-id="183c8-764">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="183c8-764">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-765">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-765">Az.Compute</span></span>
* <span data-ttu-id="183c8-766">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="183c8-766">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="183c8-767">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="183c8-767">Az.ContainerRegistry</span></span>
* <span data-ttu-id="183c8-768">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="183c8-768">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="183c8-769">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="183c8-769">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="183c8-770">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="183c8-770">Az.DataFactory</span></span>
* <span data-ttu-id="183c8-771">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="183c8-771">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="183c8-772">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="183c8-772">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="183c8-773">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="183c8-773">Az.EventHub</span></span>
* <span data-ttu-id="183c8-774">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="183c8-774">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="183c8-775">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="183c8-775">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="183c8-776">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="183c8-776">Az.KeyVault</span></span>
* <span data-ttu-id="183c8-777">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="183c8-777">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="183c8-778">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="183c8-778">Az.LogicApp</span></span>
* <span data-ttu-id="183c8-779">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="183c8-779">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="183c8-780">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="183c8-780">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="183c8-781">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="183c8-781">Az.ManagedServices</span></span>
* <span data-ttu-id="183c8-782">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="183c8-782">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-783">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-783">Az.Network</span></span>
* <span data-ttu-id="183c8-784">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="183c8-784">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="183c8-785">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="183c8-785">New cmdlets</span></span>
        - <span data-ttu-id="183c8-786">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="183c8-786">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="183c8-787">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="183c8-787">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="183c8-788">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-788">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="183c8-789">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-789">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="183c8-790">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-790">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="183c8-791">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-791">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="183c8-792">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="183c8-792">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="183c8-793">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="183c8-793">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="183c8-794">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="183c8-794">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="183c8-795">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-795">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="183c8-796">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="183c8-796">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="183c8-797">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="183c8-797">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="183c8-798">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="183c8-798">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="183c8-799">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="183c8-799">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="183c8-800">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="183c8-800">Updated cmdlets</span></span>
        - <span data-ttu-id="183c8-801">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-801">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="183c8-802">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-802">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="183c8-803">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-803">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="183c8-804">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-804">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="183c8-805">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="183c8-805">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="183c8-806">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="183c8-806">Updated cmdlet:</span></span>
        - <span data-ttu-id="183c8-807">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-807">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="183c8-808">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-808">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="183c8-809">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-809">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="183c8-810">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="183c8-810">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="183c8-811">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="183c8-811">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="183c8-812">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="183c8-812">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="183c8-813">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="183c8-813">Az.OperationalInsights</span></span>
* <span data-ttu-id="183c8-814">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="183c8-814">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="183c8-815">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="183c8-815">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-816">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-816">Az.RecoveryServices</span></span>
* <span data-ttu-id="183c8-817">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="183c8-817">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="183c8-818">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="183c8-818">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="183c8-819">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="183c8-819">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="183c8-820">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="183c8-820">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="183c8-821">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="183c8-821">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="183c8-822">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="183c8-822">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="183c8-823">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="183c8-823">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="183c8-824">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="183c8-824">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="183c8-825">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="183c8-825">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="183c8-826">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="183c8-826">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-827">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-827">Az.Resources</span></span>
- <span data-ttu-id="183c8-828">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="183c8-828">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="183c8-829">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="183c8-829">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="183c8-830">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="183c8-830">Az.ServiceBus</span></span>
* <span data-ttu-id="183c8-831">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="183c8-831">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="183c8-832">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="183c8-832">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-833">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-833">Az.Sql</span></span>
* <span data-ttu-id="183c8-834">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="183c8-834">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="183c8-835">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="183c8-835">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="183c8-836">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="183c8-836">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="183c8-837">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-837">Az.Storage</span></span>
* <span data-ttu-id="183c8-838">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="183c8-838">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="183c8-839">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="183c8-839">Az.StorageSync</span></span>
* <span data-ttu-id="183c8-840">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="183c8-840">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="183c8-841">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="183c8-841">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="183c8-842">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="183c8-842">Az.Websites</span></span>
* <span data-ttu-id="183c8-843">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="183c8-843">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="183c8-844">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="183c8-844">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="183c8-845">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="183c8-845">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="183c8-846">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-846">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="183c8-847">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-847">Az.Accounts</span></span>
* <span data-ttu-id="183c8-848">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="183c8-848">Add support for profile cmdlets</span></span>
* <span data-ttu-id="183c8-849">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="183c8-849">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="183c8-850">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="183c8-850">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="183c8-851">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="183c8-851">Az.Advisor</span></span>
* <span data-ttu-id="183c8-852">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="183c8-852">GA release of Az.Advisor</span></span>
* <span data-ttu-id="183c8-853">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="183c8-853">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="183c8-854">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="183c8-854">Az.ApiManagement</span></span>
* <span data-ttu-id="183c8-855">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="183c8-855">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="183c8-856">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="183c8-856">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="183c8-857">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="183c8-857">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="183c8-858">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="183c8-858">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="183c8-859">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="183c8-859">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="183c8-860">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="183c8-860">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="183c8-861">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="183c8-861">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="183c8-862">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="183c8-862">Az.Automation</span></span>
* <span data-ttu-id="183c8-863">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="183c8-863">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-864">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-864">Az.Compute</span></span>
* <span data-ttu-id="183c8-865">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-865">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="183c8-866">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="183c8-866">Az.DataFactory</span></span>
* <span data-ttu-id="183c8-867">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="183c8-867">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="183c8-868">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="183c8-868">Az.EventGrid</span></span>
* <span data-ttu-id="183c8-869">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="183c8-869">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="183c8-870">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="183c8-870">Az.IotHub</span></span>
* <span data-ttu-id="183c8-871">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="183c8-871">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-872">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-872">Az.Network</span></span>
* <span data-ttu-id="183c8-873">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="183c8-873">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="183c8-874">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="183c8-874">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="183c8-875">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="183c8-875">Az.PolicyInsights</span></span>
* <span data-ttu-id="183c8-876">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="183c8-876">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="183c8-877">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="183c8-877">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="183c8-878">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="183c8-878">Az.OperationalInsights</span></span>
* <span data-ttu-id="183c8-879">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="183c8-879">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-880">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-880">Az.RecoveryServices</span></span>
* <span data-ttu-id="183c8-881">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="183c8-881">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-882">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-882">Az.Resources</span></span>
    - <span data-ttu-id="183c8-883">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="183c8-883">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="183c8-884">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="183c8-884">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="183c8-885">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="183c8-885">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="183c8-886">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="183c8-886">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="183c8-887">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="183c8-887">Az.ServiceBus</span></span>
* <span data-ttu-id="183c8-888">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="183c8-888">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-889">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-889">Az.Sql</span></span>
* <span data-ttu-id="183c8-890">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="183c8-890">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="183c8-891">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="183c8-891">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="183c8-892">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="183c8-892">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="183c8-893">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="183c8-893">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="183c8-894">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="183c8-894">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="183c8-895">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="183c8-895">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="183c8-896">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="183c8-896">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="183c8-897">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="183c8-897">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="183c8-898">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="183c8-898">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="183c8-899">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-899">Az.Storage</span></span>
* <span data-ttu-id="183c8-900">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="183c8-900">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="183c8-901">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="183c8-901">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="183c8-902">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="183c8-902">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="183c8-903">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="183c8-903">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="183c8-904">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="183c8-904">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="183c8-905">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="183c8-905">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="183c8-906">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="183c8-906">Set-AzStorageAccount</span></span>
* <span data-ttu-id="183c8-907">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="183c8-907">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="183c8-908">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="183c8-908">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="183c8-909">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="183c8-909">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="183c8-910">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="183c8-910">Az.StorageSync</span></span>
* <span data-ttu-id="183c8-911">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="183c8-911">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="183c8-912">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-912">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="183c8-913">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-913">Az.Accounts</span></span>
* <span data-ttu-id="183c8-914">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="183c8-914">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="183c8-915">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="183c8-915">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="183c8-916">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="183c8-916">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="183c8-917">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="183c8-917">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="183c8-918">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="183c8-918">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-919">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-919">Az.Compute</span></span>
* <span data-ttu-id="183c8-920">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="183c8-920">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="183c8-921">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="183c8-921">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="183c8-922">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="183c8-922">Az.Dns</span></span>
* <span data-ttu-id="183c8-923">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="183c8-923">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="183c8-924">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="183c8-924">Az.EventGrid</span></span>
* <span data-ttu-id="183c8-925">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="183c8-925">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="183c8-926">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="183c8-926">New cmdlets:</span></span>
    - <span data-ttu-id="183c8-927">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="183c8-927">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="183c8-928">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="183c8-928">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="183c8-929">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="183c8-929">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="183c8-930">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-930">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="183c8-931">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="183c8-931">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="183c8-932">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="183c8-932">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="183c8-933">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="183c8-933">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="183c8-934">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="183c8-934">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="183c8-935">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="183c8-935">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="183c8-936">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="183c8-936">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="183c8-937">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="183c8-937">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="183c8-938">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="183c8-938">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="183c8-939">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="183c8-939">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="183c8-940">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="183c8-940">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="183c8-941">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="183c8-941">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="183c8-942">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="183c8-942">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="183c8-943">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="183c8-943">Updated cmdlets:</span></span>
    - <span data-ttu-id="183c8-944">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="183c8-944">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="183c8-945">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="183c8-945">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="183c8-946">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="183c8-946">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="183c8-947">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="183c8-947">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="183c8-948">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="183c8-948">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="183c8-949">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="183c8-949">Event subscription expiration date,</span></span>
            - <span data-ttu-id="183c8-950">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="183c8-950">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="183c8-951">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="183c8-951">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="183c8-952">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="183c8-952">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="183c8-953">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="183c8-953">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="183c8-954">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="183c8-954">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="183c8-955">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="183c8-955">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="183c8-956">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="183c8-956">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="183c8-957">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="183c8-957">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="183c8-958">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="183c8-958">Az.FrontDoor</span></span>
* <span data-ttu-id="183c8-959">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="183c8-959">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="183c8-960">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="183c8-960">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="183c8-961">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="183c8-961">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="183c8-962">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="183c8-962">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-963">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-963">Az.Network</span></span>
* <span data-ttu-id="183c8-964">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="183c8-964">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="183c8-965">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="183c8-965">New cmdlets</span></span>
        - <span data-ttu-id="183c8-966">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="183c8-966">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="183c8-967">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="183c8-967">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="183c8-968">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="183c8-968">New cmdlets</span></span> 
        - <span data-ttu-id="183c8-969">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="183c8-969">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="183c8-970">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="183c8-970">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="183c8-971">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="183c8-971">New cmdlets</span></span> 
        - <span data-ttu-id="183c8-972">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="183c8-972">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="183c8-973">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="183c8-973">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="183c8-974">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="183c8-974">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="183c8-975">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-975">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="183c8-976">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-976">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="183c8-977">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="183c8-977">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="183c8-978">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="183c8-978">New cmdlets</span></span>
        - <span data-ttu-id="183c8-979">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="183c8-979">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="183c8-980">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="183c8-980">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="183c8-981">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="183c8-981">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="183c8-982">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-982">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="183c8-983">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="183c8-983">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="183c8-984">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="183c8-984">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="183c8-985">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="183c8-985">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="183c8-986">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="183c8-986">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="183c8-987">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="183c8-987">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="183c8-988">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="183c8-988">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="183c8-989">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="183c8-989">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="183c8-990">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="183c8-990">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="183c8-991">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="183c8-991">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="183c8-992">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="183c8-992">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="183c8-993">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="183c8-993">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="183c8-994">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="183c8-994">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="183c8-995">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="183c8-995">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="183c8-996">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="183c8-996">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="183c8-997">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="183c8-997">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="183c8-998">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="183c8-998">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="183c8-999">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="183c8-999">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="183c8-1000">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="183c8-1000">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="183c8-1001">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="183c8-1001">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="183c8-1002">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="183c8-1002">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="183c8-1003">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="183c8-1003">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="183c8-1004">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="183c8-1004">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="183c8-1005">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="183c8-1005">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="183c8-1006">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="183c8-1006">Az.OperationalInsights</span></span>
* <span data-ttu-id="183c8-1007">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="183c8-1007">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-1008">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1008">Az.Resources</span></span>
* <span data-ttu-id="183c8-1009">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="183c8-1009">Support for additional Template Export options</span></span>
    - <span data-ttu-id="183c8-1010">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="183c8-1010">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="183c8-1011">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="183c8-1011">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="183c8-1012">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="183c8-1012">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="183c8-1013">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="183c8-1013">Az.ServiceFabric</span></span>
* <span data-ttu-id="183c8-1014">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="183c8-1014">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-1015">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-1015">Az.Sql</span></span>
* <span data-ttu-id="183c8-1016">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="183c8-1016">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="183c8-1017">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="183c8-1017">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="183c8-1018">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="183c8-1018">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="183c8-1019">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="183c8-1019">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="183c8-1020">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="183c8-1020">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="183c8-1021">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="183c8-1021">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="183c8-1022">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="183c8-1022">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="183c8-1023">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="183c8-1023">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="183c8-1024">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-1024">Az.Storage</span></span>
* <span data-ttu-id="183c8-1025">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="183c8-1025">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="183c8-1026">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="183c8-1026">New-AzStorageAccount</span></span>
* <span data-ttu-id="183c8-1027">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="183c8-1027">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="183c8-1028">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="183c8-1028">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="183c8-1029">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="183c8-1029">Az.Websites</span></span>
* <span data-ttu-id="183c8-1030">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="183c8-1030">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="183c8-1031">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="183c8-1031">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="183c8-1032">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-1032">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="183c8-1033">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="183c8-1033">Az.Cdn</span></span>
* <span data-ttu-id="183c8-1034">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="183c8-1034">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-1035">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1035">Az.Compute</span></span>
* <span data-ttu-id="183c8-1036">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="183c8-1036">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="183c8-1037">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="183c8-1037">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="183c8-1038">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="183c8-1038">Az.EventHub</span></span>
* <span data-ttu-id="183c8-1039">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="183c8-1039">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="183c8-1040">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="183c8-1040">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-1041">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1041">Az.Network</span></span>
* <span data-ttu-id="183c8-1042">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="183c8-1042">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="183c8-1043">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="183c8-1043">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="183c8-1044">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="183c8-1044">Az.PolicyInsights</span></span>
* <span data-ttu-id="183c8-1045">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="183c8-1045">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-1046">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1046">Az.RecoveryServices</span></span>
* <span data-ttu-id="183c8-1047">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="183c8-1047">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="183c8-1048">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="183c8-1048">Az.ServiceBus</span></span>
* <span data-ttu-id="183c8-1049">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="183c8-1049">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="183c8-1050">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="183c8-1050">Az.ServiceFabric</span></span>
* <span data-ttu-id="183c8-1051">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="183c8-1051">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="183c8-1052">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="183c8-1052">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-1053">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-1053">Az.Sql</span></span>
* <span data-ttu-id="183c8-1054">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="183c8-1054">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="183c8-1055">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="183c8-1055">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="183c8-1056">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="183c8-1056">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="183c8-1057">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="183c8-1057">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="183c8-1058">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="183c8-1058">Az.Websites</span></span>
* <span data-ttu-id="183c8-1059">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="183c8-1059">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="183c8-1060">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-1060">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="183c8-1061">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="183c8-1061">Az.ApiManagement</span></span>
* <span data-ttu-id="183c8-1062">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="183c8-1062">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="183c8-1063">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="183c8-1063">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="183c8-1064">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="183c8-1064">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="183c8-1065">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="183c8-1065">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="183c8-1066">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="183c8-1066">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="183c8-1067">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="183c8-1067">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="183c8-1068">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="183c8-1068">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="183c8-1069">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="183c8-1069">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="183c8-1070">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="183c8-1070">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="183c8-1071">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="183c8-1071">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="183c8-1072">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="183c8-1072">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="183c8-1073">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="183c8-1073">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="183c8-1074">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="183c8-1074">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="183c8-1075">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="183c8-1075">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="183c8-1076">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="183c8-1076">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="183c8-1077">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="183c8-1077">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="183c8-1078">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="183c8-1078">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="183c8-1079">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="183c8-1079">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="183c8-1080">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="183c8-1080">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="183c8-1081">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="183c8-1081">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="183c8-1082">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="183c8-1082">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="183c8-1083">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="183c8-1083">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="183c8-1084">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="183c8-1084">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="183c8-1085">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="183c8-1085">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="183c8-1086">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="183c8-1086">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="183c8-1087">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="183c8-1087">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="183c8-1088">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="183c8-1088">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="183c8-1089">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="183c8-1089">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="183c8-1090">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="183c8-1090">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="183c8-1091">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="183c8-1091">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="183c8-1092">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="183c8-1092">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="183c8-1093">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="183c8-1093">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="183c8-1094">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="183c8-1094">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="183c8-1095">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="183c8-1095">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="183c8-1096">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="183c8-1096">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="183c8-1097">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="183c8-1097">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="183c8-1098">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="183c8-1098">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="183c8-1099">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="183c8-1099">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="183c8-1100">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="183c8-1100">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="183c8-1101">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="183c8-1101">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="183c8-1102">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="183c8-1102">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="183c8-1103">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="183c8-1103">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="183c8-1104">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="183c8-1104">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="183c8-1105">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="183c8-1105">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="183c8-1106">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="183c8-1106">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="183c8-1107">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="183c8-1107">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="183c8-1108">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="183c8-1108">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="183c8-1109">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="183c8-1109">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="183c8-1110">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="183c8-1110">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="183c8-1111">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="183c8-1111">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="183c8-1112">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="183c8-1112">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="183c8-1113">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="183c8-1113">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="183c8-1114">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="183c8-1114">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="183c8-1115">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="183c8-1115">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="183c8-1116">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="183c8-1116">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="183c8-1117">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="183c8-1117">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="183c8-1118">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="183c8-1118">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="183c8-1119">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="183c8-1119">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="183c8-1120">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="183c8-1120">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="183c8-1121">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="183c8-1121">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="183c8-1122">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="183c8-1122">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="183c8-1123">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="183c8-1123">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="183c8-1124">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="183c8-1124">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="183c8-1125">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="183c8-1125">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="183c8-1126">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="183c8-1126">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="183c8-1127">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="183c8-1127">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="183c8-1128">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="183c8-1128">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="183c8-1129">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="183c8-1129">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="183c8-1130">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="183c8-1130">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="183c8-1131">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="183c8-1131">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="183c8-1132">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="183c8-1132">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="183c8-1133">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="183c8-1133">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="183c8-1134">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="183c8-1134">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="183c8-1135">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="183c8-1135">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="183c8-1136">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="183c8-1136">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="183c8-1137">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="183c8-1137">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="183c8-1138">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="183c8-1138">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="183c8-1139">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="183c8-1139">Az.Automation</span></span>
* <span data-ttu-id="183c8-1140">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="183c8-1140">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="183c8-1141">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="183c8-1141">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="183c8-1142">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="183c8-1142">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="183c8-1143">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="183c8-1143">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="183c8-1144">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="183c8-1144">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="183c8-1145">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="183c8-1145">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="183c8-1146">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="183c8-1146">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-1147">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1147">Az.Compute</span></span>
* <span data-ttu-id="183c8-1148">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="183c8-1148">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="183c8-1149">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="183c8-1149">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="183c8-1150">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="183c8-1150">Az.DataLakeStore</span></span>
* <span data-ttu-id="183c8-1151">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="183c8-1151">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="183c8-1152">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="183c8-1152">Az.Monitor</span></span>
* <span data-ttu-id="183c8-1153">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="183c8-1153">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-1154">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1154">Az.Network</span></span>
* <span data-ttu-id="183c8-1155">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="183c8-1155">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="183c8-1156">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="183c8-1156">Updated cmdlet:</span></span>
        - <span data-ttu-id="183c8-1157">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="183c8-1157">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="183c8-1158">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="183c8-1158">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-1159">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1159">Az.Resources</span></span>
* <span data-ttu-id="183c8-1160">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="183c8-1160">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-1161">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-1161">Az.Sql</span></span>
* <span data-ttu-id="183c8-1162">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="183c8-1162">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="183c8-1163">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-1163">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="183c8-1164">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-1164">Az.Accounts</span></span>
* <span data-ttu-id="183c8-1165">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="183c8-1165">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="183c8-1166">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1166">Az.CognitiveServices</span></span>
* <span data-ttu-id="183c8-1167">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="183c8-1167">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="183c8-1168">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="183c8-1168">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-1169">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1169">Az.Compute</span></span>
* <span data-ttu-id="183c8-1170">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="183c8-1170">Proximity placement group feature.</span></span>
    - <span data-ttu-id="183c8-1171">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="183c8-1171">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="183c8-1172">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-1172">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="183c8-1173">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="183c8-1173">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="183c8-1174">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="183c8-1174">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="183c8-1175">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="183c8-1175">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="183c8-1176">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="183c8-1176">Breaking changes</span></span>
    - <span data-ttu-id="183c8-1177">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="183c8-1177">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="183c8-1178">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="183c8-1178">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="183c8-1179">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="183c8-1179">Az.DeploymentManager</span></span>
* <span data-ttu-id="183c8-1180">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="183c8-1180">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="183c8-1181">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="183c8-1181">Az.Dns</span></span>
* <span data-ttu-id="183c8-1182">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="183c8-1182">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="183c8-1183">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="183c8-1183">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="183c8-1184">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="183c8-1184">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="183c8-1185">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="183c8-1185">Az.FrontDoor</span></span>
* <span data-ttu-id="183c8-1186">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="183c8-1186">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="183c8-1187">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="183c8-1187">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="183c8-1188">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="183c8-1188">Az.HDInsight</span></span>
* <span data-ttu-id="183c8-1189">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="183c8-1189">Removed two cmdlets:</span></span>
    - <span data-ttu-id="183c8-1190">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="183c8-1190">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="183c8-1191">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="183c8-1191">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="183c8-1192">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="183c8-1192">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="183c8-1193">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="183c8-1193">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="183c8-1194">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="183c8-1194">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="183c8-1195">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="183c8-1195">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="183c8-1196">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="183c8-1196">Az.Monitor</span></span>
* <span data-ttu-id="183c8-1197">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="183c8-1197">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="183c8-1198">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="183c8-1198">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="183c8-1199">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="183c8-1199">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="183c8-1200">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="183c8-1200">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="183c8-1201">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="183c8-1201">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="183c8-1202">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="183c8-1202">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="183c8-1203">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="183c8-1203">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="183c8-1204">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="183c8-1204">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="183c8-1205">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="183c8-1205">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="183c8-1206">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="183c8-1206">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="183c8-1207">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="183c8-1207">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="183c8-1208">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="183c8-1208">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="183c8-1209">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="183c8-1209">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="183c8-1210">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="183c8-1210">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-1211">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1211">Az.Network</span></span>
* <span data-ttu-id="183c8-1212">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="183c8-1212">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="183c8-1213">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="183c8-1213">New cmdlets</span></span>
        - <span data-ttu-id="183c8-1214">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="183c8-1214">New-AzNatGateway</span></span>
        - <span data-ttu-id="183c8-1215">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="183c8-1215">Get-AzNatGateway</span></span>
        - <span data-ttu-id="183c8-1216">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="183c8-1216">Set-AzNatGateway</span></span>
        - <span data-ttu-id="183c8-1217">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="183c8-1217">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="183c8-1218">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="183c8-1218">Updated cmdlets</span></span>
        - <span data-ttu-id="183c8-1219">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="183c8-1219">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="183c8-1220">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="183c8-1220">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="183c8-1221">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="183c8-1221">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="183c8-1222">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="183c8-1222">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="183c8-1223">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="183c8-1223">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="183c8-1224">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="183c8-1224">Az.PolicyInsights</span></span>
* <span data-ttu-id="183c8-1225">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="183c8-1225">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="183c8-1226">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="183c8-1226">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="183c8-1227">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="183c8-1227">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-1228">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1228">Az.RecoveryServices</span></span>
* <span data-ttu-id="183c8-1229">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="183c8-1229">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="183c8-1230">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="183c8-1230">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="183c8-1231">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="183c8-1231">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="183c8-1232">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-1232">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="183c8-1233">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="183c8-1233">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="183c8-1234">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="183c8-1234">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="183c8-1235">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="183c8-1235">Az.Relay</span></span>
* <span data-ttu-id="183c8-1236">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="183c8-1236">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="183c8-1237">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="183c8-1237">Az.ServiceBus</span></span>
* <span data-ttu-id="183c8-1238">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="183c8-1238">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="183c8-1239">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-1239">Az.Storage</span></span>
* <span data-ttu-id="183c8-1240">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="183c8-1240">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="183c8-1241">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="183c8-1241">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="183c8-1242">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="183c8-1242">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="183c8-1243">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="183c8-1243">New-AzStorageAccount</span></span>
* <span data-ttu-id="183c8-1244">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="183c8-1244">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="183c8-1245">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="183c8-1245">New-AzStorageAccount</span></span>
    - <span data-ttu-id="183c8-1246">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="183c8-1246">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="183c8-1247">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="183c8-1247">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="183c8-1248">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="183c8-1248">Az.Websites</span></span>
* <span data-ttu-id="183c8-1249">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="183c8-1249">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="183c8-1250">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="183c8-1250">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="183c8-1251">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-1251">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="183c8-1252">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="183c8-1252">Highlights since the last major release</span></span>
* <span data-ttu-id="183c8-1253">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="183c8-1253">General availability of `Az` module</span></span>
* <span data-ttu-id="183c8-1254">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="183c8-1254">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="183c8-1255">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="183c8-1255">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="183c8-1256">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1256">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="183c8-1257">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="183c8-1257">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="183c8-1258">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="183c8-1258">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="183c8-1259">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="183c8-1259">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="183c8-1260">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-1260">Az.Accounts</span></span>
* <span data-ttu-id="183c8-1261">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="183c8-1261">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="183c8-1262">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="183c8-1262">Az.Batch</span></span>
* <span data-ttu-id="183c8-1263">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1263">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="183c8-1264">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="183c8-1264">Az.Cdn</span></span>
* <span data-ttu-id="183c8-1265">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1265">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="183c8-1266">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1266">Az.CognitiveServices</span></span>
* <span data-ttu-id="183c8-1267">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1267">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-1268">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1268">Az.Compute</span></span>
* <span data-ttu-id="183c8-1269">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="183c8-1269">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="183c8-1270">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1270">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="183c8-1271">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="183c8-1271">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="183c8-1272">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="183c8-1272">Az.DataFactory</span></span>
* <span data-ttu-id="183c8-1273">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="183c8-1273">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="183c8-1274">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="183c8-1274">Az.DataLakeStore</span></span>
* <span data-ttu-id="183c8-1275">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1275">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="183c8-1276">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="183c8-1276">Az.EventGrid</span></span>
* <span data-ttu-id="183c8-1277">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="183c8-1277">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="183c8-1278">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="183c8-1278">Az.EventHub</span></span>
* <span data-ttu-id="183c8-1279">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="183c8-1279">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="183c8-1280">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="183c8-1280">Az.HDInsight</span></span>
* <span data-ttu-id="183c8-1281">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1281">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="183c8-1282">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="183c8-1282">Az.IotHub</span></span>
* <span data-ttu-id="183c8-1283">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1283">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="183c8-1284">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="183c8-1284">Az.KeyVault</span></span>
* <span data-ttu-id="183c8-1285">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1285">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="183c8-1286">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="183c8-1286">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="183c8-1287">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="183c8-1287">Az.MachineLearning</span></span>
* <span data-ttu-id="183c8-1288">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1288">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="183c8-1289">Az.Media</span><span class="sxs-lookup"><span data-stu-id="183c8-1289">Az.Media</span></span>
* <span data-ttu-id="183c8-1290">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1290">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="183c8-1291">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="183c8-1291">Az.Monitor</span></span>
  * <span data-ttu-id="183c8-1292">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="183c8-1292">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="183c8-1293">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="183c8-1293">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="183c8-1294">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="183c8-1294">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="183c8-1295">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="183c8-1295">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="183c8-1296">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="183c8-1296">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="183c8-1297">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="183c8-1297">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="183c8-1298">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="183c8-1298">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-1299">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1299">Az.Network</span></span>
* <span data-ttu-id="183c8-1300">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1300">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="183c8-1301">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="183c8-1301">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="183c8-1302">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="183c8-1302">Az.NotificationHubs</span></span>
* <span data-ttu-id="183c8-1303">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1303">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="183c8-1304">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="183c8-1304">Az.OperationalInsights</span></span>
* <span data-ttu-id="183c8-1305">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1305">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="183c8-1306">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="183c8-1306">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="183c8-1307">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1307">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-1308">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1308">Az.RecoveryServices</span></span>
* <span data-ttu-id="183c8-1309">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1309">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="183c8-1310">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="183c8-1310">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="183c8-1311">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="183c8-1311">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="183c8-1312">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="183c8-1312">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="183c8-1313">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="183c8-1313">Az.RedisCache</span></span>
* <span data-ttu-id="183c8-1314">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1314">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-1315">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1315">Az.Resources</span></span>
* <span data-ttu-id="183c8-1316">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="183c8-1316">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-1317">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-1317">Az.Sql</span></span>
* <span data-ttu-id="183c8-1318">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="183c8-1318">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="183c8-1319">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1319">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="183c8-1320">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="183c8-1320">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="183c8-1321">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="183c8-1321">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="183c8-1322">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="183c8-1322">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="183c8-1323">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="183c8-1323">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="183c8-1324">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="183c8-1324">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="183c8-1325">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="183c8-1325">Az.Websites</span></span>
* <span data-ttu-id="183c8-1326">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="183c8-1326">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="183c8-1327">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="183c8-1327">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="183c8-1328">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="183c8-1328">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="183c8-1329">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="183c8-1329">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="183c8-1330">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-1330">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="183c8-1331">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="183c8-1331">Highlights since the last major release</span></span>
* <span data-ttu-id="183c8-1332">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="183c8-1332">General availability of `Az` module</span></span>
* <span data-ttu-id="183c8-1333">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="183c8-1333">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="183c8-1334">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="183c8-1334">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="183c8-1335">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1335">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="183c8-1336">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="183c8-1336">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="183c8-1337">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="183c8-1337">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="183c8-1338">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="183c8-1338">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="183c8-1339">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-1339">Az.Accounts</span></span>
* <span data-ttu-id="183c8-1340">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="183c8-1340">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="183c8-1341">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1341">Az.AnalysisServices</span></span>
* <span data-ttu-id="183c8-1342">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="183c8-1342">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="183c8-1343">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="183c8-1343">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="183c8-1344">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="183c8-1344">Az.Automation</span></span>
* <span data-ttu-id="183c8-1345">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="183c8-1345">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="183c8-1346">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="183c8-1346">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="183c8-1347">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="183c8-1347">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-1348">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1348">Az.Compute</span></span>
* <span data-ttu-id="183c8-1349">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-1349">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="183c8-1350">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="183c8-1350">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="183c8-1351">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="183c8-1351">Az.ContainerInstance</span></span>
* <span data-ttu-id="183c8-1352">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="183c8-1352">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="183c8-1353">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="183c8-1353">Az.DataFactory</span></span>
* <span data-ttu-id="183c8-1354">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="183c8-1354">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="183c8-1355">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="183c8-1355">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-1356">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1356">Az.Resources</span></span>
* <span data-ttu-id="183c8-1357">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="183c8-1357">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="183c8-1358">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="183c8-1358">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="183c8-1359">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="183c8-1359">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="183c8-1360">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="183c8-1360">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="183c8-1361">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="183c8-1361">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="183c8-1362">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="183c8-1362">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-1363">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-1363">Az.Sql</span></span>
* <span data-ttu-id="183c8-1364">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="183c8-1364">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="183c8-1365">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-1365">Az.Storage</span></span>
* <span data-ttu-id="183c8-1366">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="183c8-1366">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="183c8-1367">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="183c8-1367">New-AzStorageContext</span></span>
* <span data-ttu-id="183c8-1368">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="183c8-1368">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="183c8-1369">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="183c8-1369">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="183c8-1370">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="183c8-1370">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="183c8-1371">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="183c8-1371">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="183c8-1372">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="183c8-1372">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="183c8-1373">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="183c8-1373">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="183c8-1374">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="183c8-1374">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="183c8-1375">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="183c8-1375">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="183c8-1376">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="183c8-1376">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="183c8-1377">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="183c8-1377">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="183c8-1378">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-1378">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="183c8-1379">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="183c8-1379">Highlights since the last major release</span></span>
* <span data-ttu-id="183c8-1380">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="183c8-1380">General availability of `Az` module</span></span>
* <span data-ttu-id="183c8-1381">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="183c8-1381">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="183c8-1382">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="183c8-1382">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="183c8-1383">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1383">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="183c8-1384">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="183c8-1384">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="183c8-1385">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="183c8-1385">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="183c8-1386">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="183c8-1386">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="183c8-1387">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="183c8-1387">Az.Automation</span></span>
* <span data-ttu-id="183c8-1388">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="183c8-1388">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="183c8-1389">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="183c8-1389">Dynamic grouping</span></span>
    * <span data-ttu-id="183c8-1390">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="183c8-1390">Pre-Post script</span></span>
    * <span data-ttu-id="183c8-1391">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="183c8-1391">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-1392">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1392">Az.Compute</span></span>
* <span data-ttu-id="183c8-1393">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="183c8-1393">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="183c8-1394">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="183c8-1394">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="183c8-1395">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="183c8-1395">Az.KeyVault</span></span>
* <span data-ttu-id="183c8-1396">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="183c8-1396">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-1397">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1397">Az.Network</span></span>
* <span data-ttu-id="183c8-1398">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="183c8-1398">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="183c8-1399">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="183c8-1399">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-1400">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1400">Az.RecoveryServices</span></span>
* <span data-ttu-id="183c8-1401">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="183c8-1401">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="183c8-1402">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="183c8-1402">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-1403">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1403">Az.Resources</span></span>
* <span data-ttu-id="183c8-1404">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="183c8-1404">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="183c8-1405">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="183c8-1405">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-1406">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-1406">Az.Sql</span></span>
* <span data-ttu-id="183c8-1407">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="183c8-1407">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="183c8-1408">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-1408">Az.Storage</span></span>
* <span data-ttu-id="183c8-1409">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="183c8-1409">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="183c8-1410">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="183c8-1410">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="183c8-1411">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="183c8-1411">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="183c8-1412">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="183c8-1412">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="183c8-1413">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="183c8-1413">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="183c8-1414">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="183c8-1414">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="183c8-1415">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="183c8-1415">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="183c8-1416">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="183c8-1416">Az.Websites</span></span>
* <span data-ttu-id="183c8-1417">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="183c8-1417">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="183c8-1418">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-1418">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="183c8-1419">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-1419">Az.Accounts</span></span>
* <span data-ttu-id="183c8-1420">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="183c8-1420">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="183c8-1421">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="183c8-1421">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="183c8-1422">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="183c8-1422">Az.Automation</span></span>
* <span data-ttu-id="183c8-1423">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="183c8-1423">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="183c8-1424">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="183c8-1424">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="183c8-1425">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="183c8-1425">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="183c8-1426">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="183c8-1426">Az.Cdn</span></span>
* <span data-ttu-id="183c8-1427">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="183c8-1427">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-1428">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1428">Az.Compute</span></span>
* <span data-ttu-id="183c8-1429">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="183c8-1429">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="183c8-1430">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="183c8-1430">Az.DataFactory</span></span>
* <span data-ttu-id="183c8-1431">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="183c8-1431">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="183c8-1432">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="183c8-1432">Az.LogicApp</span></span>
* <span data-ttu-id="183c8-1433">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="183c8-1433">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-1434">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1434">Az.Network</span></span>
* <span data-ttu-id="183c8-1435">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1435">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-1436">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1436">Az.RecoveryServices</span></span>
* <span data-ttu-id="183c8-1437">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="183c8-1437">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="183c8-1438">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="183c8-1438">SDK Update</span></span>
* <span data-ttu-id="183c8-1439">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="183c8-1439">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="183c8-1440">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="183c8-1440">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-1441">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1441">Az.Resources</span></span>
* <span data-ttu-id="183c8-1442">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="183c8-1442">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="183c8-1443">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="183c8-1443">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="183c8-1444">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="183c8-1444">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="183c8-1445">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="183c8-1445">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="183c8-1446">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="183c8-1446">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="183c8-1447">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="183c8-1447">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-1448">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-1448">Az.Sql</span></span>
* <span data-ttu-id="183c8-1449">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="183c8-1449">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="183c8-1450">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="183c8-1450">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="183c8-1451">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-1451">Az.Storage</span></span>
* <span data-ttu-id="183c8-1452">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="183c8-1452">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="183c8-1453">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-1453">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="183c8-1454">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1454">Az.AnalysisServices</span></span>
* <span data-ttu-id="183c8-1455">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="183c8-1455">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="183c8-1456">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="183c8-1456">Az.Automation</span></span>
* <span data-ttu-id="183c8-1457">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="183c8-1457">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="183c8-1458">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="183c8-1458">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="183c8-1459">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="183c8-1459">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="183c8-1460">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1460">Az.CognitiveServices</span></span>
* <span data-ttu-id="183c8-1461">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="183c8-1461">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-1462">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1462">Az.Compute</span></span>
* <span data-ttu-id="183c8-1463">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="183c8-1463">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="183c8-1464">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="183c8-1464">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="183c8-1465">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="183c8-1465">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="183c8-1466">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="183c8-1466">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="183c8-1467">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="183c8-1467">Az.DataLakeStore</span></span>
* <span data-ttu-id="183c8-1468">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="183c8-1468">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="183c8-1469">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="183c8-1469">Az.EventHub</span></span>
* <span data-ttu-id="183c8-1470">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="183c8-1470">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="183c8-1471">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="183c8-1471">Az.KeyVault</span></span>
* <span data-ttu-id="183c8-1472">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="183c8-1472">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="183c8-1473">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="183c8-1473">Az.LogicApp</span></span>
* <span data-ttu-id="183c8-1474">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="183c8-1474">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="183c8-1475">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="183c8-1475">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="183c8-1476">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="183c8-1476">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="183c8-1477">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="183c8-1477">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="183c8-1478">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="183c8-1478">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="183c8-1479">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="183c8-1479">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="183c8-1480">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="183c8-1480">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="183c8-1481">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="183c8-1481">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="183c8-1482">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="183c8-1482">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="183c8-1483">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="183c8-1483">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="183c8-1484">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="183c8-1484">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="183c8-1485">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="183c8-1485">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="183c8-1486">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="183c8-1486">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="183c8-1487">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="183c8-1487">Az.Monitor</span></span>
* <span data-ttu-id="183c8-1488">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="183c8-1488">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-1489">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1489">Az.Network</span></span>
* <span data-ttu-id="183c8-1490">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="183c8-1490">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="183c8-1491">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="183c8-1491">Az.OperationalInsights</span></span>
* <span data-ttu-id="183c8-1492">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="183c8-1492">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="183c8-1493">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="183c8-1493">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="183c8-1494">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="183c8-1494">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="183c8-1495">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1495">Az.Resources</span></span>
* <span data-ttu-id="183c8-1496">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="183c8-1496">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="183c8-1497">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="183c8-1497">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="183c8-1498">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="183c8-1498">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="183c8-1499">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="183c8-1499">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-1500">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-1500">Az.Sql</span></span>
* <span data-ttu-id="183c8-1501">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="183c8-1501">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="183c8-1502">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="183c8-1502">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="183c8-1503">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="183c8-1503">Az.Websites</span></span>
* <span data-ttu-id="183c8-1504">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="183c8-1504">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="183c8-1505">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-1505">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="183c8-1506">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-1506">Az.Accounts</span></span>
* <span data-ttu-id="183c8-1507">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="183c8-1507">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="183c8-1508">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1508">Az.AnalysisServices</span></span>
<span data-ttu-id="183c8-1509">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="183c8-1509">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-1510">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1510">Az.Compute</span></span>
* <span data-ttu-id="183c8-1511">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="183c8-1511">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="183c8-1512">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="183c8-1512">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="183c8-1513">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="183c8-1513">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-1514">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1514">Az.RecoveryServices</span></span>
<span data-ttu-id="183c8-1515">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="183c8-1515">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-1516">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1516">Az.Resources</span></span>
* <span data-ttu-id="183c8-1517">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="183c8-1517">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="183c8-1518">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="183c8-1518">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="183c8-1519">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="183c8-1519">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="183c8-1520">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="183c8-1520">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-1521">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-1521">Az.Sql</span></span>
* <span data-ttu-id="183c8-1522">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="183c8-1522">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="183c8-1523">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="183c8-1523">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="183c8-1524">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="183c8-1524">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="183c8-1525">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-1525">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="183c8-1526">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-1526">Az.Accounts</span></span>
* <span data-ttu-id="183c8-1527">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="183c8-1527">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="183c8-1528">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1528">Az.AnalysisServices</span></span>
* <span data-ttu-id="183c8-1529">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="183c8-1529">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-1530">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1530">Az.RecoveryServices</span></span>
* <span data-ttu-id="183c8-1531">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="183c8-1531">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="183c8-1532">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-1532">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="183c8-1533">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-1533">Az.Accounts</span></span>
* <span data-ttu-id="183c8-1534">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="183c8-1534">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="183c8-1535">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="183c8-1535">Update incorrect online help URLs</span></span>
* <span data-ttu-id="183c8-1536">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="183c8-1536">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="183c8-1537">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="183c8-1537">Az.Aks</span></span>
* <span data-ttu-id="183c8-1538">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="183c8-1538">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="183c8-1539">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="183c8-1539">Az.Automation</span></span>
* <span data-ttu-id="183c8-1540">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="183c8-1540">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="183c8-1541">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="183c8-1541">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="183c8-1542">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="183c8-1542">Az.Cdn</span></span>
* <span data-ttu-id="183c8-1543">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="183c8-1543">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-1544">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1544">Az.Compute</span></span>
* <span data-ttu-id="183c8-1545">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="183c8-1545">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="183c8-1546">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="183c8-1546">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="183c8-1547">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="183c8-1547">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="183c8-1548">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="183c8-1548">Az.ContainerRegistry</span></span>
* <span data-ttu-id="183c8-1549">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="183c8-1549">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="183c8-1550">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="183c8-1550">Az.DataFactory</span></span>
* <span data-ttu-id="183c8-1551">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="183c8-1551">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="183c8-1552">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="183c8-1552">Az.DataLakeStore</span></span>
* <span data-ttu-id="183c8-1553">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="183c8-1553">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="183c8-1554">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="183c8-1554">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="183c8-1555">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="183c8-1555">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="183c8-1556">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="183c8-1556">Az.IotHub</span></span>
* <span data-ttu-id="183c8-1557">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="183c8-1557">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="183c8-1558">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="183c8-1558">Az.KeyVault</span></span>
* <span data-ttu-id="183c8-1559">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="183c8-1559">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-1560">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1560">Az.Network</span></span>
* <span data-ttu-id="183c8-1561">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="183c8-1561">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-1562">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1562">Az.Resources</span></span>
* <span data-ttu-id="183c8-1563">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="183c8-1563">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="183c8-1564">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="183c8-1564">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="183c8-1565">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="183c8-1565">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="183c8-1566">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="183c8-1566">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="183c8-1567">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="183c8-1567">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="183c8-1568">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="183c8-1568">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="183c8-1569">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="183c8-1569">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="183c8-1570">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="183c8-1570">Az.ServiceFabric</span></span>
* <span data-ttu-id="183c8-1571">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="183c8-1571">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="183c8-1572">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="183c8-1572">Fix some error messages.</span></span>
* <span data-ttu-id="183c8-1573">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="183c8-1573">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="183c8-1574">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="183c8-1574">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="183c8-1575">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="183c8-1575">Az.SignalR</span></span>
* <span data-ttu-id="183c8-1576">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="183c8-1576">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-1577">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-1577">Az.Sql</span></span>
* <span data-ttu-id="183c8-1578">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="183c8-1578">Update incorrect online help URLs</span></span>
* <span data-ttu-id="183c8-1579">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="183c8-1579">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="183c8-1580">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="183c8-1580">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="183c8-1581">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="183c8-1581">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="183c8-1582">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-1582">Az.Storage</span></span>
* <span data-ttu-id="183c8-1583">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="183c8-1583">Update incorrect online help URLs</span></span>
* <span data-ttu-id="183c8-1584">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="183c8-1584">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="183c8-1585">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="183c8-1585">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="183c8-1586">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="183c8-1586">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="183c8-1587">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="183c8-1587">Az.TrafficManager</span></span>
* <span data-ttu-id="183c8-1588">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="183c8-1588">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="183c8-1589">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="183c8-1589">Az.Websites</span></span>
* <span data-ttu-id="183c8-1590">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="183c8-1590">Update incorrect online help URLs</span></span>
* <span data-ttu-id="183c8-1591">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="183c8-1591">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="183c8-1592">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="183c8-1592">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="183c8-1593">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="183c8-1593">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="183c8-1594">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-1594">Az.Accounts</span></span>
* <span data-ttu-id="183c8-1595">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="183c8-1595">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-1596">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1596">Az.Compute</span></span>
* <span data-ttu-id="183c8-1597">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="183c8-1597">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="183c8-1598">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="183c8-1598">Updated the description of ID in help files</span></span>
* <span data-ttu-id="183c8-1599">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-1599">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="183c8-1600">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="183c8-1600">Az.DataLakeStore</span></span>
* <span data-ttu-id="183c8-1601">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="183c8-1601">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="183c8-1602">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="183c8-1602">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="183c8-1603">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="183c8-1603">Az.EventGrid</span></span>
* <span data-ttu-id="183c8-1604">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="183c8-1604">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="183c8-1605">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="183c8-1605">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="183c8-1606">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="183c8-1606">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="183c8-1607">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="183c8-1607">Event Time-To-Live,</span></span>
        - <span data-ttu-id="183c8-1608">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="183c8-1608">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="183c8-1609">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="183c8-1609">Dead letter endpoint.</span></span>
    - <span data-ttu-id="183c8-1610">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="183c8-1610">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="183c8-1611">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="183c8-1611">Event Time-To-Live,</span></span>
        - <span data-ttu-id="183c8-1612">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="183c8-1612">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="183c8-1613">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="183c8-1613">Dead letter endpoint.</span></span>
* <span data-ttu-id="183c8-1614">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="183c8-1614">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="183c8-1615">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="183c8-1615">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="183c8-1616">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="183c8-1616">Az.IotHub</span></span>
* <span data-ttu-id="183c8-1617">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="183c8-1617">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="183c8-1618">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="183c8-1618">Az.LogicApp</span></span>
* <span data-ttu-id="183c8-1619">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="183c8-1619">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-1620">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1620">Az.Resources</span></span>
* <span data-ttu-id="183c8-1621">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="183c8-1621">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="183c8-1622">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="183c8-1622">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="183c8-1623">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="183c8-1623">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="183c8-1624">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="183c8-1624">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="183c8-1625">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="183c8-1625">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="183c8-1626">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="183c8-1626">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="183c8-1627">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="183c8-1627">Az.SignalR</span></span>
* <span data-ttu-id="183c8-1628">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-1628">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-1629">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-1629">Az.Sql</span></span>
* <span data-ttu-id="183c8-1630">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="183c8-1630">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="183c8-1631">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-1631">Az.Storage</span></span>
* <span data-ttu-id="183c8-1632">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="183c8-1632">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="183c8-1633">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="183c8-1633">New-AzStorageContext</span></span>
* <span data-ttu-id="183c8-1634">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="183c8-1634">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="183c8-1635">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="183c8-1635">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="183c8-1636">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="183c8-1636">Az.Websites</span></span>
* <span data-ttu-id="183c8-1637">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="183c8-1637">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="183c8-1638">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-1638">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="183c8-1639">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="183c8-1639">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="183c8-1640">Geral</span><span class="sxs-lookup"><span data-stu-id="183c8-1640">General</span></span>

- <span data-ttu-id="183c8-1641">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="183c8-1641">General Availability of Az Module</span></span>
- <span data-ttu-id="183c8-1642">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="183c8-1642">Online help for each module</span></span>
- <span data-ttu-id="183c8-1643">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="183c8-1643">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="183c8-1644">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="183c8-1644">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="183c8-1645">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-1645">Az.Accounts</span></span>
- <span data-ttu-id="183c8-1646">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="183c8-1646">Changed from Az.Profile</span></span>
- <span data-ttu-id="183c8-1647">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="183c8-1647">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="183c8-1648">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="183c8-1648">Az.ApiManagement</span></span>
- <span data-ttu-id="183c8-1649">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="183c8-1649">Fixes for #7002</span></span>
- <span data-ttu-id="183c8-1650">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="183c8-1650">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="183c8-1651">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="183c8-1651">Az.Batch</span></span>
- <span data-ttu-id="183c8-1652">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="183c8-1652">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="183c8-1653">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="183c8-1653">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="183c8-1654">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="183c8-1654">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="183c8-1655">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="183c8-1655">Az.Billing</span></span>
- <span data-ttu-id="183c8-1656">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="183c8-1656">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="183c8-1657">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1657">Az.CognitivServices</span></span>
- <span data-ttu-id="183c8-1658">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="183c8-1658">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="183c8-1659">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="183c8-1659">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="183c8-1660">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="183c8-1660">Az.ContainerInstance</span></span>
- <span data-ttu-id="183c8-1661">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="183c8-1661">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="183c8-1662">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="183c8-1662">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="183c8-1663">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="183c8-1663">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="183c8-1664">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="183c8-1664">Az.DataLakeStore</span></span>
- <span data-ttu-id="183c8-1665">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="183c8-1665">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="183c8-1666">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="183c8-1666">Az.Monitor</span></span>
- <span data-ttu-id="183c8-1667">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="183c8-1667">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="183c8-1668">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="183c8-1668">Az.KeyVault</span></span>
- <span data-ttu-id="183c8-1669">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="183c8-1669">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="183c8-1670">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="183c8-1670">Az.MachineLearning</span></span>
- <span data-ttu-id="183c8-1671">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="183c8-1671">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="183c8-1672">Az.Media</span><span class="sxs-lookup"><span data-stu-id="183c8-1672">Az.Media</span></span>
- <span data-ttu-id="183c8-1673">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="183c8-1673">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="183c8-1674">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1674">Az.Network</span></span>
<span data-ttu-id="183c8-1675">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="183c8-1675">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="183c8-1676">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="183c8-1676">New cmdlets added:</span></span>
        - <span data-ttu-id="183c8-1677">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="183c8-1677">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="183c8-1678">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="183c8-1678">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="183c8-1679">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="183c8-1679">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="183c8-1680">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="183c8-1680">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="183c8-1681">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="183c8-1681">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="183c8-1682">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="183c8-1682">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="183c8-1683">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="183c8-1683">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="183c8-1684">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="183c8-1684">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="183c8-1685">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="183c8-1685">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="183c8-1686">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="183c8-1686">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="183c8-1687">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="183c8-1687">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="183c8-1688">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="183c8-1688">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="183c8-1689">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-1689">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="183c8-1690">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-1690">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="183c8-1691">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="183c8-1691">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="183c8-1692">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="183c8-1692">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="183c8-1693">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="183c8-1693">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="183c8-1694">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="183c8-1694">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="183c8-1695">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="183c8-1695">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="183c8-1696">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="183c8-1696">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="183c8-1697">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="183c8-1697">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="183c8-1698">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="183c8-1698">Az.OperationalInsights</span></span>
- <span data-ttu-id="183c8-1699">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="183c8-1699">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="183c8-1700">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="183c8-1700">Az.Profile</span></span>
- <span data-ttu-id="183c8-1701">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="183c8-1701">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-1702">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1702">Az.RecoveryServices</span></span>
- <span data-ttu-id="183c8-1703">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="183c8-1703">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="183c8-1704">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1704">Az.Resources</span></span>
- <span data-ttu-id="183c8-1705">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="183c8-1705">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="183c8-1706">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="183c8-1706">Az.ServiceFabric</span></span>
- <span data-ttu-id="183c8-1707">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="183c8-1707">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="183c8-1708">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="183c8-1708">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="183c8-1709">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="183c8-1709">Az.SIgnalR</span></span>
- <span data-ttu-id="183c8-1710">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="183c8-1710">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="183c8-1711">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-1711">Az.Sql</span></span>
- <span data-ttu-id="183c8-1712">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="183c8-1712">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="183c8-1713">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="183c8-1713">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="183c8-1714">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="183c8-1714">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="183c8-1715">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-1715">Az.Storage</span></span>
- <span data-ttu-id="183c8-1716">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="183c8-1716">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="183c8-1717">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="183c8-1717">Az.Websites</span></span>
- <span data-ttu-id="183c8-1718">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="183c8-1718">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="183c8-1719">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="183c8-1719">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="183c8-1720">Geral</span><span class="sxs-lookup"><span data-stu-id="183c8-1720">General</span></span>

* <span data-ttu-id="183c8-1721">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="183c8-1721">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="183c8-1722">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1722">Az.Compute</span></span>

* <span data-ttu-id="183c8-1723">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="183c8-1723">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="183c8-1724">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="183c8-1724">Az.DataLakeStore</span></span>

* <span data-ttu-id="183c8-1725">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="183c8-1725">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="183c8-1726">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="183c8-1726">Az.FrontDoor</span></span>

* <span data-ttu-id="183c8-1727">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="183c8-1727">Fixed some broken links</span></span>
    - <span data-ttu-id="183c8-1728">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="183c8-1728">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="183c8-1729">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="183c8-1729">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="183c8-1730">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1730">Az.RecoveryServices</span></span>

* <span data-ttu-id="183c8-1731">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-1731">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="183c8-1732">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="183c8-1732">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="183c8-1733">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1733">Az.Resources</span></span>

* <span data-ttu-id="183c8-1734">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="183c8-1734">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="183c8-1735">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="183c8-1735">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="183c8-1736">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-1736">Az.Sql</span></span>

* <span data-ttu-id="183c8-1737">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="183c8-1737">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="183c8-1738">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="183c8-1738">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="183c8-1739">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="183c8-1739">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="183c8-1740">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-1740">Az.Storage</span></span>

* <span data-ttu-id="183c8-1741">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="183c8-1741">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="183c8-1742">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="183c8-1742">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="183c8-1743">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="183c8-1743">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="183c8-1744">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="183c8-1744">Support Static Website configuration</span></span>
    - <span data-ttu-id="183c8-1745">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="183c8-1745">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="183c8-1746">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="183c8-1746">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="183c8-1747">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="183c8-1747">Az.Websites</span></span>

* <span data-ttu-id="183c8-1748">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="183c8-1748">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="183c8-1749">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="183c8-1749">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="183c8-1750">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-1750">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="183c8-1751">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="183c8-1751">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="183c8-1752">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="183c8-1752">Az.ApiManagement</span></span>
* <span data-ttu-id="183c8-1753">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="183c8-1753">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="183c8-1754">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="183c8-1754">Az.Automation</span></span>
* <span data-ttu-id="183c8-1755">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="183c8-1755">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="183c8-1756">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="183c8-1756">Added Update Management cmdlets</span></span>
* <span data-ttu-id="183c8-1757">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="183c8-1757">Added Source Control cmdlets</span></span>
* <span data-ttu-id="183c8-1758">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="183c8-1758">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="183c8-1759">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="183c8-1759">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="183c8-1760">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1760">Az.Compute</span></span>
* <span data-ttu-id="183c8-1761">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="183c8-1761">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="183c8-1762">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="183c8-1762">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="183c8-1763">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="183c8-1763">Az.ContainerInstance</span></span>
* <span data-ttu-id="183c8-1764">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="183c8-1764">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="183c8-1765">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="183c8-1765">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="183c8-1766">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="183c8-1766">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="183c8-1767">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1767">Az.Network</span></span>
* <span data-ttu-id="183c8-1768">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="183c8-1768">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="183c8-1769">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="183c8-1769">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="183c8-1770">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="183c8-1770">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="183c8-1771">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="183c8-1771">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="183c8-1772">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="183c8-1772">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="183c8-1773">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="183c8-1773">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="183c8-1774">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="183c8-1774">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="183c8-1775">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="183c8-1775">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="183c8-1776">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="183c8-1776">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="183c8-1777">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="183c8-1777">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="183c8-1778">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="183c8-1778">Az.Relay</span></span>
* <span data-ttu-id="183c8-1779">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="183c8-1779">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="183c8-1780">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1780">Az.Resources</span></span>
* <span data-ttu-id="183c8-1781">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="183c8-1781">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="183c8-1782">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="183c8-1782">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="183c8-1783">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="183c8-1783">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="183c8-1784">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="183c8-1784">Az.ServiceFabric</span></span>
* <span data-ttu-id="183c8-1785">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="183c8-1785">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="183c8-1786">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-1786">Az.Sql</span></span>
* <span data-ttu-id="183c8-1787">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="183c8-1787">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="183c8-1788">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="183c8-1788">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="183c8-1789">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="183c8-1789">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="183c8-1790">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="183c8-1790">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="183c8-1791">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="183c8-1791">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="183c8-1792">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="183c8-1792">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="183c8-1793">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="183c8-1793">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="183c8-1794">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="183c8-1794">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="183c8-1795">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="183c8-1795">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="183c8-1796">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="183c8-1796">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="183c8-1797">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="183c8-1797">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="183c8-1798">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="183c8-1798">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="183c8-1799">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="183c8-1799">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="183c8-1800">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="183c8-1800">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="183c8-1801">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="183c8-1801">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="183c8-1802">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="183c8-1802">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="183c8-1803">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="183c8-1803">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="183c8-1804">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="183c8-1804">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="183c8-1805">Geral</span><span class="sxs-lookup"><span data-stu-id="183c8-1805">General</span></span>
* <span data-ttu-id="183c8-1806">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="183c8-1806">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="183c8-1807">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="183c8-1807">Az.Profile</span></span>
* <span data-ttu-id="183c8-1808">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="183c8-1808">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="183c8-1809">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="183c8-1809">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="183c8-1810">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="183c8-1810">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="183c8-1811">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="183c8-1811">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="183c8-1812">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="183c8-1812">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="183c8-1813">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="183c8-1813">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="183c8-1814">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="183c8-1814">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="183c8-1815">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1815">Az.CognitiveServices</span></span>
* <span data-ttu-id="183c8-1816">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="183c8-1816">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-1817">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1817">Az.Compute</span></span>
* <span data-ttu-id="183c8-1818">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="183c8-1818">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="183c8-1819">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="183c8-1819">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="183c8-1820">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="183c8-1820">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="183c8-1821">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="183c8-1821">Az.DataLakeStore</span></span>
* <span data-ttu-id="183c8-1822">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="183c8-1822">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="183c8-1823">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="183c8-1823">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="183c8-1824">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="183c8-1824">Az.Insights</span></span>
* <span data-ttu-id="183c8-1825">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="183c8-1825">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="183c8-1826">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="183c8-1826">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="183c8-1827">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="183c8-1827">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="183c8-1828">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="183c8-1828">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-1829">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1829">Az.Network</span></span>
* <span data-ttu-id="183c8-1830">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="183c8-1830">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="183c8-1831">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="183c8-1831">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="183c8-1832">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="183c8-1832">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="183c8-1833">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="183c8-1833">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="183c8-1834">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="183c8-1834">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="183c8-1835">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="183c8-1835">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="183c8-1836">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="183c8-1836">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="183c8-1837">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="183c8-1837">Az.PolicyInsights</span></span>
* <span data-ttu-id="183c8-1838">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="183c8-1838">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-1839">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1839">Az.Resources</span></span>
* <span data-ttu-id="183c8-1840">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="183c8-1840">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="183c8-1841">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="183c8-1841">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="183c8-1842">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="183c8-1842">Az.ServiceBus</span></span>
* <span data-ttu-id="183c8-1843">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="183c8-1843">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="183c8-1844">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="183c8-1844">Az.ServiceFabric</span></span>
* <span data-ttu-id="183c8-1845">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="183c8-1845">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="183c8-1846">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="183c8-1846">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="183c8-1847">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="183c8-1847">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="183c8-1848">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="183c8-1848">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="183c8-1849">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="183c8-1849">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="183c8-1850">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="183c8-1850">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="183c8-1851">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="183c8-1851">Az.Profile</span></span>
* <span data-ttu-id="183c8-1852">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="183c8-1852">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="183c8-1853">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="183c8-1853">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-1854">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1854">Az.Compute</span></span>
* <span data-ttu-id="183c8-1855">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="183c8-1855">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="183c8-1856">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="183c8-1856">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="183c8-1857">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="183c8-1857">Az.DataLakeStore</span></span>
* <span data-ttu-id="183c8-1858">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="183c8-1858">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="183c8-1859">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-1859">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="183c8-1860">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="183c8-1860">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="183c8-1861">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="183c8-1861">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="183c8-1862">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="183c8-1862">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-1863">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1863">Az.Network</span></span>
* <span data-ttu-id="183c8-1864">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="183c8-1864">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="183c8-1865">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="183c8-1865">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-1866">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1866">Az.Resources</span></span>
* <span data-ttu-id="183c8-1867">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="183c8-1867">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="183c8-1868">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="183c8-1868">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="183c8-1869">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="183c8-1869">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="183c8-1870">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="183c8-1870">Azure.Storage</span></span>
* <span data-ttu-id="183c8-1871">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="183c8-1871">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="183c8-1872">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="183c8-1872">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="183c8-1873">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="183c8-1873">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="183c8-1874">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="183c8-1874">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="183c8-1875">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="183c8-1875">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="183c8-1876">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="183c8-1876">Az.CognitiveServices</span></span>
* <span data-ttu-id="183c8-1877">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="183c8-1877">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="183c8-1878">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="183c8-1878">Az.Compute</span></span>
* <span data-ttu-id="183c8-1879">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="183c8-1879">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="183c8-1880">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="183c8-1880">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="183c8-1881">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="183c8-1881">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="183c8-1882">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="183c8-1882">Az.DataFactoryV2</span></span>
* <span data-ttu-id="183c8-1883">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="183c8-1883">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="183c8-1884">Az.Network</span><span class="sxs-lookup"><span data-stu-id="183c8-1884">Az.Network</span></span>
* <span data-ttu-id="183c8-1885">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="183c8-1885">Added NetworkProfile functionality.</span></span> <span data-ttu-id="183c8-1886">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="183c8-1886">new cmdlets added</span></span>
    - <span data-ttu-id="183c8-1887">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="183c8-1887">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="183c8-1888">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="183c8-1888">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="183c8-1889">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="183c8-1889">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="183c8-1890">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="183c8-1890">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="183c8-1891">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-1891">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="183c8-1892">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-1892">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="183c8-1893">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="183c8-1893">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="183c8-1894">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="183c8-1894">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="183c8-1895">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="183c8-1895">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="183c8-1896">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="183c8-1896">Az.RedisCache</span></span>
* <span data-ttu-id="183c8-1897">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="183c8-1897">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="183c8-1898">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="183c8-1898">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="183c8-1899">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="183c8-1899">Az.Resources</span></span>
* <span data-ttu-id="183c8-1900">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="183c8-1900">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="183c8-1901">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="183c8-1901">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="183c8-1902">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="183c8-1902">Az.Sql</span></span>
* <span data-ttu-id="183c8-1903">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="183c8-1903">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="183c8-1904">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="183c8-1904">Az.Websites</span></span>
* <span data-ttu-id="183c8-1905">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="183c8-1905">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="183c8-1906">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="183c8-1906">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="183c8-1907">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="183c8-1907">0.2.0 - September 2018</span></span>
 <span data-ttu-id="183c8-1908">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="183c8-1908">Initial Release</span></span>
