---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: 88e9c622ef3608b17e6cd8d4ce8c193812a97520
ms.sourcegitcommit: 23e5b2b0751777ef0a5ca74e40c7772653e339a3
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/14/2020
ms.locfileid: "86382354"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="c90e7-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c90e7-103">Azure PowerShell release notes</span></span>

## <a name="440---july-2020"></a><span data-ttu-id="c90e7-104">4.4.0 - Julho de 2020</span><span class="sxs-lookup"><span data-stu-id="c90e7-104">4.4.0 - July 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c90e7-105">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-105">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-106">Adição do novo cmdlet "Invoke-AzRestMethod"</span><span class="sxs-lookup"><span data-stu-id="c90e7-106">Added new cmdlet 'Invoke-AzRestMethod'</span></span>
* <span data-ttu-id="c90e7-107">Correção de um problema que pode causar erros de autenticação em cenários de vários processos, tais como executar vários cmdlets do Azure PowerShell utilizando "Start-Job" [#9448]</span><span class="sxs-lookup"><span data-stu-id="c90e7-107">Fixed an issue that may cause authentication errors in multi-process scenarios such as running multiple Azure PowerShell cmdlets using 'Start-Job' [#9448]</span></span>

#### <a name="azaks"></a><span data-ttu-id="c90e7-108">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="c90e7-108">Az.Aks</span></span>
* <span data-ttu-id="c90e7-109">Correção do erro "Get-AzAks" uma vez que não recebe todos os clusters [#12296]</span><span class="sxs-lookup"><span data-stu-id="c90e7-109">Fixed bug 'Get-AzAks' doesn't get all clusters [#12296]</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c90e7-110">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-110">Az.AnalysisServices</span></span>
* <span data-ttu-id="c90e7-111">Remoção da referência do projeto para Autenticação</span><span class="sxs-lookup"><span data-stu-id="c90e7-111">Removed project reference to Authentication</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c90e7-112">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-112">Az.Automation</span></span>
* <span data-ttu-id="c90e7-113">Correção do problema em que a cadeia com chars de fuga não pode ser convertida num objeto json.</span><span class="sxs-lookup"><span data-stu-id="c90e7-113">Fixed the issue that string with escape chars cannot be converted into json object.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-114">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-114">Az.Compute</span></span>
* <span data-ttu-id="c90e7-115">Adição do aviso ao utilizar "New-AzVmss" sem a versão de imagem "mais recente"</span><span class="sxs-lookup"><span data-stu-id="c90e7-115">Added warning when using 'New-AzVmss' without 'latest' image version</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-116">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-116">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-117">Adição de parâmetros globais ao Data Factory.</span><span class="sxs-lookup"><span data-stu-id="c90e7-117">Added global parameters to Data Factory.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c90e7-118">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c90e7-118">Az.EventGrid</span></span>
* <span data-ttu-id="c90e7-119">Atualização para utilizar a versão de API 2020-06-01.</span><span class="sxs-lookup"><span data-stu-id="c90e7-119">Updated to use the 2020-06-01 API version.</span></span>
* <span data-ttu-id="c90e7-120">Novas funcionalidades adicionadas:</span><span class="sxs-lookup"><span data-stu-id="c90e7-120">Added new features:</span></span>
    - <span data-ttu-id="c90e7-121">Mapeamento de entrada</span><span class="sxs-lookup"><span data-stu-id="c90e7-121">Input mapping</span></span>
    - <span data-ttu-id="c90e7-122">Esquema de Entrega de Eventos</span><span class="sxs-lookup"><span data-stu-id="c90e7-122">Event Delivery Schema</span></span>
    - <span data-ttu-id="c90e7-123">Ligação Privada</span><span class="sxs-lookup"><span data-stu-id="c90e7-123">Private Link</span></span>
    - <span data-ttu-id="c90e7-124">Esquema de Eventos na Cloud V10</span><span class="sxs-lookup"><span data-stu-id="c90e7-124">Cloud Event V10 Schema</span></span>
    - <span data-ttu-id="c90e7-125">Tópico do Service Bus como Destino</span><span class="sxs-lookup"><span data-stu-id="c90e7-125">Service Bus Topic As Destination</span></span>
    - <span data-ttu-id="c90e7-126">Função do Azure como Destino</span><span class="sxs-lookup"><span data-stu-id="c90e7-126">Azure Function As Destination</span></span>
    - <span data-ttu-id="c90e7-127">Criação de batches do WebHook</span><span class="sxs-lookup"><span data-stu-id="c90e7-127">WebHook Batching</span></span>
    - <span data-ttu-id="c90e7-128">Webhook seguro (suporte de AAD)</span><span class="sxs-lookup"><span data-stu-id="c90e7-128">Secure webhook (AAD support)</span></span>
    - <span data-ttu-id="c90e7-129">IpFiltering</span><span class="sxs-lookup"><span data-stu-id="c90e7-129">IpFiltering</span></span>
* <span data-ttu-id="c90e7-130">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="c90e7-130">Updated cmdlets:</span></span>
    - <span data-ttu-id="c90e7-131">"New-AzEventGridSubscription"/"Update-AzEventGridSubscription":</span><span class="sxs-lookup"><span data-stu-id="c90e7-131">'New-AzEventGridSubscription'/'Update-AzEventGridSubscription':</span></span>
        - <span data-ttu-id="c90e7-132">Adicionar novos parâmetros opcionais para suportar a criação de batches do webhook.</span><span class="sxs-lookup"><span data-stu-id="c90e7-132">Add new optional parameters to support webhook batching.</span></span>
        - <span data-ttu-id="c90e7-133">Adicionar novos parâmetros opcionais para suportar o webhook seguro através do AAD.</span><span class="sxs-lookup"><span data-stu-id="c90e7-133">Add new optional parameters to support secured webhook using AAD.</span></span>
        - <span data-ttu-id="c90e7-134">Adicionar uma nova enumeração para o parâmetro EndpointType para suportar a função do Azure e o tópico do Service Bus enquanto novos destinos.</span><span class="sxs-lookup"><span data-stu-id="c90e7-134">Add new enum for EndpointType parameter to support azure function and service bus topic as new destinations.</span></span>
        - <span data-ttu-id="c90e7-135">Adicionar novo parâmetro opcional para o esquema de entrega.</span><span class="sxs-lookup"><span data-stu-id="c90e7-135">Add new optional parameter for delivery schema.</span></span>
    - <span data-ttu-id="c90e7-136">"New-AzEventGridTopic"/"Update-AzEventGridTopic" e "New-AzEventGridDomain"/"Update-AzEventGridDomain":</span><span class="sxs-lookup"><span data-stu-id="c90e7-136">'New-AzEventGridTopic'/'Update-AzEventGridTopic' and 'New-AzEventGridDomain'/'Update-AzEventGridDomain':</span></span>
        - <span data-ttu-id="c90e7-137">Adicionar novos parâmetros opcionais para suportar IpFiltering.</span><span class="sxs-lookup"><span data-stu-id="c90e7-137">Add new optional parameters to support IpFiltering.</span></span>
    - <span data-ttu-id="c90e7-138">"New-AzEventGridTopic"/"New-AzEventGridDomain":</span><span class="sxs-lookup"><span data-stu-id="c90e7-138">'New-AzEventGridTopic'/'New-AzEventGridDomain':</span></span>
        - <span data-ttu-id="c90e7-139">Adicionar novos parâmetros opcionais para suportar o Mapeamento de entrada.</span><span class="sxs-lookup"><span data-stu-id="c90e7-139">Add new optional parameters to support Input mapping.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c90e7-140">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c90e7-140">Az.FrontDoor</span></span>
* <span data-ttu-id="c90e7-141">Módulo atualizado para utilizar a API 2020-05-01</span><span class="sxs-lookup"><span data-stu-id="c90e7-141">Updated module to use API 2020-05-01</span></span>
* <span data-ttu-id="c90e7-142">Adição de suporte do Private Link para recursos de Armazenamento, Cofre de chaves e Serviço de Aplicações Web</span><span class="sxs-lookup"><span data-stu-id="c90e7-142">Added Private link support for Storage, Keyvault and Web App Service resources</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c90e7-143">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c90e7-143">Az.HDInsight</span></span>
* <span data-ttu-id="c90e7-144">Suporte para a criação de cluster com armazenamento ADLSGen1/2 em clouds nacionais.</span><span class="sxs-lookup"><span data-stu-id="c90e7-144">Supported creating cluster with ADLSGen1/2 storage in national clouds.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c90e7-145">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-145">Az.Monitor</span></span>
* <span data-ttu-id="c90e7-146">Correção do erro em "Get-AzDiagnosticSetting" quando as métricas ou registos são nulos [#12272]</span><span class="sxs-lookup"><span data-stu-id="c90e7-146">Fixed bug for 'Get-AzDiagnosticSetting' when metrics or logs are null [#12272]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-147">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-147">Az.Network</span></span>
* <span data-ttu-id="c90e7-148">Correção da troca de parâmetros na ligação VWan HubVnet</span><span class="sxs-lookup"><span data-stu-id="c90e7-148">Fixed parameters swap in VWan HubVnet connection</span></span>
* <span data-ttu-id="c90e7-149">Adição de novos cmdlets para Sites de Aplicações Virtuais da Rede Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-149">Added new cmdlets for Azure Network Virtual Appliance Sites</span></span>
    - <span data-ttu-id="c90e7-150">"Get-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="c90e7-150">'Get-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="c90e7-151">"New-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="c90e7-151">'New-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="c90e7-152">"Remove-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="c90e7-152">'Remove-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="c90e7-153">"Update-AzVirtualApplianceSite"</span><span class="sxs-lookup"><span data-stu-id="c90e7-153">'Update-AzVirtualApplianceSite'</span></span>
    - <span data-ttu-id="c90e7-154">"New-AzOffice365PolicyProperty"</span><span class="sxs-lookup"><span data-stu-id="c90e7-154">'New-AzOffice365PolicyProperty'</span></span>
* <span data-ttu-id="c90e7-155">Adição de novos cmdlets para Aplicações Virtuais da Rede Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-155">Added new cmdlets for Azure Network Virtual Appliance</span></span>
    - <span data-ttu-id="c90e7-156">"Get-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="c90e7-156">'Get-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="c90e7-157">"New-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="c90e7-157">'New-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="c90e7-158">"Remove-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="c90e7-158">'Remove-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="c90e7-159">"Update-AzNetworkVirtualAppliance"</span><span class="sxs-lookup"><span data-stu-id="c90e7-159">'Update-AzNetworkVirtualAppliance'</span></span>
    - <span data-ttu-id="c90e7-160">"Get-AzNetworkVirtualApplianceSku"</span><span class="sxs-lookup"><span data-stu-id="c90e7-160">'Get-AzNetworkVirtualApplianceSku'</span></span>
    - <span data-ttu-id="c90e7-161">"New-AzVirtualApplianceSkuProperty"</span><span class="sxs-lookup"><span data-stu-id="c90e7-161">'New-AzVirtualApplianceSkuProperty'</span></span>
* <span data-ttu-id="c90e7-162">Gateway de Aplicação integrado para Cmdlets Comuns do Private Link</span><span class="sxs-lookup"><span data-stu-id="c90e7-162">Onboarded Application Gateway to Private Link Common Cmdlets</span></span>
* <span data-ttu-id="c90e7-163">StorageSync integrado para Cmdlets Comuns do Private Link</span><span class="sxs-lookup"><span data-stu-id="c90e7-163">Onboarded StorageSync to Private Link Common Cmdlets</span></span>
* <span data-ttu-id="c90e7-164">SignalR integrado para Cmdlets Comuns do Private Link</span><span class="sxs-lookup"><span data-stu-id="c90e7-164">Onboarded SignalR to Private Link Common Cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-165">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-165">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-166">Remoção da referência do projeto para Autenticação</span><span class="sxs-lookup"><span data-stu-id="c90e7-166">Removed project reference to Authentication</span></span>
* <span data-ttu-id="c90e7-167">Os cmdlets afinados do Azure Backup ajudam o texto a ser mais preciso.</span><span class="sxs-lookup"><span data-stu-id="c90e7-167">Azure Backup tuned cmdlets help text to be more accurate.</span></span>
* <span data-ttu-id="c90e7-168">O Azure Backup adicionou suporte para obter tarefas de agentes MAB através do cmdlet "Get-AzRecoveryServicesBackupJob".</span><span class="sxs-lookup"><span data-stu-id="c90e7-168">Azure Backup added support for fetching MAB agent jobs using 'Get-AzRecoveryServicesBackupJob' cmdlet.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-169">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-169">Az.Resources</span></span>
* <span data-ttu-id="c90e7-170">Atualização de "Save-AzResourceGroupDeploymentTemplate" para utilizar o SDK.</span><span class="sxs-lookup"><span data-stu-id="c90e7-170">Updated 'Save-AzResourceGroupDeploymentTemplate' to use the SDK.</span></span>
* <span data-ttu-id="c90e7-171">Adição do cmdlet "Unregister-AzResourceProvider".</span><span class="sxs-lookup"><span data-stu-id="c90e7-171">Added 'Unregister-AzResourceProvider' cmdlet.</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-172">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-172">Az.Sql</span></span>
* <span data-ttu-id="c90e7-173">Adição de suporte para o Principal de serviço e utilizadores convidados no cmdlet Set-AzSqlInstanceActiveDirectoryAdministrator</span><span class="sxs-lookup"><span data-stu-id="c90e7-173">Added support for Service principal and guest users in Set-AzSqlInstanceActiveDirectoryAdministrator cmdlet'</span></span>
* <span data-ttu-id="c90e7-174">Correção de um erro em cmdlets de Classificação de Dados.</span><span class="sxs-lookup"><span data-stu-id="c90e7-174">Fixed a bug in Data Classification cmdlets.'</span></span>
* <span data-ttu-id="c90e7-175">Adição de suporte para a ativação pós-falha do Azure SQL Managed Instance: "Invoke-AzSqlInstanceFailover"</span><span class="sxs-lookup"><span data-stu-id="c90e7-175">Added support for Azure SQL Managed Instance failover: 'Invoke-AzSqlInstanceFailover'</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-176">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-176">Az.Storage</span></span>
* <span data-ttu-id="c90e7-177">Correção do erro de que o UserAgent não é adicionado para alguns cmdlets do plano de dados.</span><span class="sxs-lookup"><span data-stu-id="c90e7-177">Fixed the issue that UserAgent is not added for some data plane cmdlets.</span></span>
* <span data-ttu-id="c90e7-178">Suporte para a criação/atualização da Conta de armazenamento com MinimumTlsVersion e AllowBlobPublicAccess</span><span class="sxs-lookup"><span data-stu-id="c90e7-178">Supported create/update Storage account with MinimumTlsVersion and AllowBlobPublicAccess</span></span>
    -  <span data-ttu-id="c90e7-179">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c90e7-179">'New-AzStorageAccount'</span></span>
    -  <span data-ttu-id="c90e7-180">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c90e7-180">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="c90e7-181">Suporte para Permitir/desativar o controlo de versões no Serviço Blob de uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="c90e7-181">Support enable/disable versioning on Blob Service of a Storage account</span></span>
    - <span data-ttu-id="c90e7-182">"Update-AzStorageBlobServiceProperty"</span><span class="sxs-lookup"><span data-stu-id="c90e7-182">'Update-AzStorageBlobServiceProperty'</span></span>
* <span data-ttu-id="c90e7-183">Suporte para a lista de blobs com versões de blobs</span><span class="sxs-lookup"><span data-stu-id="c90e7-183">Support list blobs with blob versions</span></span>
    - <span data-ttu-id="c90e7-184">"Get-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="c90e7-184">'Get-AzStorageBlob'</span></span>
* <span data-ttu-id="c90e7-185">Suporte para obter/remover instantâneo de blob único ou versão do blob</span><span class="sxs-lookup"><span data-stu-id="c90e7-185">Support get/remove single blob snapshot or blob version</span></span>
    - <span data-ttu-id="c90e7-186">"Get-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="c90e7-186">'Get-AzStorageBlob'</span></span>
    - <span data-ttu-id="c90e7-187">"Remove-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="c90e7-187">'Remove-AzStorageBlob'</span></span>
* <span data-ttu-id="c90e7-188">Suporte para pipeline a partir do objeto de blob gerado a partir de Azure.Storage.Blobs V12</span><span class="sxs-lookup"><span data-stu-id="c90e7-188">Support pipeline from blob object generated from Azure.Storage.Blobs V12</span></span>
    - <span data-ttu-id="c90e7-189">"Get-AzStorageBlobContent"</span><span class="sxs-lookup"><span data-stu-id="c90e7-189">'Get-AzStorageBlobContent'</span></span>
    - <span data-ttu-id="c90e7-190">"New-AzStorageBlobSASToken"</span><span class="sxs-lookup"><span data-stu-id="c90e7-190">'New-AzStorageBlobSASToken'</span></span>
    - <span data-ttu-id="c90e7-191">"Remove-AzStorageBlob"</span><span class="sxs-lookup"><span data-stu-id="c90e7-191">'Remove-AzStorageBlob'</span></span>
    - <span data-ttu-id="c90e7-192">"Set-AzStorageBlobContent"</span><span class="sxs-lookup"><span data-stu-id="c90e7-192">'Set-AzStorageBlobContent'</span></span>
    - <span data-ttu-id="c90e7-193">"Start-AzStorageBlobCopy"</span><span class="sxs-lookup"><span data-stu-id="c90e7-193">'Start-AzStorageBlobCopy'</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="c90e7-194">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="c90e7-194">Az.StorageSync</span></span>
* <span data-ttu-id="c90e7-195">Adição de uma nova versão StorageSync SDK para ApiVersion 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="c90e7-195">Added a new version StorageSync SDK targeting ApiVersion 2020-03-01</span></span>
* <span data-ttu-id="c90e7-196">Adição de cmdlet do Serviço de Sincronização de Armazenamento de Atualização</span><span class="sxs-lookup"><span data-stu-id="c90e7-196">Added Update Storage Sync Service cmdlet</span></span>
    - <span data-ttu-id="c90e7-197">"Set-AzStorageSyncService"</span><span class="sxs-lookup"><span data-stu-id="c90e7-197">'Set-AzStorageSyncService'</span></span>
* <span data-ttu-id="c90e7-198">Adição de IncomingTrafficPolicy e PrivateEndpointConnections para cmdlets StorageSyncService.</span><span class="sxs-lookup"><span data-stu-id="c90e7-198">Added IncomingTrafficPolicy and PrivateEndpointConnections to StorageSyncService cmdlets.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-199">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-199">Az.Websites</span></span>
* <span data-ttu-id="c90e7-200">Adição de suporte para a realização de operações para Slots em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="c90e7-200">Added support to perform operations for Slots not in the same resource group as the App Service Plan</span></span>

## <a name="430---june-2020"></a><span data-ttu-id="c90e7-201">4.3.0 - Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="c90e7-201">4.3.0 - June 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c90e7-202">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-202">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-203">Suporte para a deteção da definição do ambiente por predefinição e adição de ambiente através de "Add-AzEnvironment"</span><span class="sxs-lookup"><span data-stu-id="c90e7-203">Supported discovering environment setting by default and adding environment via 'Add-AzEnvironment'</span></span>
* <span data-ttu-id="c90e7-204">Atualizar assemblagens pré-carregadas [#12024], [#11976]</span><span class="sxs-lookup"><span data-stu-id="c90e7-204">Update preloaded assemblies [#12024], [#11976]</span></span>
* <span data-ttu-id="c90e7-205">Atualização da assemblagem Azure.Core</span><span class="sxs-lookup"><span data-stu-id="c90e7-205">Updated Azure.Core assembly</span></span>
* <span data-ttu-id="c90e7-206">Correção de um problema que pode provocar a falha de "Connect-AzAccount" numa execução de múltiplos threads [#11201]</span><span class="sxs-lookup"><span data-stu-id="c90e7-206">Fixed an issue that may cause 'Connect-AzAccount' to fail in multi-threaded execution [#11201]</span></span>

#### <a name="azaks"></a><span data-ttu-id="c90e7-207">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="c90e7-207">Az.Aks</span></span>
* <span data-ttu-id="c90e7-208">Substituição da utilização da [API AccessProfile](https://docs.microsoft.com/rest/api/aks/managedclusters/getaccessprofile) antiga por chamadas para as APIs [ListClusterAdmin](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusteradmincredentials) e [ListClusterUser](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusterusercredentials)</span><span class="sxs-lookup"><span data-stu-id="c90e7-208">Replaced usage of old [AccessProfile API](https://docs.microsoft.com/rest/api/aks/managedclusters/getaccessprofile) with calls to [ListClusterAdmin](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusteradmincredentials) and [ListClusterUser](https://docs.microsoft.com/rest/api/aks/managedclusters/listclusterusercredentials) APIs</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c90e7-209">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c90e7-209">Az.Batch</span></span>
* <span data-ttu-id="c90e7-210">Atualização da versão do SDK de Az.Batch para utilizar "Microsoft.Azure.Management.Batch" para 11.0.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-210">Updated Az.Batch to use 'Microsoft.Azure.Management.Batch' SDK version to 11.0.0</span></span>
* <span data-ttu-id="c90e7-211">Adição da capacidade de definir a Identidade BatchAccount no cmdlet "New-AzBatchAccount"</span><span class="sxs-lookup"><span data-stu-id="c90e7-211">Added the ability to set the BatchAccount Identity in the 'New-AzBatchAccount' cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c90e7-212">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-212">Az.CognitiveServices</span></span>
* <span data-ttu-id="c90e7-213">Suporte para a apresentação das capacidades da conta.</span><span class="sxs-lookup"><span data-stu-id="c90e7-213">Supported displaying account capabilities.</span></span>
* <span data-ttu-id="c90e7-214">Suporte para a modificação de PublicNetworkAccess.</span><span class="sxs-lookup"><span data-stu-id="c90e7-214">Supported modifying PublicNetworkAccess.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-215">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-215">Az.Compute</span></span>
* <span data-ttu-id="c90e7-216">Adição do parâmetro SimulateEviction aos cmdlets Set-AzVM e Set-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="c90e7-216">Added SimulateEviction parameter to Set-AzVM and Set-AzVmssVM cmdlets.</span></span>
* <span data-ttu-id="c90e7-217">Adição de "Premium_LRS" ao mecanismo de preenchimento de argumentos do parâmetro StorageAccountType para o cmdlet New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="c90e7-217">Added 'Premium_LRS' to the argument completer of StorageAccountType parameter for New-AzGalleryImageVersion cmdlet.</span></span>
* <span data-ttu-id="c90e7-218">Adição de subestados a VMCustomScriptExtension [#11297]</span><span class="sxs-lookup"><span data-stu-id="c90e7-218">Added Substatuses to VMCustomScriptExtension [#11297]</span></span>
* <span data-ttu-id="c90e7-219">Adição de "Delete" ao mecanismo de preenchimento de argumentos do parâmetro EvictionPolicy para os cmdlets New-AzVM e New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="c90e7-219">Added 'Delete' to the argument completer of EvictionPolicy parameter for New-AzVM and New-AzVMConfig cmdlets.</span></span>
* <span data-ttu-id="c90e7-220">Correção do nome da nova Extensão de VM para SAP</span><span class="sxs-lookup"><span data-stu-id="c90e7-220">Fixed name of new VM Extension for SAP</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-221">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-221">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-222">Atualização da versão do SDK de .Net do ADF para 4.9.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-222">Updated ADF .Net SDK version to 4.9.0</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c90e7-223">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-223">Az.EventHub</span></span>
* <span data-ttu-id="c90e7-224">Adição de parâmetros de Identidade Gerida aos cmdlets "New-AzEventHubNamespace" e "Set-AzEventHubNamespace"</span><span class="sxs-lookup"><span data-stu-id="c90e7-224">Added Managed Identity parameters to 'New-AzEventHubNamespace' and 'Set-AzEventHubNamespace' cmdlets</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="c90e7-225">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="c90e7-225">Az.Functions</span></span>
* <span data-ttu-id="c90e7-226">Adição de suporte para a criação de aplicações de funções do PowerShell 7.0 e de Java 11</span><span class="sxs-lookup"><span data-stu-id="c90e7-226">Added support to create PowerShell 7.0 and Java 11 function apps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c90e7-227">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c90e7-227">Az.HDInsight</span></span>
* <span data-ttu-id="c90e7-228">Suporte para listagem de anfitriões e reinício de anfitriões específicos do cluster HDInsight.</span><span class="sxs-lookup"><span data-stu-id="c90e7-228">Supported listing hosts and restart specific hosts of the HDInsight cluster.</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="c90e7-229">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="c90e7-229">Az.HealthcareApis</span></span>
* <span data-ttu-id="c90e7-230">Atualização da versão do SDK para 1.1.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-230">Updated the SDK version to 1.1.0</span></span>
* <span data-ttu-id="c90e7-231">Adição de suporte para as definições de Exportação e a Identidade Gerida</span><span class="sxs-lookup"><span data-stu-id="c90e7-231">Added support for Export settings and Managed Identity</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c90e7-232">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-232">Az.Monitor</span></span>
* <span data-ttu-id="c90e7-233">Correção do parâmetro de objeto de entrada para "Set-AzActivityLogAlert"</span><span class="sxs-lookup"><span data-stu-id="c90e7-233">Fixed input object parameter for 'Set-AzActivityLogAlert'</span></span>
* <span data-ttu-id="c90e7-234">Correção do parâmetro "InputObject" para "Set-AzActionGroup" [#10868]</span><span class="sxs-lookup"><span data-stu-id="c90e7-234">Fixed 'InputObject' parameter for 'Set-AzActionGroup' [#10868]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-235">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-235">Az.Network</span></span>
* <span data-ttu-id="c90e7-236">Adição de suporte para o parâmetro AddressPrefixType a "Remove-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="c90e7-236">Added support for AddressPrefixType parameter to 'Remove-AzExpressRouteCircuitConnectionConfig'</span></span>
* <span data-ttu-id="c90e7-237">Adição de novos cmdlets para a Política de Firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-237">Added new cmdlets for Azure FirewallPolicy</span></span>
    - <span data-ttu-id="c90e7-238">"New-AzFirewallPolicyDnsSetting"</span><span class="sxs-lookup"><span data-stu-id="c90e7-238">'New-AzFirewallPolicyDnsSetting'</span></span>
    - <span data-ttu-id="c90e7-239">Suporte para FQDN de Destino nas Regras de Rede para a Política de Firewall</span><span class="sxs-lookup"><span data-stu-id="c90e7-239">Support for Destination FQDN in Network Rules for Firewall Policy</span></span>
* <span data-ttu-id="c90e7-240">Adição de suporte para operações de conjuntos de endereços back-end</span><span class="sxs-lookup"><span data-stu-id="c90e7-240">Added support for backend address pool operations</span></span>
    - <span data-ttu-id="c90e7-241">"New-AzLoadBalancerBackendAddressConfig"</span><span class="sxs-lookup"><span data-stu-id="c90e7-241">'New-AzLoadBalancerBackendAddressConfig'</span></span>
    - <span data-ttu-id="c90e7-242">"New-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="c90e7-242">'New-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="c90e7-243">"Set-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="c90e7-243">'Set-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="c90e7-244">"Remove-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="c90e7-244">'Remove-AzLoadBalancerBackendAddressPool'</span></span>
    - <span data-ttu-id="c90e7-245">"Get-AzLoadBalancerBackendAddressPool"</span><span class="sxs-lookup"><span data-stu-id="c90e7-245">'Get-AzLoadBalancerBackendAddressPool'</span></span>
* <span data-ttu-id="c90e7-246">Adição de validação de nomes para "New-AzIpGroup"</span><span class="sxs-lookup"><span data-stu-id="c90e7-246">Added name validation for 'New-AzIpGroup'</span></span>
* <span data-ttu-id="c90e7-247">Adição de novos cmdlets para a Política de Firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-247">Added new cmdlets for Azure FirewallPolicy</span></span>
    - <span data-ttu-id="c90e7-248">"New-AzFirewallPolicyThreatIntelWhitelist"</span><span class="sxs-lookup"><span data-stu-id="c90e7-248">'New-AzFirewallPolicyThreatIntelWhitelist'</span></span>
* <span data-ttu-id="c90e7-249">Foram atualizados os seguintes comandos para a funcionalidade: Definição/remoção de servidores DNS personalizados no P2SVpnGateway de VirtualWan.</span><span class="sxs-lookup"><span data-stu-id="c90e7-249">Updated below commands for feature: Custom dns servers set/remove on VirtualWan P2SVpnGateway.</span></span>
    - <span data-ttu-id="c90e7-250">Atualização de New-AzP2sVpnGateway: Adição do parâmetro opcional "-CustomDnsServer" para os clientes especificarem os respetivos servidores DNS a definir no P2SVpnGateway, o qual pode ser utilizado por clientes do tipo Ponto a site.</span><span class="sxs-lookup"><span data-stu-id="c90e7-250">Updated New-AzP2sVpnGateway: Added optional parameter '-CustomDnsServer' for customers to specify their dns servers to set on P2SVpnGateway, which can be used by Point to site clients.</span></span>
    - <span data-ttu-id="c90e7-251">Atualização de Update-AzP2sVpnGateway: Adição do parâmetro opcional "-CustomDnsServer" para os clientes especificarem os respetivos servidores DNS a definir no P2SVpnGateway, o qual pode ser utilizado por clientes do tipo Ponto a site.</span><span class="sxs-lookup"><span data-stu-id="c90e7-251">Updated Update-AzP2sVpnGateway: Added optional parameter '-CustomDnsServer' for customers to specify their dns servers to set on P2SVpnGateway, which can be used by Point to site clients.</span></span>
* <span data-ttu-id="c90e7-252">Atualização de "Update-AzVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="c90e7-252">Updated 'Update-AzVpnGateway'</span></span>
    - <span data-ttu-id="c90e7-253">Adição do parâmetro opcional "-BgpPeeringAddress" para os clientes especificarem os respetivos bgps personalizados a definir no VpnGateway.</span><span class="sxs-lookup"><span data-stu-id="c90e7-253">Added optional parameter '-BgpPeeringAddress' for customers to specify their custom bgps to set on VpnGateway.</span></span>
* <span data-ttu-id="c90e7-254">Adição de novo cmdlet para suportar a reposição do estado de encaminhamento de um recurso VirtualHub:</span><span class="sxs-lookup"><span data-stu-id="c90e7-254">Added new cmdlet to support resetting the routing state of a VirtualHub resource:</span></span>
    - <span data-ttu-id="c90e7-255">"Reset-AzHubRouter"</span><span class="sxs-lookup"><span data-stu-id="c90e7-255">'Reset-AzHubRouter'</span></span>
* <span data-ttu-id="c90e7-256">Atualização dos elementos indicados abaixo com base na alteração recente de Swagger para a Política de Firewall</span><span class="sxs-lookup"><span data-stu-id="c90e7-256">Updated below things based on recent swagger change for Firewall Policy</span></span>
    - <span data-ttu-id="c90e7-257">Alteração de nomes para RuleGroup, RuleCollectionGroup e RuleType</span><span class="sxs-lookup"><span data-stu-id="c90e7-257">Changes names for RuleGroup, RuleCollectionGroup and RuleType</span></span>
    - <span data-ttu-id="c90e7-258">Adição de suporte para Coleções de Regras de NAT da Política de Firewall para suportar várias Coleções de Regras de NAT</span><span class="sxs-lookup"><span data-stu-id="c90e7-258">Added support for Firewall Policy NAT Rule Collections to support multiple NAT Rule Collection</span></span>
* <span data-ttu-id="c90e7-259">[Alteração Interruptiva] Adição do parâmetro obrigatório "SourceIpGroup" para "New-AzFirewallPolicyApplicationRule" e "New-AzFirewallPolicyNetworkRule".</span><span class="sxs-lookup"><span data-stu-id="c90e7-259">[Breaking Change] Added mandatory parameter 'SourceIpGroup' for 'New-AzFirewallPolicyApplicationRule' and 'New-AzFirewallPolicyNetworkRule'.</span></span>
* <span data-ttu-id="c90e7-260">[Alteração Interruptiva] Correção do parâmetro "SourceAddress" de "New-AzFirewallPolicyApplicationRule" de modo a ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c90e7-260">[Breaking Change] Fixed 'New-AzFirewallPolicyApplicationRule', parameter 'SourceAddress' to be mandatory.</span></span>
* <span data-ttu-id="c90e7-261">[Alteração Interruptiva] Correção do parâmetro "SourceAddress" de "New-AzFirewallPolicyApplicationRule" de modo a ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c90e7-261">[Breaking Change] Fixed 'New-AzFirewallPolicyApplicationRule', parameter 'SourceAddress' to be mandatory.</span></span>
* <span data-ttu-id="c90e7-262">[Alteração Interruptiva] Remoção de parâmetros obrigatórios: "TranslatedAddress", "TranslatedPort" para "New-AzFirewallPolicyNatRuleCollection".</span><span class="sxs-lookup"><span data-stu-id="c90e7-262">[Breaking Change] Removed mandatory parameters: 'TranslatedAddress', 'TranslatedPort' for 'New-AzFirewallPolicyNatRuleCollection'.</span></span>
* <span data-ttu-id="c90e7-263">Adição de novos cmdlets para suportar PrivateLink no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="c90e7-263">Added new cmdlets to support PrivateLink On Application Gateway</span></span>
    - <span data-ttu-id="c90e7-264">"New-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c90e7-264">'New-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="c90e7-265">"Get-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c90e7-265">'Get-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="c90e7-266">"New-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c90e7-266">'New-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="c90e7-267">"Set-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c90e7-267">'Set-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="c90e7-268">"Remove-AzApplicationGatewayPrivateLinkConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c90e7-268">'Remove-AzApplicationGatewayPrivateLinkConfiguration'</span></span>
    - <span data-ttu-id="c90e7-269">"New-AzApplicationGatewayPrivateLinkIpConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c90e7-269">'New-AzApplicationGatewayPrivateLinkIpConfiguration'</span></span>
* <span data-ttu-id="c90e7-270">Adição de novos cmdlets para o recurso subordinado HubRouteTables de VirtualHub.</span><span class="sxs-lookup"><span data-stu-id="c90e7-270">Added new cmdlets for HubRouteTables child resource of VirtualHub.</span></span>
    - <span data-ttu-id="c90e7-271">"New-AzVHubRoute"</span><span class="sxs-lookup"><span data-stu-id="c90e7-271">'New-AzVHubRoute'</span></span>
    - <span data-ttu-id="c90e7-272">"New-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="c90e7-272">'New-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="c90e7-273">"Get-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="c90e7-273">'Get-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="c90e7-274">"Update-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="c90e7-274">'Update-AzVHubRouteTable'</span></span>
    - <span data-ttu-id="c90e7-275">"Remove-AzVHubRouteTable"</span><span class="sxs-lookup"><span data-stu-id="c90e7-275">'Remove-AzVHubRouteTable'</span></span>
* <span data-ttu-id="c90e7-276">Atualização dos cmdlets existentes para suportar o parâmetro de entrada opcional RoutingConfiguration para encaminhamento personalizado em VirtualWan.</span><span class="sxs-lookup"><span data-stu-id="c90e7-276">Updated existing cmdlets to support optional RoutingConfiguration input parameter for custom routing in VirtualWan.</span></span>
    - <span data-ttu-id="c90e7-277">"New-AzExpressRouteConnection"</span><span class="sxs-lookup"><span data-stu-id="c90e7-277">'New-AzExpressRouteConnection'</span></span>
    - <span data-ttu-id="c90e7-278">"Set-AzExpressRouteConnection"</span><span class="sxs-lookup"><span data-stu-id="c90e7-278">'Set-AzExpressRouteConnection'</span></span>
    - <span data-ttu-id="c90e7-279">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="c90e7-279">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="c90e7-280">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="c90e7-280">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="c90e7-281">"New-AzVpnConnection"</span><span class="sxs-lookup"><span data-stu-id="c90e7-281">'New-AzVpnConnection'</span></span>
    - <span data-ttu-id="c90e7-282">"Update-AzVpnConnection"</span><span class="sxs-lookup"><span data-stu-id="c90e7-282">'Update-AzVpnConnection'</span></span>
    - <span data-ttu-id="c90e7-283">"New-AzP2sVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="c90e7-283">'New-AzP2sVpnGateway'</span></span>
    - <span data-ttu-id="c90e7-284">"Update-AzP2sVpnGateway"</span><span class="sxs-lookup"><span data-stu-id="c90e7-284">'Update-AzP2sVpnGateway'</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c90e7-285">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-285">Az.OperationalInsights</span></span>
* <span data-ttu-id="c90e7-286">Correção do erro PSWorkspace não implementa IOperationalInsightsWorkspace [#12135]</span><span class="sxs-lookup"><span data-stu-id="c90e7-286">Fixed bug PSWorkspace doesn't implement IOperationalInsightsWorkspace [#12135]</span></span>
* <span data-ttu-id="c90e7-287">Adição de "pergb2018" ao conjunto de valores válidos do parâmetro "Sku" em "Set-AzOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="c90e7-287">Added 'pergb2018' to valid value set of parameter 'Sku' in 'Set-AzOperationalInsightsWorkspace'</span></span> 
* <span data-ttu-id="c90e7-288">Adição do alias "FunctionParameters" para o parâmetro "FunctionParameter" a</span><span class="sxs-lookup"><span data-stu-id="c90e7-288">Added alias 'FunctionParameters' for parameter 'FunctionParameter' to</span></span>
    - <span data-ttu-id="c90e7-289">"New-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="c90e7-289">'New-AzOperationalInsightsSavedSearch'</span></span>
    - <span data-ttu-id="c90e7-290">"Set-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="c90e7-290">'Set-AzOperationalInsightsSavedSearch'</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-291">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-291">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-292">Adição de suporte no Azure Backup para a obtenção de itens de MAB.</span><span class="sxs-lookup"><span data-stu-id="c90e7-292">Azure Backup added support for fetching MAB items.</span></span>
* <span data-ttu-id="c90e7-293">Suporte do Azure Site Recovery para o tipo de disco "StandardSSD_LRS"</span><span class="sxs-lookup"><span data-stu-id="c90e7-293">Azure Site Recovery supports disk type 'StandardSSD_LRS'</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-294">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-294">Az.Resources</span></span>
* <span data-ttu-id="c90e7-295">Adição de "UsageLocation", "GivenName", "Surname", "AccountEnabled", "MailNickname", "Mail" em "PSADUser" [#10526] [#10497]</span><span class="sxs-lookup"><span data-stu-id="c90e7-295">Added 'UsageLocation', 'GivenName', 'Surname', 'AccountEnabled', 'MailNickname', 'Mail' on 'PSADUser' [#10526] [#10497]</span></span>
* <span data-ttu-id="c90e7-296">Correção do problema em que "-Mail" não funciona em "Get-AzADUser" [#11981]</span><span class="sxs-lookup"><span data-stu-id="c90e7-296">Fixed issue that '-Mail' doesn't work on 'Get-AzADUser' [#11981]</span></span>
* <span data-ttu-id="c90e7-297">Adição do parâmetro "-ExcludeChangeType" a "Get-AzDeploymentWhatIfResult" e "Get-AzResourceGroupDeploymentWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="c90e7-297">Added '-ExcludeChangeType' parameter to 'Get-AzDeploymentWhatIfResult' and 'Get-AzResourceGroupDeploymentWhatIfResult'</span></span>
* <span data-ttu-id="c90e7-298">Adição do parâmetro "-WhatIfExcludeChangeType" a "New-AzDeployment" e "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="c90e7-298">Added '-WhatIfExcludeChangeType' parameter to 'New-AzDeployment' and 'New-AzResourceGroupDeployment'</span></span>
* <span data-ttu-id="c90e7-299">Atualização de cmdlets "Test-Az\*Deployment" para apresentação de mensagens de erro melhores</span><span class="sxs-lookup"><span data-stu-id="c90e7-299">Updated 'Test-Az\*Deployment' cmdlets to show better error messages</span></span>
* <span data-ttu-id="c90e7-300">Correção da mensagem de ajuda para o parâmetro "-Name" de criação de implementação e cmdlets What-If</span><span class="sxs-lookup"><span data-stu-id="c90e7-300">Fixed help message for '-Name' parameter of deployment create and What-If cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-301">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-301">Az.Sql</span></span>
* <span data-ttu-id="c90e7-302">Adição de suporte para o principal de serviço para o cmdlet Set SQL Server Azure Active Directory Admin</span><span class="sxs-lookup"><span data-stu-id="c90e7-302">Added support for service principal for Set SQL Server Azure Active Directory Admin cmdlet</span></span>
* <span data-ttu-id="c90e7-303">Correção de problema de sincronização em cmdlets de Classificação de Dados.</span><span class="sxs-lookup"><span data-stu-id="c90e7-303">Fixed sync issue in Data Classification cmdlets.</span></span>
* <span data-ttu-id="c90e7-304">Suporte para a pesquisa de utilizador por correio em "Set-AzSqlServerActiveDirectoryAdministrator" [#12192]</span><span class="sxs-lookup"><span data-stu-id="c90e7-304">Supported searching user by mail on 'Set-AzSqlServerActiveDirectoryAdministrator' [#12192]</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-305">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-305">Az.Storage</span></span>
* <span data-ttu-id="c90e7-306">Suporte para a criação de Conta de armazenamento com RequireInfrastructureEncryption</span><span class="sxs-lookup"><span data-stu-id="c90e7-306">Supported create Storage account with RequireInfrastructureEncryption</span></span>
    -  <span data-ttu-id="c90e7-307">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c90e7-307">'New-AzStorageAccount'</span></span>
* <span data-ttu-id="c90e7-308">Mudança da lógica de carregamento de Azure.Core para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-308">Moved the logic of loading Azure.Core to Az.Accounts</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-309">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-309">Az.Websites</span></span>
* <span data-ttu-id="c90e7-310">Adição de salvaguarda para eliminar a aplicação Web criada em caso de falha do restauro em "Restore-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="c90e7-310">Added safeguard to delete created webapp if restore failed in 'Restore-AzDeletedWebApp'</span></span>
* <span data-ttu-id="c90e7-311">Adição de "SourceWebApp.Location" para "New-AzWebApp" e "New-AzWebAppSlot"</span><span class="sxs-lookup"><span data-stu-id="c90e7-311">Added 'SourceWebApp.Location' for 'New-AzWebApp' and 'New-AzWebAppSlot'</span></span>
* <span data-ttu-id="c90e7-312">Correção do erro que impedia a alteração de definições de Contentor em "Set-AzWebApp" e "Set-AzWebAppSlot"</span><span class="sxs-lookup"><span data-stu-id="c90e7-312">Fixed bug that prevented changing Container settings in 'Set-AzWebApp' and 'Set-AzWebAppSlot'</span></span>
* <span data-ttu-id="c90e7-313">Correção do erro para obter SiteConfig quando -Name não é fornecido para Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="c90e7-313">Fixed bug to get SiteConfig when -Name is not given for Get-AzWebApp</span></span>
* <span data-ttu-id="c90e7-314">Adição de suporte para a criação de ASP para Aplicações Linux</span><span class="sxs-lookup"><span data-stu-id="c90e7-314">Added a support to create ASP for Linux Apps</span></span>
* <span data-ttu-id="c90e7-315">Adição de exceções para clonagem entre grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="c90e7-315">Added exceptions for clone across resource groups</span></span>

## <a name="420---june-2020"></a><span data-ttu-id="c90e7-316">4.2.0 - Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="c90e7-316">4.2.0 - June 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c90e7-317">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-317">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-318">Correção de um problema que fazia com que o Az ignorasse registos nas tarefas da Automatização do Azure ou do PowerShell [#11492]</span><span class="sxs-lookup"><span data-stu-id="c90e7-318">Fixed an issue that may cause Az to skip logs in Azure Automation or PowerShell jobs [#11492]</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c90e7-319">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-319">Az.AnalysisServices</span></span>
* <span data-ttu-id="c90e7-320">Atualização da versão de assemblagem dos cmdlets de plano de dados</span><span class="sxs-lookup"><span data-stu-id="c90e7-320">Updated assembly version of data plane cmdlets</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c90e7-321">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c90e7-321">Az.ApiManagement</span></span>
* <span data-ttu-id="c90e7-322">Atualização da versão de assemblagem dos cmdlets de gestão de serviços</span><span class="sxs-lookup"><span data-stu-id="c90e7-322">Updated assembly version of service management cmdlets</span></span>

#### <a name="azbilling"></a><span data-ttu-id="c90e7-323">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="c90e7-323">Az.Billing</span></span>
* <span data-ttu-id="c90e7-324">Atualização da versão de assemblagem dos cmdlets de consumo</span><span class="sxs-lookup"><span data-stu-id="c90e7-324">Updated assembly version of consumption cmdlets</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c90e7-325">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-325">Az.CognitiveServices</span></span>
* <span data-ttu-id="c90e7-326">Suporte para o controlo de PrivateEndpoint e PublicNetworkAccess.</span><span class="sxs-lookup"><span data-stu-id="c90e7-326">Support PrivateEndpoint and PublicNetworkAccess control.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-327">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-327">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-328">Atualização da versão de assemblagem dos cmdlets V2 de fábrica de dados</span><span class="sxs-lookup"><span data-stu-id="c90e7-328">Updated assembly version of data factory V2 cmdlets</span></span>

#### <a name="azdatashare"></a><span data-ttu-id="c90e7-329">Az.DataShare</span><span class="sxs-lookup"><span data-stu-id="c90e7-329">Az.DataShare</span></span>
* <span data-ttu-id="c90e7-330">Disponibilidade geral do módulo "Az.DataShare"</span><span class="sxs-lookup"><span data-stu-id="c90e7-330">General availability of ''Az.DataShare'' module</span></span>

#### <a name="azdesktopvirtualization"></a><span data-ttu-id="c90e7-331">Az.DesktopVirtualization</span><span class="sxs-lookup"><span data-stu-id="c90e7-331">Az.DesktopVirtualization</span></span>
* <span data-ttu-id="c90e7-332">Disponibilidade geral do módulo "Az.DesktopVirtualization"</span><span class="sxs-lookup"><span data-stu-id="c90e7-332">General availability of ''Az.DesktopVirtualization'' module</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c90e7-333">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-333">Az.OperationalInsights</span></span>
* <span data-ttu-id="c90e7-334">Atualização do SDK para a versão 0.21.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-334">Upgraded SDK to 0.21.0</span></span>
* <span data-ttu-id="c90e7-335">Adição de parâmetros opcionais a</span><span class="sxs-lookup"><span data-stu-id="c90e7-335">Added optional parameters to</span></span> 
    - <span data-ttu-id="c90e7-336">"New-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="c90e7-336">'New-AzOperationalInsightsSavedSearch'</span></span>
    - <span data-ttu-id="c90e7-337">"Set-AzOperationalInsightsSavedSearch"</span><span class="sxs-lookup"><span data-stu-id="c90e7-337">'Set-AzOperationalInsightsSavedSearch'</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c90e7-338">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-338">Az.PolicyInsights</span></span>
* <span data-ttu-id="c90e7-339">Correção do exemplo 3 de "Start-AzPolicyComplianceScan"</span><span class="sxs-lookup"><span data-stu-id="c90e7-339">Corrected example 3 for 'Start-AzPolicyComplianceScan'</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="c90e7-340">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="c90e7-340">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="c90e7-341">Atualização da versão de assemblagem dos cmdlets do PowerBI</span><span class="sxs-lookup"><span data-stu-id="c90e7-341">Updated assembly version of PowerBI cmdlets</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="c90e7-342">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="c90e7-342">Az.PrivateDns</span></span>
* <span data-ttu-id="c90e7-343">Correção da formatação da cadeia de saída verbosa de Remove-AzPrivateDnsRecordSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-343">Corrected verbose output string formatting for Remove-AzPrivateDnsRecordSet</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-344">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-344">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-345">Suporte do Azure Site Recovery para a criação de um plano de recuperação para replicação zona a zona a partir de uma entrada xml.</span><span class="sxs-lookup"><span data-stu-id="c90e7-345">Azure Site Recovery support for creating recovery plan for zone to zone replication from xml input.</span></span>
* <span data-ttu-id="c90e7-346">Atualização da versão de assemblagem dos cmdlets do SiteRecovery e Backup</span><span class="sxs-lookup"><span data-stu-id="c90e7-346">Updated assembly version of SiteRecovery and Backup cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-347">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-347">Az.Resources</span></span>
* <span data-ttu-id="c90e7-348">Adição do parâmetro Tail aos cmdlets Get-AzDeploymentScriptLog e Save-AzDeploymentScriptLog</span><span class="sxs-lookup"><span data-stu-id="c90e7-348">Added Tail parameter to Get-AzDeploymentScriptLog and Save-AzDeploymentScriptLog cmdlets</span></span>
* <span data-ttu-id="c90e7-349">Formatação da propriedade Output e apresentação da mesma na saída do cmdlet Get-AzDeploymentScript</span><span class="sxs-lookup"><span data-stu-id="c90e7-349">Formatted Output property and show it on the Get-AzDeploymentScript cmdlet output</span></span>
* <span data-ttu-id="c90e7-350">Mudança de nome do parâmetro -DeploymentScriptInputObject para -DeploymentScriptObject</span><span class="sxs-lookup"><span data-stu-id="c90e7-350">Renamed -DeploymentScriptInputObject parameter to -DeploymentScriptObject</span></span>
* <span data-ttu-id="c90e7-351">Correção do nome em falta do ficheiro/destino nas mensagens de cmdlet.</span><span class="sxs-lookup"><span data-stu-id="c90e7-351">Fixed missing file/target name in cmdlet messages.</span></span>
* <span data-ttu-id="c90e7-352">Atualização da versão de assemblagem dos cmdlets de gestor de recursos e de etiquetas</span><span class="sxs-lookup"><span data-stu-id="c90e7-352">Updated assembly version of resource manager and tags cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-353">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-353">Az.Sql</span></span>
* <span data-ttu-id="c90e7-354">Adição de UsePrivateLinkConnection a "New-AzSqlSyncGroup", "Update-AzSqlSyncGroup", "New-AzSqlSyncMember" e "Update-AzSqlSyncMember"</span><span class="sxs-lookup"><span data-stu-id="c90e7-354">Added UsePrivateLinkConnection to 'New-AzSqlSyncGroup', 'Update-AzSqlSyncGroup', 'New-AzSqlSyncMember' and 'Update-AzSqlSyncMember'</span></span>
* <span data-ttu-id="c90e7-355">Adição de SyncMemberAzureDatabaseResourceId a "New-AzSqlSyncMember" e "Update-AzSqlSyncMember"</span><span class="sxs-lookup"><span data-stu-id="c90e7-355">Added SyncMemberAzureDatabaseResourceId to 'New-AzSqlSyncMember' and 'Update-AzSqlSyncMember'</span></span>
* <span data-ttu-id="c90e7-356">Adição do suporte de pesquisa de Utilizador convidado ao cmdlet Set SQL Server Azure Active Directory Admin</span><span class="sxs-lookup"><span data-stu-id="c90e7-356">Added Guest user lookup support to Set SQL Server Azure Active Directory Admin cmdlet</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-357">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-357">Az.Storage</span></span>
* <span data-ttu-id="c90e7-358">Atualização da versão de assemblagem dos cmdlets de plano de dados</span><span class="sxs-lookup"><span data-stu-id="c90e7-358">Updated assembly version of data plane cmdlets</span></span>

## <a name="410---may-2020"></a><span data-ttu-id="c90e7-359">4.1.0 - Maio de 2020</span><span class="sxs-lookup"><span data-stu-id="c90e7-359">4.1.0 - May 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="c90e7-360">Destaques desde a última versão</span><span class="sxs-lookup"><span data-stu-id="c90e7-360">Highlights since the last release</span></span>
* <span data-ttu-id="c90e7-361">Versões do PowerShell suportadas: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="c90e7-361">Supported PowerShell versions: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>
* <span data-ttu-id="c90e7-362">Disponibilidade geral de Az.Functions</span><span class="sxs-lookup"><span data-stu-id="c90e7-362">General availability of Az.Functions</span></span> 
* <span data-ttu-id="c90e7-363">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources e Az.Storage são alvo de grandes versões</span><span class="sxs-lookup"><span data-stu-id="c90e7-363">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources, and Az.Storage have major release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c90e7-364">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-364">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-365">"Add-AzEnvironment" e "Set-AzEnvironment" foram atualizados para aceitar os parâmetros "AzureSynapseAnalyticsEndpointResourceId" e "AzureSynapseAnalyticsEndpointSuffix"</span><span class="sxs-lookup"><span data-stu-id="c90e7-365">Updated 'Add-AzEnvironment' and 'Set-AzEnvironment' to accept parameters 'AzureSynapseAnalyticsEndpointResourceId' and 'AzureSynapseAnalyticsEndpointSuffix'</span></span>
* <span data-ttu-id="c90e7-366">Foram adicionadas assemblagens relacionadas ao Azure.Core em Az.Accounts; as plataformas suportadas do PowerShell incluem Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span><span class="sxs-lookup"><span data-stu-id="c90e7-366">Added Azure.Core related assemblies into Az.Accounts, supported PowerShell platforms include Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span></span>

#### <a name="azaks"></a><span data-ttu-id="c90e7-367">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="c90e7-367">Az.Aks</span></span>
* <span data-ttu-id="c90e7-368">Versão da API atualizada para 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="c90e7-368">Upgraded API Version to 2019-10-01</span></span>
* <span data-ttu-id="c90e7-369">Suportado para criar o AKS com contentores do Windows</span><span class="sxs-lookup"><span data-stu-id="c90e7-369">Supported to create AKS using Windows container</span></span>
* <span data-ttu-id="c90e7-370">Novos cmdlets fornecidos: "New-AzAksNodePool", "Update-AzAksNodePool", "Remove-AzAksNodePool",        "Get-AzAksNodePool", "Install-AzAksKubectl", "Get-AzAksVersion"</span><span class="sxs-lookup"><span data-stu-id="c90e7-370">Provided new cmdlets: 'New-AzAksNodePool', 'Update-AzAksNodePool', 'Remove-AzAksNodePool',        'Get-AzAksNodePool', 'Install-AzAksKubectl', 'Get-AzAksVersion'</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c90e7-371">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c90e7-371">Az.ApiManagement</span></span>
* <span data-ttu-id="c90e7-372">"New-AzApiManagement" e "Set-AzApiManagement": o nome do parâmetro [-AssignIdentity] foi mudado para [-SystemAssignedIdentity]</span><span class="sxs-lookup"><span data-stu-id="c90e7-372">'New-AzApiManagement' and 'Set-AzApiManagement': [-AssignIdentity] parameter renamed as [-SystemAssignedIdentity]</span></span>
* <span data-ttu-id="c90e7-373">"New-AzApiManagement" e "Set-AzApiManagement": Novo parâmetro adicionado: [-UserAssignedIdentity <String[]>]</span><span class="sxs-lookup"><span data-stu-id="c90e7-373">'New-AzApiManagement' and 'Set-AzApiManagement': New parameter added: [-UserAssignedIdentity <String[]>]</span></span>
* <span data-ttu-id="c90e7-374">"Get-AzApiManagementProperty": o nome foi mudado para "Get-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="c90e7-374">'Get-AzApiManagementProperty': renamed as 'Get-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="c90e7-375">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="c90e7-375">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="c90e7-376">"New-AzApiManagementProperty": o nome foi mudado para "New-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="c90e7-376">'New-AzApiManagementProperty': renamed as 'New-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="c90e7-377">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="c90e7-377">PropertyId parameter renamed as NamedValueId.</span></span> 
* <span data-ttu-id="c90e7-378">"Set-AzApiManagementProperty": o nome foi mudado para "Set-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="c90e7-378">'Set-AzApiManagementProperty': renamed as 'Set-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="c90e7-379">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="c90e7-379">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="c90e7-380">"Remove-AzApiManagementProperty": o nome foi mudado para "Remove-AzApiManagementNamedValue".</span><span class="sxs-lookup"><span data-stu-id="c90e7-380">'Remove-AzApiManagementProperty': renamed as 'Remove-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="c90e7-381">O nome do parâmetro PropertyId foi mudado para NamedValueId.</span><span class="sxs-lookup"><span data-stu-id="c90e7-381">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="c90e7-382">Foi adicionado o cmdlet novo "Get-AzApiManagementAuthorizationServerClientSecret" e "Get-AzApiManagementAuthorizationServer" vai deixar de devolver o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="c90e7-382">Added new 'Get-AzApiManagementAuthorizationServerClientSecret' cmdlet and 'Get-AzApiManagementAuthorizationServer' will not return client secret anymore.</span></span>
* <span data-ttu-id="c90e7-383">Foi adicionado o cmdlet novo "Get-AzApiManagementNamedValueSecretValue" e "Get-AzApiManagementNamedValue" vai deixar de devolver o valor do segredo.</span><span class="sxs-lookup"><span data-stu-id="c90e7-383">Added new 'Get-AzApiManagementNamedValueSecretValue' cmdlet and 'Get-AzApiManagementNamedValue' will not return secret value.</span></span>
* <span data-ttu-id="c90e7-384">Foi adicionado o cmdlet novo "Get-AzApiManagementOpenIdConnectProviderClientSecret" e "Get-AzApiManagementOpenIdConnectProvider" vai deixar de devolver o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="c90e7-384">Added new 'Get-AzApiManagementOpenIdConnectProviderClientSecret' cmdlet and 'Get-AzApiManagementOpenIdConnectProvider' will not return client secret anymore.</span></span>
* <span data-ttu-id="c90e7-385">Foi adicionado o cmdlet "Get-AzApiManagementSubscriptionKey" e "Get-AzApiManagementSubscription" vai deixar de devolver chaves de subscrições.</span><span class="sxs-lookup"><span data-stu-id="c90e7-385">Added new 'Get-AzApiManagementSubscriptionKey' cmdlet and 'Get-AzApiManagementSubscription' will not return subscription keys anymore.</span></span>
* <span data-ttu-id="c90e7-386">Foi adicionado o cmdlet novo "Get-AzApiManagementTenantAccessSecret" e "Get-AzApiManagementTenantAccess" vai deixar de devolver chaves.</span><span class="sxs-lookup"><span data-stu-id="c90e7-386">Added new 'Get-AzApiManagementTenantAccessSecret' cmdlet and 'Get-AzApiManagementTenantAccess' will not return keys anymore.</span></span>
* <span data-ttu-id="c90e7-387">Foi adicionado o cmdlet novo "Get-AzApiManagementTenantGitAccessSecret" e "Get-AzApiManagementTenantGitAccess" vai deixar de devolver chaves.</span><span class="sxs-lookup"><span data-stu-id="c90e7-387">Added new 'Get-AzApiManagementTenantGitAccessSecret' cmdlet and 'Get-AzApiManagementTenantGitAccess' will not return keys anymore.</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="c90e7-388">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-388">Az.ApplicationInsights</span></span>
* <span data-ttu-id="c90e7-389">Parâmetros adicionados: "RetentionInDays" "PublicNetworkAccessForIngestion" "PublicNetworkAccessForQuery" a "New-AzApplicationInsights"</span><span class="sxs-lookup"><span data-stu-id="c90e7-389">Added Parameters: 'RetentionInDays' 'PublicNetworkAccessForIngestion' 'PublicNetworkAccessForQuery' for 'New-AzApplicationInsights'</span></span>
* <span data-ttu-id="c90e7-390">Foi criado o cmdlet "Update-AzApplicationInsights”</span><span class="sxs-lookup"><span data-stu-id="c90e7-390">Created cmdlet 'Update-AzApplicationInsights'</span></span>
* <span data-ttu-id="c90e7-391">Foram criados cmdlets para a Conta de Armazenamento Associada</span><span class="sxs-lookup"><span data-stu-id="c90e7-391">Created cmdlets for Linked Storage Account</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c90e7-392">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c90e7-392">Az.Batch</span></span>
* <span data-ttu-id="c90e7-393">Az.Batch foi atualizado para utilizar a versão do SDK "Microsoft.Azure.Batc" 13.0.0 e a versão do SDK "Microsoft.Azure.Management.Batch" 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="c90e7-393">Updated Az.Batch to use 'Microsoft.Azure.Batch' SDK version 13.0.0 and 'Microsoft.Azure.Management.Batch' SDK version 9.0.0.</span></span>
* <span data-ttu-id="c90e7-394">Foi adicionada a capacidade de selecionar o tipo de certificado que vai ser adicionado mediante a utilização do novo parâmetro "-CertificateKind" para "New-AzBatchCertificate".</span><span class="sxs-lookup"><span data-stu-id="c90e7-394">Added the ability to select the kind of certificate being added using the new '-CertificateKind' parameter to 'New-AzBatchCertificate'.</span></span>
* <span data-ttu-id="c90e7-395">A propriedade "ApplicationPackages" foi removida de "PSApplication", que anteriormente era sempre ''.</span><span class="sxs-lookup"><span data-stu-id="c90e7-395">Removed 'ApplicationPackages' property from 'PSApplication' which was previously always ''.</span></span>
  - <span data-ttu-id="c90e7-396">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com "Get-AzBatchApplicationPackage".</span><span class="sxs-lookup"><span data-stu-id="c90e7-396">The specific packages inside of an application now can be retrieved using 'Get-AzBatchApplicationPackage'.</span></span> <span data-ttu-id="c90e7-397">Por exemplo: "Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication".</span><span class="sxs-lookup"><span data-stu-id="c90e7-397">For example: 'Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication'.</span></span>
* <span data-ttu-id="c90e7-398">Agora, ao utilizar "New-AzBatchPool" para criar um conjunto, a propriedade "VirtualMachineImageId" de "PSImageReference" só pode fazer referência a uma imagem do Shared Image Gallery.</span><span class="sxs-lookup"><span data-stu-id="c90e7-398">When creating a pool using 'New-AzBatchPool', the 'VirtualMachineImageId' property of 'PSImageReference' can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="c90e7-399">Ao utilizar "New-AzBatchPool" para criar um conjunto, o conjunto pode ser aprovisionado sem um IP público mediante a utilização da nova propriedade "PublicIPAddressConfiguration" de "PSNetworkConfiguration".</span><span class="sxs-lookup"><span data-stu-id="c90e7-399">When creating a pool using 'New-AzBatchPool', the pool can be provisioned without a public IP using the new 'PublicIPAddressConfiguration' property of 'PSNetworkConfiguration'.</span></span>
  - <span data-ttu-id="c90e7-400">A propriedade "PublicIPs" de "PSNetworkConfiguration" foi igualmente movida para "PSPublicIPAddressConfiguration".</span><span class="sxs-lookup"><span data-stu-id="c90e7-400">The 'PublicIPs' property of 'PSNetworkConfiguration' has moved in to 'PSPublicIPAddressConfiguration' as well.</span></span> <span data-ttu-id="c90e7-401">Esta propriedade só pode ser especificada se "IPAddressProvisioningType" for "UserManaged".</span><span class="sxs-lookup"><span data-stu-id="c90e7-401">This property can only be specified if 'IPAddressProvisioningType' is 'UserManaged'.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-402">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-402">Az.Compute</span></span>
* <span data-ttu-id="c90e7-403">Foi adicionado o parâmetro HostId ao cmdlet "Update-AzVM"</span><span class="sxs-lookup"><span data-stu-id="c90e7-403">Added HostId parameter to 'Update-AzVM' cmdlet</span></span>
* <span data-ttu-id="c90e7-404">Os documentos de Ajuda para os cmdlets "New-AzVMConfig", "New-AzVmssConfig", "Update-AzVmss", "Set-AzVMOperatingSystem" e "Set-AzVmssOsProfile" foram atualizados.</span><span class="sxs-lookup"><span data-stu-id="c90e7-404">Updated Help documents for 'New-AzVMConfig', 'New-AzVmssConfig', 'Update-AzVmss', 'Set-AzVMOperatingSystem' and 'Set-AzVmssOsProfile' cmdlets.</span></span>
* <span data-ttu-id="c90e7-405">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="c90e7-405">Breaking changes</span></span>
    - <span data-ttu-id="c90e7-406">O parâmetro FilterExpression foi removido do cmdlet "Get-AzVMImage".</span><span class="sxs-lookup"><span data-stu-id="c90e7-406">FilterExpression parameter is removed from 'Get-AzVMImage' cmdlet.</span></span>
    - <span data-ttu-id="c90e7-407">O parâmetro AssignIdentity foi removido dos cmdlets "New-AzVmssConfig", "New-AzVMConfig" e "Update-AzVM".</span><span class="sxs-lookup"><span data-stu-id="c90e7-407">AssignIdentity parameter is removed from 'New-AzVmssConfig', 'New-AzVMConfig' and 'Update-AzVM' cmdlets.</span></span>
    - <span data-ttu-id="c90e7-408">AutomaticRepairMaxInstanceRepairsPercent foi removido dos cmdlets "New-AzVmssConfig" e "Update-AzVmss".</span><span class="sxs-lookup"><span data-stu-id="c90e7-408">AutomaticRepairMaxInstanceRepairsPercent is removed from 'New-AzVmssConfig' and 'Update-AzVmss' cmdlets.</span></span>
    - <span data-ttu-id="c90e7-409">As propriedades AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus e VirtualMachineScaleSetsColocationStatus foram removidas de ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="c90e7-409">AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus and VirtualMachineScaleSetsColocationStatus properties are removed from ProximityPlacementGroup.</span></span>
    - <span data-ttu-id="c90e7-410">A propriedade MaxInstanceRepairsPercent foi removida de AutomaticRepairsPolicy.</span><span class="sxs-lookup"><span data-stu-id="c90e7-410">MaxInstanceRepairsPercent property is removed from AutomaticRepairsPolicy.</span></span>
    - <span data-ttu-id="c90e7-411">Os tipos de AvailabilitySets, VirtualMachines e VirtualMachineScaleSets foram alterados de IList<SubResource> para IList<SubResourceWithColocationStatus>.</span><span class="sxs-lookup"><span data-stu-id="c90e7-411">The types of AvailabilitySets, VirtualMachines and VirtualMachineScaleSets are changed from IList<SubResource> to IList<SubResourceWithColocationStatus>.</span></span>
* <span data-ttu-id="c90e7-412">A descrição do cmdlet "Get-AzVM" foi atualizada para o descrever melhor.</span><span class="sxs-lookup"><span data-stu-id="c90e7-412">Description for 'Get-AzVM' cmdlet has been updated to better describe it.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-413">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-413">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-414">CRUD suportado das propriedades de fluxo de dados no IR Gerido.</span><span class="sxs-lookup"><span data-stu-id="c90e7-414">Supported CRUD of data flow runtime properties in Managed IR.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c90e7-415">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c90e7-415">Az.FrontDoor</span></span>
* <span data-ttu-id="c90e7-416">Foram adicionados cmdlets novos para criação, atualização, obtenção e eliminação do objeto de Motor de Regras do Front Door</span><span class="sxs-lookup"><span data-stu-id="c90e7-416">Added new cmdlets for creation, update, retreival, and deletion of Front Door Rules Engine object</span></span>
* <span data-ttu-id="c90e7-417">Foram adicionados cmdlets de programas auxiliares para construção do objeto de Motor de Regras do Front Door</span><span class="sxs-lookup"><span data-stu-id="c90e7-417">Added helper cmdlets for construction of Front Door Rules Engine object</span></span>
* <span data-ttu-id="c90e7-418">Foi adicionada a referência ao Motor de Regras ao objeto Regra de Encaminhamento do Front Door.</span><span class="sxs-lookup"><span data-stu-id="c90e7-418">Added Rules Engine reference to Front Door Routing Rule object.</span></span>
* <span data-ttu-id="c90e7-419">Foram adicionados parâmetros do Private Link ao objeto de Back-end do Front Door</span><span class="sxs-lookup"><span data-stu-id="c90e7-419">Added Private Link parameters to Front Door Backend object</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="c90e7-420">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="c90e7-420">Az.Functions</span></span>
* <span data-ttu-id="c90e7-421">Disponibilidade geral do módulo Az.Functions</span><span class="sxs-lookup"><span data-stu-id="c90e7-421">General availability of ''Az.Functions'' module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c90e7-422">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c90e7-422">Az.HDInsight</span></span>
* <span data-ttu-id="c90e7-423">Encriptação de discos de chave gerida pelo cliente suportada</span><span class="sxs-lookup"><span data-stu-id="c90e7-423">Supported Customer-managed key disk encryption.</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="c90e7-424">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="c90e7-424">Az.HealthcareApis</span></span>
* <span data-ttu-id="c90e7-425">As políticas de acesso já não são predefinidas para o principal atual</span><span class="sxs-lookup"><span data-stu-id="c90e7-425">Access policies are no longer defaulted to the current principal</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c90e7-426">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-426">Az.IotHub</span></span>
* <span data-ttu-id="c90e7-427">Foi adicionado um cmdlet para invocar uma consulta num hub IoT para obter informações mediante a utilização de uma linguagem tipo SQL.</span><span class="sxs-lookup"><span data-stu-id="c90e7-427">Added cmdlet to invoke a query in an IoT hub to retrieve information using a SQL-like language.</span></span>
* <span data-ttu-id="c90e7-428">Foi corrigido um problema em que "Add-AzIotHubDevice" falha ao criar um Dispositivo Compatível com o Edge sem dispositivos subordinados [#11597]</span><span class="sxs-lookup"><span data-stu-id="c90e7-428">Fix issue that 'Add-AzIotHubDevice' fails to create Edge Enabled Device without child devices [#11597]</span></span>
* <span data-ttu-id="c90e7-429">Foi adicionado o cmdlet para gerar o token de SAS para o Hub IoT, um dispositivo ou um módulo.</span><span class="sxs-lookup"><span data-stu-id="c90e7-429">Added cmdlet to generate SAS token for Iot Hub, device or module.</span></span>
* <span data-ttu-id="c90e7-430">Foi adicionado um cmdlet para invocar a consulta de métricas de configuração.</span><span class="sxs-lookup"><span data-stu-id="c90e7-430">Added cmdlet to invoke configuration metrics query.</span></span>
* <span data-ttu-id="c90e7-431">Gerir implementações automáticas do IoT Edge em escala.</span><span class="sxs-lookup"><span data-stu-id="c90e7-431">Manage IoT Edge automatic deployment at scale.</span></span> <span data-ttu-id="c90e7-432">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c90e7-432">New cmdlets are:</span></span>
    - <span data-ttu-id="c90e7-433">"Add-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="c90e7-433">'Add-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="c90e7-434">"Get-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="c90e7-434">'Get-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="c90e7-435">"Remove-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="c90e7-435">'Remove-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="c90e7-436">"Set-AzIotHubDeployment"</span><span class="sxs-lookup"><span data-stu-id="c90e7-436">'Set-AzIotHubDeployment'</span></span>
* <span data-ttu-id="c90e7-437">Foi adicionado um cmdlet para invocar uma consulta de métricas de implementação do IoT Edge.</span><span class="sxs-lookup"><span data-stu-id="c90e7-437">Added cmdlet to invoke an IoT Edge deployment metrics query.</span></span>
* <span data-ttu-id="c90e7-438">Foi adicionado um cmdlet para aplicar o conteúdo da configuração ao dispositivo edge especificado.</span><span class="sxs-lookup"><span data-stu-id="c90e7-438">Added cmdlet to apply the configuration content to the specified edge device.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c90e7-439">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c90e7-439">Az.KeyVault</span></span>
* <span data-ttu-id="c90e7-440">Foram removidos dois aliases: "New-AzKeyVaultCertificateAdministratorDetails" e "New-AzKeyVaultCertificateOrganizationDetails"</span><span class="sxs-lookup"><span data-stu-id="c90e7-440">Removed two aliases: 'New-AzKeyVaultCertificateAdministratorDetails' and 'New-AzKeyVaultCertificateOrganizationDetails'</span></span>
* <span data-ttu-id="c90e7-441">A eliminação recuperável foi ativada por predefinição ao criar um cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="c90e7-441">Enabled soft delete by default when creating a key vault</span></span>
* <span data-ttu-id="c90e7-442">Podem ser definidas regras de rede para governar a acessibilidade a partir de localizações na rede ao criar um cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="c90e7-442">Network rules can be set to govern the accessibility from specific network locations when creating a key vault</span></span>
* <span data-ttu-id="c90e7-443">Foi adicionado suporte para Bring Your Own Key (BYOK)</span><span class="sxs-lookup"><span data-stu-id="c90e7-443">Added support to bring your own key (BYOK)</span></span>
    - <span data-ttu-id="c90e7-444">"Add-AzKeyVaultKey" suporta a geração de chaves de intercâmbio de chaves</span><span class="sxs-lookup"><span data-stu-id="c90e7-444">'Add-AzKeyVaultKey' supports generating a key exchange key</span></span>
    - <span data-ttu-id="c90e7-445">"Get-AzKeyVaultKey" suporta a transferência de chaves públicas no formato PEM</span><span class="sxs-lookup"><span data-stu-id="c90e7-445">'Get-AzKeyVaultKey' supports downloading a public key in PEM format</span></span>
* <span data-ttu-id="c90e7-446">"KeyOps" foi atualizado como parte do documento de ajuda de "Add-AzKeyVaultKey"</span><span class="sxs-lookup"><span data-stu-id="c90e7-446">Updated the 'KeyOps' part of the help document of 'Add-AzKeyVaultKey'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c90e7-447">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-447">Az.Monitor</span></span>
* <span data-ttu-id="c90e7-448">Foi corrigido um erro em "Set-AzDiagnosticSettings"; a política de retenção não se aplicará a todas as categorias [#11589]</span><span class="sxs-lookup"><span data-stu-id="c90e7-448">Fixed bug for 'Set-AzDiagnosticSettings', retention policy won't apply to all categories [#11589]</span></span>
* <span data-ttu-id="c90e7-449">Suporte para critérios de disponibilidade de WebTest para alertas de métricas V2</span><span class="sxs-lookup"><span data-stu-id="c90e7-449">Supported WebTest availability criteria for metric alert V2</span></span>
    - <span data-ttu-id="c90e7-450">Novo "New-AzMetricAlertRuleV2Criteria": foi adicionada uma opção para criar critérios de disponibilidade WebTest</span><span class="sxs-lookup"><span data-stu-id="c90e7-450">'New-AzMetricAlertRuleV2Criteria': an option to create webtest availability criteria was added</span></span>
    - <span data-ttu-id="c90e7-451">"Add-AzMetricAlertRuleV2": suporta os novos critérios de disponibilidade de WebTest</span><span class="sxs-lookup"><span data-stu-id="c90e7-451">'Add-AzMetricAlertRuleV2': supports the new webtest availability criteria</span></span>
* <span data-ttu-id="c90e7-452">Foi removida a definição redundante de RetentionPolicy em PSLogProfile [#7608]</span><span class="sxs-lookup"><span data-stu-id="c90e7-452">Removed redundant definition for RetentionPolicy in PSLogProfile [#7608]</span></span>
* <span data-ttu-id="c90e7-453">Foram removidas as propriedades redundantes definidas em PSEventData [#11353]</span><span class="sxs-lookup"><span data-stu-id="c90e7-453">Removed redundant properties difined in PSEventData [#11353]</span></span>
* <span data-ttu-id="c90e7-454">O nome de "Get-AzLog" foi mudado para "Get-AzActivityLog"</span><span class="sxs-lookup"><span data-stu-id="c90e7-454">Renamed 'Get-AzLog' to 'Get-AzActivityLog'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-455">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-455">Az.Network</span></span>
* <span data-ttu-id="c90e7-456">Foi adicionado um atributo de alteração interruptiva para notificar que o comportamento predefinido da Zona vai ser alterado</span><span class="sxs-lookup"><span data-stu-id="c90e7-456">Added breaking change attribute to notify that Zone default behaviour will be changed</span></span>
    - <span data-ttu-id="c90e7-457">"New-AzPublicIpAddress"</span><span class="sxs-lookup"><span data-stu-id="c90e7-457">'New-AzPublicIpAddress'</span></span>
    - <span data-ttu-id="c90e7-458">"New-AzPublicIpPrefix"</span><span class="sxs-lookup"><span data-stu-id="c90e7-458">'New-AzPublicIpPrefix'</span></span>
    - <span data-ttu-id="c90e7-459">"New-AzLoadBalancerFrontendIpConfig"</span><span class="sxs-lookup"><span data-stu-id="c90e7-459">'New-AzLoadBalancerFrontendIpConfig'</span></span>
* <span data-ttu-id="c90e7-460">Foi adicionado suportado para um recurso de nível superior novo SecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="c90e7-460">Added support for a new top level resource SecurityPartnerProvider</span></span>
    - <span data-ttu-id="c90e7-461">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c90e7-461">New cmdlets added:</span></span>
        - <span data-ttu-id="c90e7-462">New-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="c90e7-462">New-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="c90e7-463">Remove-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="c90e7-463">Remove-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="c90e7-464">Get-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="c90e7-464">Get-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="c90e7-465">Set-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="c90e7-465">Set-AzSecurityPartnerProvider</span></span>
* <span data-ttu-id="c90e7-466">Foi adicionado "RequiredZoneNames" em "PSPrivateLinkResource" e "GroupId" em "PSPrivateEndpointConnection”</span><span class="sxs-lookup"><span data-stu-id="c90e7-466">Added 'RequiredZoneNames' on 'PSPrivateLinkResource' and 'GroupId' on 'PSPrivateEndpointConnection'</span></span>
* <span data-ttu-id="c90e7-467">Foi corrigido o tipo incorreto do parâmetro SuccessThresholdRoundTripTimeMs para New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span><span class="sxs-lookup"><span data-stu-id="c90e7-467">Fixed incorrect type of SuccessThresholdRoundTripTimeMs parameter for New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span></span>
* <span data-ttu-id="c90e7-468">Foram atualizados os cmdlets VirtualWan para definir o valor predefinido do argumento AllowVnetToVnetTraffic como Verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="c90e7-468">Updated VirtualWan cmdlets to set default value of AllowVnetToVnetTraffic argument to True.</span></span>
    - <span data-ttu-id="c90e7-469">"New-AzVirtualWan"</span><span class="sxs-lookup"><span data-stu-id="c90e7-469">'New-AzVirtualWan'</span></span>
    - <span data-ttu-id="c90e7-470">"Update-AzVirtualWan"</span><span class="sxs-lookup"><span data-stu-id="c90e7-470">'Update-AzVirtualWan'</span></span>
* <span data-ttu-id="c90e7-471">Foram adicionados cmdlets para suportar o grupo de zonas DNS para pontos finais privados</span><span class="sxs-lookup"><span data-stu-id="c90e7-471">Added new cmdlets to support DNS zone group for private endpoint</span></span>
    - <span data-ttu-id="c90e7-472">"New-AzPrivateDnsZoneConfig"</span><span class="sxs-lookup"><span data-stu-id="c90e7-472">'New-AzPrivateDnsZoneConfig'</span></span>
    - <span data-ttu-id="c90e7-473">"Get-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="c90e7-473">'Get-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="c90e7-474">"New-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="c90e7-474">'New-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="c90e7-475">"Set-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="c90e7-475">'Set-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="c90e7-476">"Remove-AzPrivateDnsZoneGroup"</span><span class="sxs-lookup"><span data-stu-id="c90e7-476">'Remove-AzPrivateDnsZoneGroup'</span></span>
* <span data-ttu-id="c90e7-477">Foram adicionados os parâmetros "DNSEnableProxy", "DNSRequireProxyForNetworkRules" e "DNSServers" a "AzureFirewall"</span><span class="sxs-lookup"><span data-stu-id="c90e7-477">Added 'DNSEnableProxy', 'DNSRequireProxyForNetworkRules' and 'DNSServers' parameters to 'AzureFirewall'</span></span>
* <span data-ttu-id="c90e7-478">Foram adicionados os parâmetros "EnableDnsProxy", "DnsProxyNotRequiredForNetworkRule" e "DnsServer" a "AzureFirewall"</span><span class="sxs-lookup"><span data-stu-id="c90e7-478">Added 'EnableDnsProxy', 'DnsProxyNotRequiredForNetworkRule' and 'DnsServer' parameters to 'AzureFirewall'</span></span>
    - <span data-ttu-id="c90e7-479">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="c90e7-479">Updated cmdlet:</span></span>
        - <span data-ttu-id="c90e7-480">New-AzFirewall</span><span class="sxs-lookup"><span data-stu-id="c90e7-480">New-AzFirewall</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c90e7-481">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-481">Az.OperationalInsights</span></span>
* <span data-ttu-id="c90e7-482">O código legado foi atualizado para aplicar o SDK recém-gerado</span><span class="sxs-lookup"><span data-stu-id="c90e7-482">Updated legacy code to apply new generated SDK</span></span>
* <span data-ttu-id="c90e7-483">Foram eliminados cmdlets devido a APIs preteridas</span><span class="sxs-lookup"><span data-stu-id="c90e7-483">Deleted cmdlets due to deprecated APIs</span></span>
    - <span data-ttu-id="c90e7-484">"Get-AzOperationalInsightsSavedSearchResult" (alias "Get-AzOperationalInsightsSavedSearchResults")</span><span class="sxs-lookup"><span data-stu-id="c90e7-484">'Get-AzOperationalInsightsSavedSearchResult' (alias 'Get-AzOperationalInsightsSavedSearchResults')</span></span>
    - <span data-ttu-id="c90e7-485">"Get-AzOperationalInsightsSearchResult" (alias "Get-AzOperationalInsightsSearchResults")</span><span class="sxs-lookup"><span data-stu-id="c90e7-485">'Get-AzOperationalInsightsSearchResult' (alias 'Get-AzOperationalInsightsSearchResults')</span></span>
    - <span data-ttu-id="c90e7-486">"Get-AzOperationalInsightsLinkTarget" (alias "Get-AzOperationalInsightsLinkTargets")</span><span class="sxs-lookup"><span data-stu-id="c90e7-486">'Get-AzOperationalInsightsLinkTarget' (alias 'Get-AzOperationalInsightsLinkTargets')</span></span>
* <span data-ttu-id="c90e7-487">Foram adicionados parâmetros para "Set-AzOperationalInsightsWorkspace" e "New-AzOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="c90e7-487">Added parameters for 'Set-AzOperationalInsightsWorkspace' and 'New-AzOperationalInsightsWorkspace'</span></span>
* <span data-ttu-id="c90e7-488">Foram criados cmdlets para a Conta de Armazenamento Associada</span><span class="sxs-lookup"><span data-stu-id="c90e7-488">Created cmdlets for Linked Stoarge Account</span></span>
* <span data-ttu-id="c90e7-489">Foram criados cmdlets para Clusters e para o Serviço Associado</span><span class="sxs-lookup"><span data-stu-id="c90e7-489">Created cmdlets for Clusters and Linked Service</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-490">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-490">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-491">O Azure Site Recovery adicionou suporte para proteger máquinas virtuais de grupo de colocação por proximidade para fornecedor do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-491">Azure Site Recovery added support for protecting proximity placement group virtual machines for Azure to Azure provider.</span></span>
* <span data-ttu-id="c90e7-492">O Azure Site Recovery adicionou suporte para a replicação de zona para zona.</span><span class="sxs-lookup"><span data-stu-id="c90e7-492">Azure Site Recovery added support for zone to zone replication.</span></span>
* <span data-ttu-id="c90e7-493">O Azure Backup adicionou suporte para a retenção de longo prazo para Pontos de Recuperação de Partilhas de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-493">Azure Backup Added Long term retention support for Azure FileShare Recovery Points.</span></span>
* <span data-ttu-id="c90e7-494">O Azure Backup adicionou propriedades de exclusão de discos à saída do cmdlet "Get-AzRecoveryServicesBackupItem".</span><span class="sxs-lookup"><span data-stu-id="c90e7-494">Azure Backup Added disk exclusion properties to 'Get-AzRecoveryServicesBackupItem' cmdlet output.</span></span>
* <span data-ttu-id="c90e7-495">Foi adicionado o ponto final privado para o ficheiro de credenciais de Cofre para o Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="c90e7-495">Added private endpoint for Vault credential file for site recovery service.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-496">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-496">Az.Resources</span></span>
* <span data-ttu-id="c90e7-497">Foi adicionado um aviso de mensagem relativo a um atraso na vista ao criar uma Definição de Função nova</span><span class="sxs-lookup"><span data-stu-id="c90e7-497">Added message warning about view delay when creating a new Role Definition</span></span>
* <span data-ttu-id="c90e7-498">Os cmdlets de política foram alterados para produzir objetos de tipos compatíveis</span><span class="sxs-lookup"><span data-stu-id="c90e7-498">Changed policy cmdlets to output strongly-typed objects</span></span>
* <span data-ttu-id="c90e7-499">Foi removido o parâmetro "-TenantLevel" utilizado no cmdlet "Get-AzResourceLock" [#11335]</span><span class="sxs-lookup"><span data-stu-id="c90e7-499">Removed '-TenantLevel' parameter used for on the 'Get-AzResourceLock' cmdlet [#11335]</span></span>
* <span data-ttu-id="c90e7-500">"Remove-AzResourceGroup -Id ResourceId" foi corrigido [#9882]</span><span class="sxs-lookup"><span data-stu-id="c90e7-500">Fixed 'Remove-AzResourceGroup -Id ResourceId'[#9882]</span></span>
* <span data-ttu-id="c90e7-501">Foi adicionado um cmdlet novo para obter resultados de What-If de modelos do ARM no âmbito de um grupo de recursos: "Get-AzDeploymentResourceGroupWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="c90e7-501">Added new cmdlet for getting ARM template What-If results at resource group scope: 'Get-AzDeploymentResourceGroupWhatIfResult'</span></span>
* <span data-ttu-id="c90e7-502">Foi adicionado um cmdlet novo para obter resultados de What-If de modelos do ARM no âmbito de uma subscrição: "Get-AzDeploymentWhatIfResult"</span><span class="sxs-lookup"><span data-stu-id="c90e7-502">Added new cmdlet for getting ARM template What-If results at subscription scope: 'Get-AzDeploymentWhatIfResult'</span></span>
   - <span data-ttu-id="c90e7-503">Alias: "Get-AzSubscriptionDeploymentWhatIf"</span><span class="sxs-lookup"><span data-stu-id="c90e7-503">Alias: 'Get-AzSubscriptionDeploymentWhatIf'</span></span>
* <span data-ttu-id="c90e7-504">Os parâmetros "-WhatIf" e "-Confirm" foram substituídos para "New-AzDeployment" e "New-AzResourceGroupDeployment" para utilizar resultados de What-If de modelos do ARM</span><span class="sxs-lookup"><span data-stu-id="c90e7-504">Overrode '-WhatIf' and '-Confirm' parameters for 'New-AzDeployment' and 'New-AzResourceGroupDeployment' to use ARM template What-If results</span></span>
* <span data-ttu-id="c90e7-505">Foi adicionada a mensagem de descontinuação para o parâmetro "ApiVersion" em cmdlets implementados</span><span class="sxs-lookup"><span data-stu-id="c90e7-505">Added deprecation message for 'ApiVersion' parameter in deployment cmdlets</span></span>
* <span data-ttu-id="c90e7-506">Foi adicionada a capacidade para mostrar mensagens de erro melhoradas relativas a falhas em implementações</span><span class="sxs-lookup"><span data-stu-id="c90e7-506">Added capability to show improved error messages for deployment failures</span></span>
* <span data-ttu-id="c90e7-507">Foi adicionado o registo de correlationId para falhas em implementações</span><span class="sxs-lookup"><span data-stu-id="c90e7-507">Added correlationId logging for deployment failures</span></span>
* <span data-ttu-id="c90e7-508">Foi adicionada a propriedade "error" à saída do script de implementação</span><span class="sxs-lookup"><span data-stu-id="c90e7-508">Added 'error' property to the deployment script output</span></span>
* <span data-ttu-id="c90e7-509">O nuget Microsoft.Azure.Management.ResourceManager foi atualizado para "3.7.1-preview"</span><span class="sxs-lookup"><span data-stu-id="c90e7-509">Updated nuget Microsoft.Azure.Management.ResourceManager to '3.7.1-preview'</span></span>
* <span data-ttu-id="c90e7-510">Foram removidos casos de teste específicos, uma vez que a propriedade Error em DeploymentValidateResult foi alterada para apenas de leitura a partir de 3.7.1-preview</span><span class="sxs-lookup"><span data-stu-id="c90e7-510">Removed specific test cases as Error property in DeploymentValidateResult has changed to readonly from nuget 3.7.1-preview</span></span>
* <span data-ttu-id="c90e7-511">GenericResourceExpanded foi importado do SDK ResourceManager 3.7.1-preview</span><span class="sxs-lookup"><span data-stu-id="c90e7-511">Brought GenericResourceExpanded from SDK ResourceManager 3.7.1-preview</span></span>
* <span data-ttu-id="c90e7-512">Foi adicionado suporte para etiquetas a todos os cmdlets Get para implementação, bem como</span><span class="sxs-lookup"><span data-stu-id="c90e7-512">Added tag support for all Get cmdlets for deployment, as well as</span></span>
    - <span data-ttu-id="c90e7-513">"New-AzDeployment"</span><span class="sxs-lookup"><span data-stu-id="c90e7-513">'New-AzDeployment'</span></span>
    - <span data-ttu-id="c90e7-514">"New-AzManagementGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="c90e7-514">'New-AzManagementGroupDeployment'</span></span>
    - <span data-ttu-id="c90e7-515">"New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="c90e7-515">'New-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="c90e7-516">"New-AzTenantDeployment"</span><span class="sxs-lookup"><span data-stu-id="c90e7-516">'New-AzTenantDeployment'</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c90e7-517">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c90e7-517">Az.ServiceFabric</span></span>
* <span data-ttu-id="c90e7-518">Foi corrigido um erro na adição de certificados mediante a utilização de --SecretIdentifier que obtinha o thumbprint de certificado incorreto</span><span class="sxs-lookup"><span data-stu-id="c90e7-518">Fixed bug in add certificate using --SecretIdentifier that was getting the wrong certificate thumbprint</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-519">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-519">Az.Sql</span></span>
* <span data-ttu-id="c90e7-520">Foi melhorado o desempenho de:</span><span class="sxs-lookup"><span data-stu-id="c90e7-520">Enhance performance of:</span></span>
    - <span data-ttu-id="c90e7-521">"Set-AzSqlDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="c90e7-521">'Set-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="c90e7-522">"Set-AzSqlInstanceDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="c90e7-522">'Set-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="c90e7-523">"Remove-AzSqlDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="c90e7-523">'Remove-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="c90e7-524">"Remove-AzSqlInstanceDatabaseSensitivityClassification"</span><span class="sxs-lookup"><span data-stu-id="c90e7-524">'Remove-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="c90e7-525">"Enable-AzSqlDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="c90e7-525">'Enable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="c90e7-526">"Enable-AzSqlInstanceDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="c90e7-526">'Enable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="c90e7-527">"Disable-AzSqlDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="c90e7-527">'Disable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="c90e7-528">"Disable-AzSqlInstanceDatabaseSensitivityRecommendation"</span><span class="sxs-lookup"><span data-stu-id="c90e7-528">'Disable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
* <span data-ttu-id="c90e7-529">Foi removida a validação do lado do cliente do parâmetro "RetentionDays" do cmdlet "Set-AzSqlDatabaseBackupShortTermRetentionPolicy"</span><span class="sxs-lookup"><span data-stu-id="c90e7-529">Removed client-side validation of 'RetentionDays' parameter from cmdlet 'Set-AzSqlDatabaseBackupShortTermRetentionPolicy'</span></span>
* <span data-ttu-id="c90e7-530">Auditoria a uma conta de armazenamento na Vnet; corrigido um erro ao criar uma função de Contribuidor de Dados de Blobs de Armazenamento.</span><span class="sxs-lookup"><span data-stu-id="c90e7-530">Auditing to a storage account in Vnet, fixing a bug when creating a Storage Blob Data Contributor role.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-531">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-531">Az.Storage</span></span>
* <span data-ttu-id="c90e7-532">Foi adicionado "-AsJob" ao cmdlet para obter/listar contas "Get-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c90e7-532">Added '-AsJob' to get/list account cmdlet 'Get-AzStorageAccount'</span></span>
* <span data-ttu-id="c90e7-533">KeyVersion foi tornado opcional ao atualizar a conta de Armazenamento com KeyvaultEncryption, para suportar a rotação automática de chaves</span><span class="sxs-lookup"><span data-stu-id="c90e7-533">Make KeyVersion to optional when update Storage account with KeyvaultEncryption, to support key auto-rotation</span></span>
    - <span data-ttu-id="c90e7-534">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c90e7-534">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="c90e7-535">Corrigida a remoção de falha do Diretório de Ficheiros do Azure com o pipeline</span><span class="sxs-lookup"><span data-stu-id="c90e7-535">Fixed remove Azure File Directory fail with pipeline</span></span>
    - <span data-ttu-id="c90e7-536">"Remove-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="c90e7-536">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="c90e7-537">Corrigido [#9880]: A definição do valor DefaultAction de NetWorkRule foi alterado para estar alinhado com o swagger.</span><span class="sxs-lookup"><span data-stu-id="c90e7-537">Fixed [#9880]: Change NetWorkRule DefaultAction value defination to align with swagger.</span></span>
    - <span data-ttu-id="c90e7-538">"Update-AzStorageAccountNetworkRuleSet"</span><span class="sxs-lookup"><span data-stu-id="c90e7-538">'Update-AzStorageAccountNetworkRuleSet'</span></span>
    - <span data-ttu-id="c90e7-539">"Get-AzStorageAccountNetworkRuleSet"</span><span class="sxs-lookup"><span data-stu-id="c90e7-539">'Get-AzStorageAccountNetworkRuleSet'</span></span>
* <span data-ttu-id="c90e7-540">Corrigido [#11624]: Ignorar regras duplicadas ao adicionar NetworkRules, para evitar falhas de servidores</span><span class="sxs-lookup"><span data-stu-id="c90e7-540">Fixed [#11624]: Skip duplicated rules when add NetworkRules, to avoid server failure</span></span>
    - <span data-ttu-id="c90e7-541">"Add-AzStorageAccountNetworkRule"</span><span class="sxs-lookup"><span data-stu-id="c90e7-541">'Add-AzStorageAccountNetworkRule'</span></span>
* <span data-ttu-id="c90e7-542">O SDK Microsoft.Azure.Cosmos.Table foi atualizado para 1.0.7</span><span class="sxs-lookup"><span data-stu-id="c90e7-542">Upgraded Microsoft.Azure.Cosmos.Table SDK to 1.0.7</span></span>
* <span data-ttu-id="c90e7-543">Foi adicionada uma mensagem de aviso para relembrar o utilizador para listar novamente com ContinuationToken apenas quando são devolvidos itens de peças na lista DataLake Gen2 Items,</span><span class="sxs-lookup"><span data-stu-id="c90e7-543">Added a warning message to remind user to list again with ContinuationToken when only part items are returned in list DataLake Gen2 Items,</span></span>
    - <span data-ttu-id="c90e7-544">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="c90e7-544">'Get-AzDataLakeGen2ChildItem'</span></span>
* <span data-ttu-id="c90e7-545">Suportado para criar ou atualizar a conta de Armazenamento com a Autenticação do Active Directory Domain Service dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-545">Supported to create or update Storage account with Azure Files Active Directory Domain Service Authentication</span></span>
    -  <span data-ttu-id="c90e7-546">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c90e7-546">'New-AzStorageAccount'</span></span>
    -  <span data-ttu-id="c90e7-547">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c90e7-547">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="c90e7-548">Suportado para os comandos "new" ou "list" de chaves de Kerberos da conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="c90e7-548">Supported to new or list Kerberos keys of Storage account</span></span>
    -  <span data-ttu-id="c90e7-549">"New-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="c90e7-549">'New-AzStorageAccountKey'</span></span>
    -  <span data-ttu-id="c90e7-550">"Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="c90e7-550">'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="c90e7-551">Suportada conta de Armazenamento de ativação pós-falha</span><span class="sxs-lookup"><span data-stu-id="c90e7-551">Supported failover Storage account</span></span>
    - <span data-ttu-id="c90e7-552">"Invoke-AzStorageAccountFailover"</span><span class="sxs-lookup"><span data-stu-id="c90e7-552">'Invoke-AzStorageAccountFailover'</span></span>
* <span data-ttu-id="c90e7-553">Ajuda de "Get-AzStorageBlobCopyState" atualizada</span><span class="sxs-lookup"><span data-stu-id="c90e7-553">Updated help of 'Get-AzStorageBlobCopyState'</span></span>
* <span data-ttu-id="c90e7-554">Ajuda de "Get-AzStorageFileCopyState" e "Start-AzStorageBlobCopy" atualizada</span><span class="sxs-lookup"><span data-stu-id="c90e7-554">Updated help of 'Get-AzStorageFileCopyState' and 'Start-AzStorageBlobCopy'</span></span>
* <span data-ttu-id="c90e7-555">Integração da biblioteca de cliente do Armazenamento v12 para cmdlets de Filas e Ficheiros</span><span class="sxs-lookup"><span data-stu-id="c90e7-555">Integrated Storage client library v12 to Queue and File cmdlets</span></span>
* <span data-ttu-id="c90e7-556">Alteração ao tipo de saída de CloudFile para AzureStorageFile; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="c90e7-556">Changed output type from CloudFile to AzureStorageFile, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="c90e7-557">"Get-AzStorageFile"</span><span class="sxs-lookup"><span data-stu-id="c90e7-557">'Get-AzStorageFile'</span></span>
    - <span data-ttu-id="c90e7-558">"Remove-AzStorageFile"</span><span class="sxs-lookup"><span data-stu-id="c90e7-558">'Remove-AzStorageFile'</span></span>
    - <span data-ttu-id="c90e7-559">"Get-AzStorageFileContent"</span><span class="sxs-lookup"><span data-stu-id="c90e7-559">'Get-AzStorageFileContent'</span></span>
    - <span data-ttu-id="c90e7-560">"Set-AzStorageFileContent"</span><span class="sxs-lookup"><span data-stu-id="c90e7-560">'Set-AzStorageFileContent'</span></span>
    - <span data-ttu-id="c90e7-561">"Start-AzStorageFileCopy"</span><span class="sxs-lookup"><span data-stu-id="c90e7-561">'Start-AzStorageFileCopy'</span></span>
* <span data-ttu-id="c90e7-562">Alteração ao tipo de saída de CloudFileDirectory para AzureStorageFileDirectory; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="c90e7-562">Changed output type from CloudFileDirectory to AzureStorageFileDirectory, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="c90e7-563">"New-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="c90e7-563">'New-AzStorageDirectory'</span></span>
    - <span data-ttu-id="c90e7-564">"Remove-AzStorageDirectory"</span><span class="sxs-lookup"><span data-stu-id="c90e7-564">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="c90e7-565">Alteração ao tipo de saída de CloudFileShare para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="c90e7-565">Changed output type from CloudFileShare to AzureStorageFileShare, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="c90e7-566">"Get-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="c90e7-566">'Get-AzStorageShare'</span></span>
    - <span data-ttu-id="c90e7-567">"New-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="c90e7-567">'New-AzStorageShare'</span></span>
    - <span data-ttu-id="c90e7-568">"Remove-AzStorageShare"</span><span class="sxs-lookup"><span data-stu-id="c90e7-568">'Remove-AzStorageShare'</span></span>
* <span data-ttu-id="c90e7-569">Alteração ao tipo de saída de FileShareProperties para AzureStorageFileShare; a saída original tornar-se-á na propriedade subordinada da saída nova</span><span class="sxs-lookup"><span data-stu-id="c90e7-569">Changed output type from FileShareProperties to AzureStorageFileShare, the original output will become a sub child property of the new output</span></span>
    - <span data-ttu-id="c90e7-570">"Set-AzStorageShareQuota"</span><span class="sxs-lookup"><span data-stu-id="c90e7-570">'Set-AzStorageShareQuota'</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="c90e7-571">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c90e7-571">Az.TrafficManager</span></span>
* <span data-ttu-id="c90e7-572">Corrigido o nome de perfil errado na saída verbosa de "DisableAzureTrafficManagerEndpoint"</span><span class="sxs-lookup"><span data-stu-id="c90e7-572">Fixed incorrect profile name in 'DisableAzureTrafficManagerEndpoint' verbose output</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-573">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-573">Az.Websites</span></span>
* <span data-ttu-id="c90e7-574">Corrigido um erro ortográfico na ajuda de "Update-AzWebAppAccessRestrictionConfig".</span><span class="sxs-lookup"><span data-stu-id="c90e7-574">Fixed typo on help of 'Update-AzWebAppAccessRestrictionConfig'.</span></span>

## <a name="380---april-2020"></a><span data-ttu-id="c90e7-575">3.8.0 - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="c90e7-575">3.8.0 - April 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="c90e7-576">Destaques desde a última versão</span><span class="sxs-lookup"><span data-stu-id="c90e7-576">Highlights since the last release</span></span>
* <span data-ttu-id="c90e7-577">Versões do Powershell suportadas pelo Az.Storage: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="c90e7-577">PowerShell versions that Az.Storage supports: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c90e7-578">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-578">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-579">Atualização do URL de inquérito do Azure PowerShell em "Resolve-AzError" [#11507]</span><span class="sxs-lookup"><span data-stu-id="c90e7-579">Updated Azure PowerShell survey URL in 'Resolve-AzError' [#11507]</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c90e7-580">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c90e7-580">Az.ApiManagement</span></span>
* <span data-ttu-id="c90e7-581">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="c90e7-581">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="c90e7-582">Documentação atualizada de "Set-AzApiManagementGroup" para especificar o parâmetro GroupId</span><span class="sxs-lookup"><span data-stu-id="c90e7-582">'Set-AzApiManagementGroup' Updated documentation to specify the GroupId parameter</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c90e7-583">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c90e7-583">Az.Cdn</span></span>
* <span data-ttu-id="c90e7-584">Correção da apresentação do SKU de preços relacionados com ChinaCDN</span><span class="sxs-lookup"><span data-stu-id="c90e7-584">Fixed ChinaCDN related pricing SKU display</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c90e7-585">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-585">Az.CognitiveServices</span></span>
* <span data-ttu-id="c90e7-586">Suporte para Identidade, Encriptação, UserOwnedStorage</span><span class="sxs-lookup"><span data-stu-id="c90e7-586">Supported Identity, Encryption, UserOwnedStorage</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-587">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-587">Az.Compute</span></span>
* <span data-ttu-id="c90e7-588">Adicionado o cmdlet "Set-AzVmssOrchestrationServiceState".</span><span class="sxs-lookup"><span data-stu-id="c90e7-588">Added 'Set-AzVmssOrchestrationServiceState' cmdlet.</span></span>
* <span data-ttu-id="c90e7-589">"Get-AzVmss" com -InstanceView mostra os estados de OrchestrationService.</span><span class="sxs-lookup"><span data-stu-id="c90e7-589">'Get-AzVmss' with -InstanceView shows OrchestrationService states.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c90e7-590">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-590">Az.IotHub</span></span>
* <span data-ttu-id="c90e7-591">Gestão da configuração do dispositivo duplo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c90e7-591">Manage IoT device twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="c90e7-592">"Get-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="c90e7-592">'Get-AzIotHubDeviceTwin'</span></span>
    - <span data-ttu-id="c90e7-593">"Update-AzIotHubDeviceTwin"</span><span class="sxs-lookup"><span data-stu-id="c90e7-593">'Update-AzIotHubDeviceTwin'</span></span>
* <span data-ttu-id="c90e7-594">Adicionado cmdlet para invocar o método direto num dispositivo num hub IoT.</span><span class="sxs-lookup"><span data-stu-id="c90e7-594">Added cmdlet to invoke direct method on a device in an Iot Hub.</span></span>
* <span data-ttu-id="c90e7-595">Gestão da configuração do módulo duplo do dispositivo de IoT. Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c90e7-595">Manage IoT device module twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="c90e7-596">"Get-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="c90e7-596">'Get-AzIotHubModuleTwin'</span></span>
    - <span data-ttu-id="c90e7-597">"Update-AzIotHubModuleTwin"</span><span class="sxs-lookup"><span data-stu-id="c90e7-597">'Update-AzIotHubModuleTwin'</span></span>
* <span data-ttu-id="c90e7-598">Gestão da configuração da gestão automática de dispositivos IoT em escala.</span><span class="sxs-lookup"><span data-stu-id="c90e7-598">Manage IoT automatic device management configuration at scale.</span></span> <span data-ttu-id="c90e7-599">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c90e7-599">New cmdlets are:</span></span>
    - <span data-ttu-id="c90e7-600">"Add-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c90e7-600">'Add-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="c90e7-601">"Get-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c90e7-601">'Get-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="c90e7-602">"Remove-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c90e7-602">'Remove-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="c90e7-603">"Set-AzIotHubConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c90e7-603">'Set-AzIotHubConfiguration'</span></span>
* <span data-ttu-id="c90e7-604">Adicionado cmdlet para invocar um método de módulo de periferia num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="c90e7-604">Added cmdlet to invoke an edge module method in an Iot Hub.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c90e7-605">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c90e7-605">Az.KeyVault</span></span>
* <span data-ttu-id="c90e7-606">Adicionado um novo cmdlet "Update-AzKeyVault" que pode permitir a eliminação recuperável e a proteção contra remoções num cofre</span><span class="sxs-lookup"><span data-stu-id="c90e7-606">Added a new cmdlet 'Update-AzKeyVault' that can enable soft delete and purge protection on a vault</span></span>
* <span data-ttu-id="c90e7-607">Adicionado suporte para Microsoft.PowerShell.SecretManagement [#11178]</span><span class="sxs-lookup"><span data-stu-id="c90e7-607">Added support to Microsoft.PowerShell.SecretManagement [#11178]</span></span>
* <span data-ttu-id="c90e7-608">Correção do erro nos exemplos de "Remove-AzKeyVaultManagedStorageSasDefinition" [#11479]</span><span class="sxs-lookup"><span data-stu-id="c90e7-608">Fixed error in the examples of 'Remove-AzKeyVaultManagedStorageSasDefinition' [#11479]</span></span>
* <span data-ttu-id="c90e7-609">Adicionado suporte para o ponto final privado</span><span class="sxs-lookup"><span data-stu-id="c90e7-609">Added support to private endpoint</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="c90e7-610">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="c90e7-610">Az.Maintenance</span></span>
* <span data-ttu-id="c90e7-611">Publicação da versão de lançamento dos cmdlets de Manutenção para Disponibilidade Geral</span><span class="sxs-lookup"><span data-stu-id="c90e7-611">Publishing release version of Maintenance cmdlets for GA</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c90e7-612">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-612">Az.Monitor</span></span>
* <span data-ttu-id="c90e7-613">Adicionados cmdlets para o âmbito de ligação privada</span><span class="sxs-lookup"><span data-stu-id="c90e7-613">Added cmdlets for private link scope</span></span>
    - <span data-ttu-id="c90e7-614">"Get-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="c90e7-614">'Get-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="c90e7-615">"Remove-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="c90e7-615">'Remove-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="c90e7-616">"New-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="c90e7-616">'New-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="c90e7-617">"Update-AzInsightsPrivateLinkScope"</span><span class="sxs-lookup"><span data-stu-id="c90e7-617">'Update-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="c90e7-618">"Get-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="c90e7-618">'Get-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="c90e7-619">"New-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="c90e7-619">'New-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="c90e7-620">"Remove-AzInsightsPrivateLinkScopedResource"</span><span class="sxs-lookup"><span data-stu-id="c90e7-620">'Remove-AzInsightsPrivateLinkScopedResource'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-621">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-621">Az.Network</span></span>
* <span data-ttu-id="c90e7-622">Atualização dos cmdlets para permitir a ligação num IP privado para o Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="c90e7-622">Updated cmdlets to enable connection on private IP for Virtual Network Gateway.</span></span>
    - <span data-ttu-id="c90e7-623">"New-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="c90e7-623">'New-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="c90e7-624">"Set-AzVirtualNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="c90e7-624">'Set-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="c90e7-625">"New-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="c90e7-625">'New-AzVirtualNetworkGatewayConnection'</span></span>
    - <span data-ttu-id="c90e7-626">"Set-AzVirtualNetworkGatewayConnection"</span><span class="sxs-lookup"><span data-stu-id="c90e7-626">'Set-AzVirtualNetworkGatewayConnection'</span></span>
* <span data-ttu-id="c90e7-627">Atualização dos cmdlets para permitir LocalNetworkGateways e VpnSites com base em FQDN</span><span class="sxs-lookup"><span data-stu-id="c90e7-627">Updated cmdlets to enable FQDN based LocalNetworkGateways and VpnSites</span></span>
    - <span data-ttu-id="c90e7-628">"New-AzLocalNetworkGateway"</span><span class="sxs-lookup"><span data-stu-id="c90e7-628">'New-AzLocalNetworkGateway'</span></span>
    - <span data-ttu-id="c90e7-629">"New-AzVpnSiteLink"</span><span class="sxs-lookup"><span data-stu-id="c90e7-629">'New-AzVpnSiteLink'</span></span>
* <span data-ttu-id="c90e7-630">Adicionado suporte para a família de endereços IPv6 em ExpressRouteCircuitConnectionConfig (Alcance Global)</span><span class="sxs-lookup"><span data-stu-id="c90e7-630">Added support for IPv6 address family in ExpressRouteCircuitConnectionConfig (Global Reach)</span></span>
    - <span data-ttu-id="c90e7-631">Adicionado "Set-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="c90e7-631">Added 'Set-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="c90e7-632">permite a definição de todas as propriedades existentes, incluindo o IPv6CircuitConnectionProperties</span><span class="sxs-lookup"><span data-stu-id="c90e7-632">allows setting of all the existing properties including the IPv6CircuitConnectionProperties</span></span>
    - <span data-ttu-id="c90e7-633">Atualização de "Add-AzExpressRouteCircuitConnectionConfig"</span><span class="sxs-lookup"><span data-stu-id="c90e7-633">Updated 'Add-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="c90e7-634">Adicionado outro parâmetro opcional AddressPrefixType para especificar a família de endereços do prefixo de endereço</span><span class="sxs-lookup"><span data-stu-id="c90e7-634">Added another optional parameter AddressPrefixType to specify the address family of address prefix</span></span>
* <span data-ttu-id="c90e7-635">Atualização dos cmdlets para permitir a definição do Tempo Limite de DPD nas Ligações do Gateway de Rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="c90e7-635">Updated cmdlets to enable setting of DPD Timeout on Virtual Network Gateway Connections.</span></span>
    - <span data-ttu-id="c90e7-636">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-636">New-AzVirtualNetworkGatewayConnection</span></span>
    - <span data-ttu-id="c90e7-637">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-637">Set-AzVirtualNetworkGatewayConnection</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c90e7-638">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-638">Az.PolicyInsights</span></span>
* <span data-ttu-id="c90e7-639">Adicionado o cmdlet "Start-AzPolicyComplianceScan" para acionar análises de conformidade de políticas</span><span class="sxs-lookup"><span data-stu-id="c90e7-639">Added 'Start-AzPolicyComplianceScan' cmdlet for triggering policy compliance scans</span></span>
* <span data-ttu-id="c90e7-640">Adição de definição de políticas, definição de conjuntos e versões de atribuição ao resultado de "Get-AzPolicyState"</span><span class="sxs-lookup"><span data-stu-id="c90e7-640">Added policy definition, set definition, and assignment versions to 'Get-AzPolicyState' output</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c90e7-641">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c90e7-641">Az.ServiceFabric</span></span>
* <span data-ttu-id="c90e7-642">Melhorias da formatação e usabilidade do código dos exemplos de "New-AzServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="c90e7-642">Improved code formatting and usability of 'New-AzServiceFabricCluster' examples</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-643">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-643">Az.Sql</span></span>
* <span data-ttu-id="c90e7-644">Adicionados os cmdlets "Get-AzSqlInstanceOperation" e "Stop-AzSqlInstanceOperation"</span><span class="sxs-lookup"><span data-stu-id="c90e7-644">Added cmdlets 'Get-AzSqlInstanceOperation' and 'Stop-AzSqlInstanceOperation'</span></span>
* <span data-ttu-id="c90e7-645">Suporte de auditorias a uma conta de armazenamento numa VNet.</span><span class="sxs-lookup"><span data-stu-id="c90e7-645">Supported auditing to a storage account in VNet.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-646">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-646">Az.Storage</span></span>
* <span data-ttu-id="c90e7-647">Adicionado aviso de alteração interruptiva para a alteração de resultados de cmdlets de Ficheiro do Azure numa versão futura</span><span class="sxs-lookup"><span data-stu-id="c90e7-647">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="c90e7-648">Suportado novo SkuName StandardGZRS, StandardRAGZRS ao criar/atualizar a Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="c90e7-648">Supported new SkuName StandardGZRS, StandardRAGZRS when create/update Storage account</span></span>
    - <span data-ttu-id="c90e7-649">"New-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c90e7-649">'New-AzStorageAccount'</span></span>
    - <span data-ttu-id="c90e7-650">"Set-AzStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c90e7-650">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="c90e7-651">Suportado o DataLake Gen2</span><span class="sxs-lookup"><span data-stu-id="c90e7-651">Supported DataLake Gen2</span></span>
    - <span data-ttu-id="c90e7-652">"New-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="c90e7-652">'New-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="c90e7-653">"Get-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="c90e7-653">'Get-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="c90e7-654">"Get-AzDataLakeGen2ChildItem"</span><span class="sxs-lookup"><span data-stu-id="c90e7-654">'Get-AzDataLakeGen2ChildItem'</span></span>
    - <span data-ttu-id="c90e7-655">"Move-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="c90e7-655">'Move-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="c90e7-656">"Set-AzDataLakeGen2ItemAclObject"</span><span class="sxs-lookup"><span data-stu-id="c90e7-656">'Set-AzDataLakeGen2ItemAclObject'</span></span>
    - <span data-ttu-id="c90e7-657">"Update-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="c90e7-657">'Update-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="c90e7-658">"Get-AzDataLakeGen2ItemContent"</span><span class="sxs-lookup"><span data-stu-id="c90e7-658">'Get-AzDataLakeGen2ItemContent'</span></span>
    - <span data-ttu-id="c90e7-659">"Remove-AzDataLakeGen2Item"</span><span class="sxs-lookup"><span data-stu-id="c90e7-659">'Remove-AzDataLakeGen2Item'</span></span>

## <a name="0100-preview---april-2020"></a><span data-ttu-id="c90e7-660">0.10.0-preview - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="c90e7-660">0.10.0-preview - April 2020</span></span>
### <a name="general"></a><span data-ttu-id="c90e7-661">Geral</span><span class="sxs-lookup"><span data-stu-id="c90e7-661">General</span></span>
* <span data-ttu-id="c90e7-662">Os módulos Az já estão disponíveis em pré-visualização no Azure Stack Hub.</span><span class="sxs-lookup"><span data-stu-id="c90e7-662">Az modules is now available in preview on Azure Stack Hub.</span></span> <span data-ttu-id="c90e7-663">Isto permite a compatibilidade entre plataformas diferentes com o Linux e macOS.</span><span class="sxs-lookup"><span data-stu-id="c90e7-663">This allows for cross-platform compatibility with Linux and macOs.</span></span> <span data-ttu-id="c90e7-664">Agora, o Azure Stack Hub suporta o PowerShell Core com os módulos Az. Obtenha mais informações [aqui](https://aka.ms/az4AzureStack)</span><span class="sxs-lookup"><span data-stu-id="c90e7-664">Azure Stack Hub now supports PowerShell core with the Az modules, more information [here](https://aka.ms/az4AzureStack)</span></span>
* <span data-ttu-id="c90e7-665">Os módulos Az suportam o perfil 2019-03-01-hybrid:</span><span class="sxs-lookup"><span data-stu-id="c90e7-665">Az modules support profile 2019-03-01-hybrid:</span></span>
  - <span data-ttu-id="c90e7-666">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="c90e7-666">Az.Billing</span></span>
  - <span data-ttu-id="c90e7-667">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-667">Az.Compute</span></span>
  - <span data-ttu-id="c90e7-668">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="c90e7-668">Az.DataBoxEdge</span></span>
  - <span data-ttu-id="c90e7-669">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-669">Az.EventHub</span></span>
  - <span data-ttu-id="c90e7-670">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-670">Az.IotHub</span></span>
  - <span data-ttu-id="c90e7-671">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c90e7-671">Az.KeyVault</span></span>
  - <span data-ttu-id="c90e7-672">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-672">Az.Monitor</span></span>
  - <span data-ttu-id="c90e7-673">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-673">Az.Network</span></span>
  - <span data-ttu-id="c90e7-674">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-674">Az.Resources</span></span>
  - <span data-ttu-id="c90e7-675">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-675">Az.Storage</span></span>
  - <span data-ttu-id="c90e7-676">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-676">Az.Websites</span></span>
* <span data-ttu-id="c90e7-677">Foram introduzidos três novos módulos do PowerShell para Az que funcionam com o Azure Stack Hub. São eles o Az.Databox, Az.IotHub e Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-677">Three new PowerShell modules for az have been introduced that work with Azure Stack Hub, which are Az.Databox, Az.IotHub, and Az.EventHub</span></span>
* <span data-ttu-id="c90e7-678">Os comandos permanecem sensivelmente iguais, com pequenas alterações como, por exemplo, a alteração do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="c90e7-678">Commands remain relatively the same, with minor changes such as changing AzureRM to Az</span></span>
* <span data-ttu-id="c90e7-679">Veja uma ligação atualizada à documentação do PowerShell para o Azure Stack Hub [aqui](https://aka.ms/InstallASHPowerShell)</span><span class="sxs-lookup"><span data-stu-id="c90e7-679">Updated link to PowerShell documentation for Azure Stack Hub can be found [here](https://aka.ms/InstallASHPowerShell)</span></span>

## <a name="370---march-2020"></a><span data-ttu-id="c90e7-680">3.7.0 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="c90e7-680">3.7.0 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c90e7-681">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-681">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-682">Foram corrigidos os parâmetros "Get-AzTenant"/"Get-AzDefault"/"Set-AzDefault" que emitiam uma NullReferenceException quando a sessão não estava iniciada [#10292]</span><span class="sxs-lookup"><span data-stu-id="c90e7-682">Fixed 'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' throw NullReferenceException when not login [#10292]</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-683">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-683">Az.Compute</span></span>
* <span data-ttu-id="c90e7-684">Foram adicionados os seguintes parâmetros ao cmdlet "New-AzDiskConfig":</span><span class="sxs-lookup"><span data-stu-id="c90e7-684">Added the following parameters to 'New-AzDiskConfig' cmdlet:</span></span>
    - <span data-ttu-id="c90e7-685">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span><span class="sxs-lookup"><span data-stu-id="c90e7-685">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span></span>
* <span data-ttu-id="c90e7-686">A propriedade Encryption foi permitida para o parâmetro Target do cmdlet "New-AzGalleryImageVersion".</span><span class="sxs-lookup"><span data-stu-id="c90e7-686">Allowed Encryption property to Target parameter of 'New-AzGalleryImageVersion' cmdlet.</span></span>
* <span data-ttu-id="c90e7-687">Foi corrigido o problema de tempDisk para os cmdlets "Set-AzVmss" -Reimage e "Invoke-AzVMReimage".</span><span class="sxs-lookup"><span data-stu-id="c90e7-687">Fixed tempDisk issue for 'Set-AzVmss' -Reimage and 'Invoke-AzVMReimage' cmdlets.</span></span> <span data-ttu-id="c90e7-688">[#11354]</span><span class="sxs-lookup"><span data-stu-id="c90e7-688">[#11354]</span></span>
* <span data-ttu-id="c90e7-689">Foi adicionado suporte aos cmdlets abaixo para a nova Extensão SAP</span><span class="sxs-lookup"><span data-stu-id="c90e7-689">Added support to below cmdlets for new SAP Extension</span></span>
    - <span data-ttu-id="c90e7-690">"Set-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="c90e7-690">'Set-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="c90e7-691">"Get-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="c90e7-691">'Get-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="c90e7-692">"Remove-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="c90e7-692">'Remove-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="c90e7-693">"Update-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="c90e7-693">'Update-AzVMAEMExtension'</span></span>
* <span data-ttu-id="c90e7-694">Foram corrigidos os erros em exemplos do documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="c90e7-694">Fixed errors in examples of help document</span></span>
* <span data-ttu-id="c90e7-695">É apresentado o valor de cadeia exato para o PowerState da VM no formato de tabela.</span><span class="sxs-lookup"><span data-stu-id="c90e7-695">Showed the exact string value for VM PowerState in the table format.</span></span>
* <span data-ttu-id="c90e7-696">"New-AzVmssConfig": foi corrigida a serialização da propriedade AutomaticRepairs quando a opção SinglePlacementGroup está desativada.</span><span class="sxs-lookup"><span data-stu-id="c90e7-696">'New-AzVmssConfig': fixed serialization of AutomaticRepairs property when SinglePlacementGroup is disabled.</span></span> <span data-ttu-id="c90e7-697">[#11257]</span><span class="sxs-lookup"><span data-stu-id="c90e7-697">[#11257]</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-698">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-698">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-699">Atualização da versão do SDK .Net do ADF para 4.8.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-699">Updated ADF .Net SDK version to 4.8.0</span></span>
* <span data-ttu-id="c90e7-700">Foram adicionados parâmetros opcionais ao comando "Invoke-AzDataFactoryV2Pipeline" para suportar uma nova execução</span><span class="sxs-lookup"><span data-stu-id="c90e7-700">Added optional parameters to 'Invoke-AzDataFactoryV2Pipeline' command to support rerun</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c90e7-701">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c90e7-701">Az.DataLakeStore</span></span>
* <span data-ttu-id="c90e7-702">Foi adicionada a descrição da alteração interruptiva para "Export-AzDataLakeStoreItem" e "Import-AzDataLakeStoreItem"</span><span class="sxs-lookup"><span data-stu-id="c90e7-702">Added breaking change description for 'Export-AzDataLakeStoreItem' and 'Import-AzDataLakeStoreItem'</span></span>
* <span data-ttu-id="c90e7-703">Foi adicionada a opção de codificação de bytes para "New-AzDataLakeStoreItem", "Add-AzDAtaLakeStoreItemContent" e "Get-AzDAtaLakeStoreItemContent"</span><span class="sxs-lookup"><span data-stu-id="c90e7-703">Added option of Byte encoding for 'New-AzDataLakeStoreItem', 'Add-AzDAtaLakeStoreItemContent', and 'Get-AzDAtaLakeStoreItemContent'</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c90e7-704">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c90e7-704">Az.HDInsight</span></span>
* <span data-ttu-id="c90e7-705">É suportada a versão de TLS mínima suportada ao criar o cluster.</span><span class="sxs-lookup"><span data-stu-id="c90e7-705">Supported specifying minimal supported TLS version when creating cluster.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c90e7-706">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-706">Az.IotHub</span></span>
* <span data-ttu-id="c90e7-707">Foi adicionado suporte para gerir as definições distribuídas por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c90e7-707">Added support to manage distributed settings per-device.</span></span> <span data-ttu-id="c90e7-708">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c90e7-708">New Cmdlets are:</span></span>
    - <span data-ttu-id="c90e7-709">"Get-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="c90e7-709">'Get-AzIotHubDistributedTracing'</span></span>
    - <span data-ttu-id="c90e7-710">"Set-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="c90e7-710">'Set-AzIotHubDistributedTracing'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c90e7-711">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c90e7-711">Az.KeyVault</span></span>
* <span data-ttu-id="c90e7-712">Foram adicionados os atributos da alteração interruptiva a "New-AzKeyVault"</span><span class="sxs-lookup"><span data-stu-id="c90e7-712">Added breaking change attributes to 'New-AzKeyVault'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c90e7-713">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-713">Az.Monitor</span></span>
* <span data-ttu-id="c90e7-714">Foi atualizada a documentação de "New-AzScheduledQueryRuleLogMetricTrigger"</span><span class="sxs-lookup"><span data-stu-id="c90e7-714">Updated documentation for 'New-AzScheduledQueryRuleLogMetricTrigger'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-715">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-715">Az.Network</span></span>
* <span data-ttu-id="c90e7-716">Foram atualizados os cmdlets para permitir VirtualHubVnetConnections entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="c90e7-716">Updated cmdlets to allow cross-tenant VirtualHubVnetConnections</span></span>
    - <span data-ttu-id="c90e7-717">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="c90e7-717">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="c90e7-718">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="c90e7-718">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="c90e7-719">"New-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="c90e7-719">'New-AzVirtualHub'</span></span>
    - <span data-ttu-id="c90e7-720">"Update-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="c90e7-720">'Update-AzVirtualHub'</span></span>
* <span data-ttu-id="c90e7-721">Foi removida a dependência do SDK do SQL Management</span><span class="sxs-lookup"><span data-stu-id="c90e7-721">Removed Sql Management SDK dependency</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c90e7-722">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-722">Az.PolicyInsights</span></span>
* <span data-ttu-id="c90e7-723">Mensagens de erro melhoradas</span><span class="sxs-lookup"><span data-stu-id="c90e7-723">Improved error messages</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-724">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-724">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-725">O Azure Site Recovery adicionou suporte para nova proteção e atualização das propriedades de VM para Máquinas Virtuais encriptadas em disco do Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-725">Azure Site Recovery added support for doing reprotect and updated vm properties for Azure disk encrypted Virtual Machines.</span></span>
* <span data-ttu-id="c90e7-726">Foi adicionada monitorização DR das propriedades VmwareToAzure ao Azure Site Recovery</span><span class="sxs-lookup"><span data-stu-id="c90e7-726">Added Azure Site Recovery VmwareToAzure properties DR monitoring</span></span>
* <span data-ttu-id="c90e7-727">O Azure Backup adicionou suporte para repetir a atualização de políticas para itens falhados.</span><span class="sxs-lookup"><span data-stu-id="c90e7-727">Azure Backup added support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="c90e7-728">O Azure Backup adicionou suporte para definições de exclusão do disco durante a cópia de segurança e o restauro.</span><span class="sxs-lookup"><span data-stu-id="c90e7-728">Azure Backup Added support for disk exclusion settings during backup and restore.</span></span>
* <span data-ttu-id="c90e7-729">O Azure Backup adicionou suporte para restaurar vários ficheiros/pastas no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="c90e7-729">Azure Backup Added Support for Restoring Multiple files/folders in AzureFileShare</span></span>
* <span data-ttu-id="c90e7-730">O Azure Backup adicionou suporte para o Resourcegroup especificado pelo utilizador durante a atualização da Política IaasVM</span><span class="sxs-lookup"><span data-stu-id="c90e7-730">Azure Backup Added support for User-specified Resourcegroup support while updating IaasVM Policy</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-731">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-731">Az.Resources</span></span>
* <span data-ttu-id="c90e7-732">Foi corrigido o parâmetro "Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType" para utilizar a apiVersion real dos recursos em vez da apiVersion predefinida [#11267]</span><span class="sxs-lookup"><span data-stu-id="c90e7-732">Fixed 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' to use actual apiVersion of resources instead of default apiVersion [#11267]</span></span>
* <span data-ttu-id="c90e7-733">Foi adicionado o registo de correlationId para cenários de erro</span><span class="sxs-lookup"><span data-stu-id="c90e7-733">Added correlationId logging for error scenarios</span></span>
* <span data-ttu-id="c90e7-734">Pequena alteração à documentação referente a "Get-AzResourceLock".</span><span class="sxs-lookup"><span data-stu-id="c90e7-734">Small documentation change to 'Get-AzResourceLock'.</span></span> <span data-ttu-id="c90e7-735">Exemplo adicionado.</span><span class="sxs-lookup"><span data-stu-id="c90e7-735">Added example.</span></span>
* <span data-ttu-id="c90e7-736">Aspas com caráter de escape no valor de parâmetro "Get-AzADUser" [#11317]</span><span class="sxs-lookup"><span data-stu-id="c90e7-736">Escaped single quote in parameter value of 'Get-AzADUser' [#11317]</span></span>
* <span data-ttu-id="c90e7-737">Foram adicionados novos cmdlets aos Scripts de Implementação ("Get-AzDeploymentScript", "Get-AzDeploymentScriptLog", "Save-AzDeploymentScriptLog", "Remove-AzDeploymentScript")</span><span class="sxs-lookup"><span data-stu-id="c90e7-737">Added new cmdlets for Deployment Scripts ('Get-AzDeploymentScript', 'Get-AzDeploymentScriptLog', 'Save-AzDeploymentScriptLog', 'Remove-AzDeploymentScript')</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-738">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-738">Az.Sql</span></span>
* <span data-ttu-id="c90e7-739">Foi adicionado um parâmetro secundário legível a "Invoke-AzSqlDatabaseFailover"</span><span class="sxs-lookup"><span data-stu-id="c90e7-739">Added readable secondary parameter to 'Invoke-AzSqlDatabaseFailover'</span></span>
* <span data-ttu-id="c90e7-740">Foi adicionado o cmdlet "Disable-AzSqlServerActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="c90e7-740">Added cmdlet 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="c90e7-741">Classificação de sensibilidade guardada ao classificar as colunas na base de dados.</span><span class="sxs-lookup"><span data-stu-id="c90e7-741">Saved sensitivity rank when classifying columns in the database.</span></span>

#### <a name="azsupport"></a><span data-ttu-id="c90e7-742">Az.Support</span><span class="sxs-lookup"><span data-stu-id="c90e7-742">Az.Support</span></span>
* <span data-ttu-id="c90e7-743">Disponibilidade geral do módulo "Az.Support"</span><span class="sxs-lookup"><span data-stu-id="c90e7-743">General availability of 'Az.Support' module</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-744">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-744">Az.Websites</span></span>
* <span data-ttu-id="c90e7-745">Foi adicionado suporte para utilizar Regras de Encaminhamento de Tráfego webapp através dos novos cmdlets abaixo</span><span class="sxs-lookup"><span data-stu-id="c90e7-745">Added support for working with webapp Traffic Routing Rules via below new cmdlets</span></span>
    - <span data-ttu-id="c90e7-746">"Get-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="c90e7-746">'Get-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="c90e7-747">"Update-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="c90e7-747">'Update-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="c90e7-748">"Add-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="c90e7-748">'Add-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="c90e7-749">"Remove-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="c90e7-749">'Remove-AzWebAppTrafficRouting'</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="c90e7-750">3.6.1 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="c90e7-750">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c90e7-751">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-751">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-752">Abrir a página de inquérito do Azure PowerShell em "Send-Feedback" [#11020]</span><span class="sxs-lookup"><span data-stu-id="c90e7-752">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="c90e7-753">Apresentar o URL de inquérito do Azure PowerShell em "Resolve-Error" [#11021]</span><span class="sxs-lookup"><span data-stu-id="c90e7-753">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="c90e7-754">Adicionada versão de Az em UserAgent</span><span class="sxs-lookup"><span data-stu-id="c90e7-754">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c90e7-755">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c90e7-755">Az.ApiManagement</span></span>
* <span data-ttu-id="c90e7-756">Adicionado suporte para a obtenção e configuração do Domínio Personalizado no Ponto Final do DeveloperPortal [#11007]</span><span class="sxs-lookup"><span data-stu-id="c90e7-756">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="c90e7-757">"Export-AzApiManagementApi" Adicionado suporte para a transferência da definição da API no formato JSON [#9987]</span><span class="sxs-lookup"><span data-stu-id="c90e7-757">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="c90e7-758">"Import-AzApiManagementApi" Adicionado suporte para a importação da definição de OpenApi 3.0 a partir de documento JSON</span><span class="sxs-lookup"><span data-stu-id="c90e7-758">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="c90e7-759">"New-AzApiManagementIdentityProvider" e "Set-AzApiManagementIdentityProvider" Adicionado suporte para a configuração de "Inquilino de Início de Sessão" para Fornecedor de AAD B2C [#9784]</span><span class="sxs-lookup"><span data-stu-id="c90e7-759">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c90e7-760">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c90e7-760">Az.DataLakeStore</span></span>
* <span data-ttu-id="c90e7-761">Adicionada referência a System.Buffers explicitamente em csproj e psd1.</span><span class="sxs-lookup"><span data-stu-id="c90e7-761">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c90e7-762">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-762">Az.IotHub</span></span>
* <span data-ttu-id="c90e7-763">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="c90e7-763">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="c90e7-764">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c90e7-764">New Cmdlets are:</span></span>
    - <span data-ttu-id="c90e7-765">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c90e7-765">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c90e7-766">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c90e7-766">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c90e7-767">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c90e7-767">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c90e7-768">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c90e7-768">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="c90e7-769">Adicionado suporte para a gestão de módulos num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="c90e7-769">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="c90e7-770">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c90e7-770">New Cmdlets are:</span></span>
    - <span data-ttu-id="c90e7-771">"Add-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="c90e7-771">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="c90e7-772">"Get-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="c90e7-772">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="c90e7-773">"Remove-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="c90e7-773">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="c90e7-774">"Set-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="c90e7-774">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="c90e7-775">Adicionado cmdlet para obter a cadeia de ligação de um dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="c90e7-775">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="c90e7-776">Adicionado cmdlet para obter a cadeia de ligação de um módulo num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="c90e7-776">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="c90e7-777">Adicionado suporte para obter/definir dispositivo principal de um dispositivo IoT.</span><span class="sxs-lookup"><span data-stu-id="c90e7-777">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="c90e7-778">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c90e7-778">New Cmdlets are:</span></span>
    - <span data-ttu-id="c90e7-779">"Get-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="c90e7-779">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="c90e7-780">"Set-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="c90e7-780">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="c90e7-781">Adicionado suporte para gerir relações principal-subordinado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c90e7-781">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c90e7-782">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-782">Az.Monitor</span></span>
* <span data-ttu-id="c90e7-783">Corrigido o valor de saída de "Get-AzMetricDefinition" [#9714]</span><span class="sxs-lookup"><span data-stu-id="c90e7-783">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-784">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-784">Az.Network</span></span>
* <span data-ttu-id="c90e7-785">Sdk Sql Management atualizado.</span><span class="sxs-lookup"><span data-stu-id="c90e7-785">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="c90e7-786">Corrigido um problema de diferença de nomes na classe PrivateLinkServiceConnectionState.</span><span class="sxs-lookup"><span data-stu-id="c90e7-786">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="c90e7-787">Mapeamento do campo ActionsRequired para ActionRequired.</span><span class="sxs-lookup"><span data-stu-id="c90e7-787">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="c90e7-788">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="c90e7-788">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-789">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-789">Az.Resources</span></span>
* <span data-ttu-id="c90e7-790">Correção para erro de referência nula em "Get-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="c90e7-790">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="c90e7-791">Comutadores "-Force" e "-PassThru" marcados como opcionais em "Remove-AzADGroup" [#10849]</span><span class="sxs-lookup"><span data-stu-id="c90e7-791">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="c90e7-792">Corrigido problema em que "MailNickname" não devolve "Remove-AzADGroup" [#11167]</span><span class="sxs-lookup"><span data-stu-id="c90e7-792">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="c90e7-793">Corrigido problema em que a operação de pipe "Remove-AzADGroup" não funciona [#11171]</span><span class="sxs-lookup"><span data-stu-id="c90e7-793">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="c90e7-794">Correção para erro de referência nula em GetAzureRoleAssignmentCommand</span><span class="sxs-lookup"><span data-stu-id="c90e7-794">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="c90e7-795">Adicionados atributos de alterações interruptivas para futuras alterações a cmdlets de política</span><span class="sxs-lookup"><span data-stu-id="c90e7-795">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="c90e7-796">"Get-AzResourceGroup" atualizado para realizar filtragem de etiqueta de grupo de recursos no lado do servidor</span><span class="sxs-lookup"><span data-stu-id="c90e7-796">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="c90e7-797">Cmdlets Tag alargados para accept -ResourceId</span><span class="sxs-lookup"><span data-stu-id="c90e7-797">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="c90e7-798">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="c90e7-798">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="c90e7-799">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="c90e7-799">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="c90e7-800">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="c90e7-800">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="c90e7-801">Adicionado cmdlet Tag novo</span><span class="sxs-lookup"><span data-stu-id="c90e7-801">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="c90e7-802">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="c90e7-802">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="c90e7-803">ScopedDeployment trazido de SDK 3.3.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-803">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-804">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-804">Az.Sql</span></span>
* <span data-ttu-id="c90e7-805">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="c90e7-805">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="c90e7-806">Adicionado suporte para configuração de cópia de segurança de Retenção de Longo Prazo para Bases de Dados Geridas</span><span class="sxs-lookup"><span data-stu-id="c90e7-806">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="c90e7-807">Política Get/Set numa base de dados gerida</span><span class="sxs-lookup"><span data-stu-id="c90e7-807">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="c90e7-808">Obter cópia(s) de segurança LTR por base de dados gerida, por instância gerida ou por localização</span><span class="sxs-lookup"><span data-stu-id="c90e7-808">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="c90e7-809">Remover uma cópia de segurança LTR</span><span class="sxs-lookup"><span data-stu-id="c90e7-809">Remove an LTR backup</span></span>
    - <span data-ttu-id="c90e7-810">Restaurar uma cópia de segurança LTR para criar uma base de dados gerida nova</span><span class="sxs-lookup"><span data-stu-id="c90e7-810">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="c90e7-811">Adicionado MinimalTlsVersion a New-AzSqlServer e Set-AzSqlServer</span><span class="sxs-lookup"><span data-stu-id="c90e7-811">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="c90e7-812">Adicionado MinimalTlsVersion a New-AzSqlInstance e Set-AzSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c90e7-812">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="c90e7-813">Versão de SDK SQL atualizada para Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-813">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-814">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-814">Az.Storage</span></span>
* <span data-ttu-id="c90e7-815">AllowProtectedAppendWrite suportada em ImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="c90e7-815">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="c90e7-816">"Set-AzRmStorageContainerImmutabilityPolicy"</span><span class="sxs-lookup"><span data-stu-id="c90e7-816">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="c90e7-817">Adicionada uma mensagem de aviso de alteração interruptiva para alteração do tipo AzureStorageTable numa futura versão</span><span class="sxs-lookup"><span data-stu-id="c90e7-817">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="c90e7-818">"New-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="c90e7-818">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="c90e7-819">"Get-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="c90e7-819">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-820">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-820">Az.Websites</span></span>
* <span data-ttu-id="c90e7-821">Adicionado o parâmetro Tag para "New-AzAppServicePlan" e "Set-AzAppServicePlan"</span><span class="sxs-lookup"><span data-stu-id="c90e7-821">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="c90e7-822">Paragem da execução de cmdlet caso seja emitida uma exceção ao adicionar um domínio personalizado a um site</span><span class="sxs-lookup"><span data-stu-id="c90e7-822">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="c90e7-823">Adicionado suporte para a realização de operações para Serviços de Aplicações em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="c90e7-823">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="c90e7-824">Aplicada restrição de acesso a WebApp/Função em diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="c90e7-824">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="c90e7-825">Corrigido problema para definir os nomes de anfitrião personalizados para WebAppSlots</span><span class="sxs-lookup"><span data-stu-id="c90e7-825">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="c90e7-826">3.5.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="c90e7-826">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c90e7-827">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="c90e7-827">Highlights since the last major release</span></span>
* <span data-ttu-id="c90e7-828">Telemetria do lado do cliente atualizada.</span><span class="sxs-lookup"><span data-stu-id="c90e7-828">Updated client side telemetry.</span></span>
* <span data-ttu-id="c90e7-829">O Az.IotHub adicionou cmdlets para suportar a gestão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="c90e7-829">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="c90e7-830">O Az.SqlVirtualMachine adicionou cmdlets ao Serviço de Escuta do Grupo de Disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="c90e7-830">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c90e7-831">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-831">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-832">SubscriptionId, TenantId e tempo de execução adicionados aos dados de telemetria do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="c90e7-832">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c90e7-833">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-833">Az.Automation</span></span>
* <span data-ttu-id="c90e7-834">Foi corrigido o erro no Exemplo 1 na documentação de referência de "New-AzAutomationSoftwareUpdateConfiguration"</span><span class="sxs-lookup"><span data-stu-id="c90e7-834">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c90e7-835">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-835">Az.CognitiveServices</span></span>
* <span data-ttu-id="c90e7-836">SDK atualizado para a versão 7.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-836">Updated SDK to 7.0</span></span>
* <span data-ttu-id="c90e7-837">Mensagem de erro melhorada quando o servidor responde ao corpo vazio</span><span class="sxs-lookup"><span data-stu-id="c90e7-837">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-838">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-838">Az.Compute</span></span>
* <span data-ttu-id="c90e7-839">Valor vazio permitido para ProximityPlacementGroupId durante a atualização</span><span class="sxs-lookup"><span data-stu-id="c90e7-839">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c90e7-840">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c90e7-840">Az.FrontDoor</span></span>
* <span data-ttu-id="c90e7-841">Cmdlet adicionado para obter definições de regras geridas que podem ser utilizadas na WAF</span><span class="sxs-lookup"><span data-stu-id="c90e7-841">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c90e7-842">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-842">Az.IotHub</span></span>
* <span data-ttu-id="c90e7-843">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="c90e7-843">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="c90e7-844">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c90e7-844">New Cmdlets are:</span></span>
    - <span data-ttu-id="c90e7-845">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c90e7-845">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c90e7-846">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c90e7-846">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c90e7-847">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c90e7-847">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c90e7-848">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="c90e7-848">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c90e7-849">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c90e7-849">Az.KeyVault</span></span>
* <span data-ttu-id="c90e7-850">Texto duplicado fixo para Add-AzKeyVaultKey.md</span><span class="sxs-lookup"><span data-stu-id="c90e7-850">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c90e7-851">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-851">Az.Monitor</span></span>
* <span data-ttu-id="c90e7-852">Descrição fixa do cmdlet Get-AzLog.</span><span class="sxs-lookup"><span data-stu-id="c90e7-852">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="c90e7-853">Foi adicionado um novo parâmetro chamado ActionGroupId ao comando "New-AzMetricAlertRuleV2".</span><span class="sxs-lookup"><span data-stu-id="c90e7-853">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="c90e7-854">O utilizador pode fornecer ActionGroupId(string) ou ActionGorup(ActivityLogAlertActionGroup).</span><span class="sxs-lookup"><span data-stu-id="c90e7-854">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-855">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-855">Az.Network</span></span>
* <span data-ttu-id="c90e7-856">Foi adicionada uma nota de parâmetro adicional para o parâmetro "-EnableProxyProtocol" para o cmdlet "New-AzPrivateLinkService".</span><span class="sxs-lookup"><span data-stu-id="c90e7-856">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="c90e7-857">Exemplo de FilterData fixo em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="c90e7-857">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="c90e7-858">Exemplo de Captura de Pacotes adicionado para capturar todos os pacotes internos e externos em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="c90e7-858">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="c90e7-859">Política do Azure Firewall suportada em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="c90e7-859">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="c90e7-860">Não foram adicionados novos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="c90e7-860">No new cmdlets are added.</span></span> <span data-ttu-id="c90e7-861">Simplificação da restrição da política de firewall em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="c90e7-861">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-862">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-862">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-863">Suporte adicionado da funcionalidade Restaurar como ficheiros para Bases de Dados SQL.</span><span class="sxs-lookup"><span data-stu-id="c90e7-863">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-864">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-864">Az.Resources</span></span>
* <span data-ttu-id="c90e7-865">Cmdlets de implementação de modelos refatorizados</span><span class="sxs-lookup"><span data-stu-id="c90e7-865">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="c90e7-866">Foram adicionados novos cmdlets para gerir implementações no grupo de gestão: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="c90e7-866">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="c90e7-867">Foram adicionados novos cmdlets para gerir implementações no inquilino: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="c90e7-867">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="c90e7-868">Cmdlets \*-AzDeployment refatorizados para trabalhar especificamente no âmbito da subscrição</span><span class="sxs-lookup"><span data-stu-id="c90e7-868">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="c90e7-869">Foram criados aliases \*-AzSubscriptionDeployment para os cmdlets \*-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="c90e7-869">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="c90e7-870">"Update-AzADApplication" fixo quando o parâmetro "AvailableToOtherTenants" não está definido</span><span class="sxs-lookup"><span data-stu-id="c90e7-870">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="c90e7-871">ApplicationObjectWithoutCredentialParameterSet removido para evitar AmbiguousParameterSetException.</span><span class="sxs-lookup"><span data-stu-id="c90e7-871">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="c90e7-872">Ficheiros de ajuda regenerados</span><span class="sxs-lookup"><span data-stu-id="c90e7-872">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-873">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-873">Az.Sql</span></span>
* <span data-ttu-id="c90e7-874">Suporte adicionado para restauro para um ponto anterior no tempo entre subscrições nas Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="c90e7-874">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="c90e7-875">Suporte adicionado para alterar a geração de hardware das Instâncias Geridas de SQL existentes</span><span class="sxs-lookup"><span data-stu-id="c90e7-875">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="c90e7-876">Exemplos de ajuda "Update-AzSqlServerVulnerabilityAssessmentSetting" fixos: saída do parâmetro/propriedade - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="c90e7-876">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="c90e7-877">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="c90e7-877">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="c90e7-878">Cmdlets adicionados para o Serviço de Escuta do Grupo de Disponibilidade</span><span class="sxs-lookup"><span data-stu-id="c90e7-878">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="c90e7-879">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="c90e7-879">Az.StorageSync</span></span>
* <span data-ttu-id="c90e7-880">Conjuntos de carateres suportados atualizados em "Invoke-AzStorageSyncCompatibilityCheck".</span><span class="sxs-lookup"><span data-stu-id="c90e7-880">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="c90e7-881">3.4.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="c90e7-881">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c90e7-882">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="c90e7-882">Highlights since the last major release</span></span>
* <span data-ttu-id="c90e7-883">Versão inicial Az.CosmosDB 0.1.0 lançada</span><span class="sxs-lookup"><span data-stu-id="c90e7-883">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="c90e7-884">Foi adicionado suporte para Az.Network ConnectionMonitor V2</span><span class="sxs-lookup"><span data-stu-id="c90e7-884">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c90e7-885">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-885">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-886">Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível</span><span class="sxs-lookup"><span data-stu-id="c90e7-886">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="c90e7-887">Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5</span><span class="sxs-lookup"><span data-stu-id="c90e7-887">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c90e7-888">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c90e7-888">Az.ApiManagement</span></span>
* <span data-ttu-id="c90e7-889">**Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="c90e7-889">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="c90e7-890">**New-AzApiManagementProduct**\* e **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="c90e7-890">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="c90e7-891">Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472</span><span class="sxs-lookup"><span data-stu-id="c90e7-891">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="c90e7-892">**Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet</span><span class="sxs-lookup"><span data-stu-id="c90e7-892">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-893">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-893">Az.Compute</span></span>
* <span data-ttu-id="c90e7-894">Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.</span><span class="sxs-lookup"><span data-stu-id="c90e7-894">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="c90e7-895">Foi adicionado o cmdlet Update-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-895">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="c90e7-896">Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c90e7-896">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="c90e7-897">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-897">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="c90e7-898">Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="c90e7-898">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-899">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-899">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-900">Atualização do SDK .NET do ADF para a versão 4.7.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-900">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="c90e7-901">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="c90e7-901">Az.DeploymentManager</span></span>
* <span data-ttu-id="c90e7-902">Adiciona operações LIST para os recursos</span><span class="sxs-lookup"><span data-stu-id="c90e7-902">Adds LIST operations for resources</span></span>
* <span data-ttu-id="c90e7-903">Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="c90e7-903">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c90e7-904">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c90e7-904">Az.HDInsight</span></span>
* <span data-ttu-id="c90e7-905">Foi corrigido o erro do documento de New-AzHDInsightCluster.</span><span class="sxs-lookup"><span data-stu-id="c90e7-905">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c90e7-906">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c90e7-906">Az.KeyVault</span></span>
* <span data-ttu-id="c90e7-907">Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.</span><span class="sxs-lookup"><span data-stu-id="c90e7-907">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-908">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-908">Az.Network</span></span>
* <span data-ttu-id="c90e7-909">Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="c90e7-909">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="c90e7-910">Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão</span><span class="sxs-lookup"><span data-stu-id="c90e7-910">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="c90e7-911">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="c90e7-911">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="c90e7-912">Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="c90e7-912">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="c90e7-913">Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"</span><span class="sxs-lookup"><span data-stu-id="c90e7-913">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="c90e7-914">Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.</span><span class="sxs-lookup"><span data-stu-id="c90e7-914">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="c90e7-915">Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="c90e7-915">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="c90e7-916">Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="c90e7-916">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="c90e7-917">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c90e7-917">New cmdlets added:</span></span>
        - <span data-ttu-id="c90e7-918">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="c90e7-918">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="c90e7-919">Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="c90e7-919">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="c90e7-920">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-920">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="c90e7-921">Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2</span><span class="sxs-lookup"><span data-stu-id="c90e7-921">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c90e7-922">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-922">Az.PolicyInsights</span></span>
* <span data-ttu-id="c90e7-923">Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar</span><span class="sxs-lookup"><span data-stu-id="c90e7-923">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="c90e7-924">Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation</span><span class="sxs-lookup"><span data-stu-id="c90e7-924">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="c90e7-925">Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política</span><span class="sxs-lookup"><span data-stu-id="c90e7-925">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="c90e7-926">Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="c90e7-926">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-927">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-927">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-928">Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.</span><span class="sxs-lookup"><span data-stu-id="c90e7-928">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="c90e7-929">O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.</span><span class="sxs-lookup"><span data-stu-id="c90e7-929">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-930">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-930">Az.Resources</span></span>
* <span data-ttu-id="c90e7-931">-Scope foi tornado opcional nos cmdlets \*-AzPolicyAssignment com subscrição de contexto predefinida</span><span class="sxs-lookup"><span data-stu-id="c90e7-931">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="c90e7-932">Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves</span><span class="sxs-lookup"><span data-stu-id="c90e7-932">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-933">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-933">Az.Sql</span></span>
<span data-ttu-id="c90e7-934">Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.</span><span class="sxs-lookup"><span data-stu-id="c90e7-934">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-935">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-935">Az.Storage</span></span>
* <span data-ttu-id="c90e7-936">Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="c90e7-936">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="c90e7-937">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-937">New-AzStorageAccount</span></span>
* <span data-ttu-id="c90e7-938">Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation</span><span class="sxs-lookup"><span data-stu-id="c90e7-938">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="c90e7-939">Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="c90e7-939">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-940">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-940">Az.Websites</span></span>
* <span data-ttu-id="c90e7-941">Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState</span><span class="sxs-lookup"><span data-stu-id="c90e7-941">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="c90e7-942">Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido</span><span class="sxs-lookup"><span data-stu-id="c90e7-942">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="c90e7-943">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="c90e7-943">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c90e7-944">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-944">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-945">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="c90e7-945">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c90e7-946">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c90e7-946">Az.Cdn</span></span>
* <span data-ttu-id="c90e7-947">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="c90e7-947">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-948">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-948">Az.Compute</span></span>
* <span data-ttu-id="c90e7-949">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="c90e7-949">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="c90e7-950">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c90e7-950">Az.ContainerInstance</span></span>
* <span data-ttu-id="c90e7-951">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="c90e7-951">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="c90e7-952">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="c90e7-952">Az.DataBoxEdge</span></span>
* <span data-ttu-id="c90e7-953">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="c90e7-953">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="c90e7-954">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="c90e7-954">Get the Edge Storage Container</span></span>
* <span data-ttu-id="c90e7-955">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="c90e7-955">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="c90e7-956">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="c90e7-956">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="c90e7-957">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="c90e7-957">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="c90e7-958">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="c90e7-958">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="c90e7-959">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="c90e7-959">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="c90e7-960">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="c90e7-960">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="c90e7-961">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c90e7-961">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="c90e7-962">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="c90e7-962">Get the Edge Storage Account</span></span>
* <span data-ttu-id="c90e7-963">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c90e7-963">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="c90e7-964">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="c90e7-964">Create new Edge Storage Account</span></span>
* <span data-ttu-id="c90e7-965">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="c90e7-965">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="c90e7-966">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="c90e7-966">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="c90e7-967">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="c90e7-967">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="c90e7-968">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="c90e7-968">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="c90e7-969">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="c90e7-969">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="c90e7-970">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="c90e7-970">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-971">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-971">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-972">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="c90e7-972">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="c90e7-973">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-973">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="c90e7-974">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="c90e7-974">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="c90e7-975">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="c90e7-975">Az.DevTestLabs</span></span>
* <span data-ttu-id="c90e7-976">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="c90e7-976">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c90e7-977">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-977">Az.EventHub</span></span>
* <span data-ttu-id="c90e7-978">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="c90e7-978">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c90e7-979">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c90e7-979">Az.HDInsight</span></span>
* <span data-ttu-id="c90e7-980">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="c90e7-980">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="c90e7-981">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="c90e7-981">Az.MachineLearning</span></span>
* <span data-ttu-id="c90e7-982">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="c90e7-982">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="c90e7-983">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="c90e7-983">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="c90e7-984">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="c90e7-984">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="c90e7-985">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="c90e7-985">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="c90e7-986">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="c90e7-986">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="c90e7-987">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="c90e7-987">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="c90e7-988">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="c90e7-988">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="c90e7-989">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="c90e7-989">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-990">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-990">Az.Network</span></span>
* <span data-ttu-id="c90e7-991">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="c90e7-991">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-992">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-992">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-993">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-993">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="c90e7-994">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-994">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="c90e7-995">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-995">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="c90e7-996">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-996">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-997">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-997">Az.Resources</span></span>
* <span data-ttu-id="c90e7-998">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="c90e7-998">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-999">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-999">Az.Sql</span></span>
* <span data-ttu-id="c90e7-1000">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="c90e7-1000">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="c90e7-1001">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="c90e7-1001">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="c90e7-1002">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="c90e7-1002">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="c90e7-1003">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="c90e7-1003">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-1004">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-1004">Az.Storage</span></span>
* <span data-ttu-id="c90e7-1005">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="c90e7-1005">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="c90e7-1006">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-1006">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="c90e7-1007">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="c90e7-1007">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="c90e7-1008">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-1008">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="c90e7-1009">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-1009">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="c90e7-1010">Geral</span><span class="sxs-lookup"><span data-stu-id="c90e7-1010">General</span></span>
* <span data-ttu-id="c90e7-1011">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="c90e7-1011">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c90e7-1012">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-1012">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-1013">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-1013">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="c90e7-1014">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-1014">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c90e7-1015">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c90e7-1015">Az.Batch</span></span>
* <span data-ttu-id="c90e7-1016">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1016">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-1017">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-1017">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-1018">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-1018">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c90e7-1019">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c90e7-1019">Az.FrontDoor</span></span>
* <span data-ttu-id="c90e7-1020">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="c90e7-1020">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="c90e7-1021">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="c90e7-1021">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="c90e7-1022">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="c90e7-1022">Az.HealthcareApis</span></span>
* <span data-ttu-id="c90e7-1023">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="c90e7-1023">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c90e7-1024">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c90e7-1024">Az.KeyVault</span></span>
* <span data-ttu-id="c90e7-1025">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="c90e7-1025">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="c90e7-1026">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="c90e7-1026">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="c90e7-1027">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="c90e7-1027">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c90e7-1028">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-1028">Az.Monitor</span></span>
* <span data-ttu-id="c90e7-1029">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1029">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="c90e7-1030">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="c90e7-1030">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="c90e7-1031">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="c90e7-1031">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-1032">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-1032">Az.Network</span></span>
* <span data-ttu-id="c90e7-1033">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1033">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-1034">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-1034">Az.Resources</span></span>
* <span data-ttu-id="c90e7-1035">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1035">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="c90e7-1036">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1036">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-1037">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-1037">Az.Sql</span></span>
* <span data-ttu-id="c90e7-1038">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="c90e7-1038">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-1039">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-1039">Az.Storage</span></span>
* <span data-ttu-id="c90e7-1040">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="c90e7-1040">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="c90e7-1041">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="c90e7-1041">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="c90e7-1042">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="c90e7-1042">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="c90e7-1043">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="c90e7-1043">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="c90e7-1044">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="c90e7-1044">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="c90e7-1045">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1045">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="c90e7-1046">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1046">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="c90e7-1047">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c90e7-1047">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="c90e7-1048">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c90e7-1048">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="c90e7-1049">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1049">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="c90e7-1050">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="c90e7-1050">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="c90e7-1051">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="c90e7-1051">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="c90e7-1052">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="c90e7-1052">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="c90e7-1053">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-1053">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c90e7-1054">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="c90e7-1054">Highlights since the last major release</span></span>
* <span data-ttu-id="c90e7-1055">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="c90e7-1055">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="c90e7-1056">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="c90e7-1056">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-1057">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-1057">Az.Compute</span></span>
* <span data-ttu-id="c90e7-1058">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="c90e7-1058">VM Reapply feature</span></span>
    - <span data-ttu-id="c90e7-1059">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="c90e7-1059">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="c90e7-1060">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1060">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="c90e7-1061">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c90e7-1061">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="c90e7-1062">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="c90e7-1062">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="c90e7-1063">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c90e7-1063">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="c90e7-1064">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="c90e7-1064">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="c90e7-1065">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="c90e7-1065">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="c90e7-1066">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="c90e7-1066">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="c90e7-1067">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="c90e7-1067">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="c90e7-1068">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c90e7-1068">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="c90e7-1069">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="c90e7-1069">Az.DataBoxEdge</span></span>
* <span data-ttu-id="c90e7-1070">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="c90e7-1070">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="c90e7-1071">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="c90e7-1071">Get the Order</span></span>
* <span data-ttu-id="c90e7-1072">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="c90e7-1072">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="c90e7-1073">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="c90e7-1073">Create new Order</span></span>
* <span data-ttu-id="c90e7-1074">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="c90e7-1074">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="c90e7-1075">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="c90e7-1075">Remove the Order</span></span>
* <span data-ttu-id="c90e7-1076">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="c90e7-1076">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="c90e7-1077">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="c90e7-1077">Now creates Local Share</span></span>
* <span data-ttu-id="c90e7-1078">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="c90e7-1078">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="c90e7-1079">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="c90e7-1079">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="c90e7-1080">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="c90e7-1080">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="c90e7-1081">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="c90e7-1081">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="c90e7-1082">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="c90e7-1082">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="c90e7-1083">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="c90e7-1083">Gets the information about Triggers</span></span>
* <span data-ttu-id="c90e7-1084">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="c90e7-1084">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="c90e7-1085">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="c90e7-1085">Create new Triggers</span></span>
* <span data-ttu-id="c90e7-1086">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="c90e7-1086">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="c90e7-1087">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="c90e7-1087">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-1088">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-1088">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-1089">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-1089">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="c90e7-1090">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1090">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c90e7-1091">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c90e7-1091">Az.DataLakeStore</span></span>
* <span data-ttu-id="c90e7-1092">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="c90e7-1092">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c90e7-1093">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-1093">Az.EventHub</span></span>
* <span data-ttu-id="c90e7-1094">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="c90e7-1094">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c90e7-1095">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c90e7-1095">Az.FrontDoor</span></span>
* <span data-ttu-id="c90e7-1096">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="c90e7-1096">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="c90e7-1097">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="c90e7-1097">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="c90e7-1098">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="c90e7-1098">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="c90e7-1099">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="c90e7-1099">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-1100">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-1100">Az.Network</span></span>
* <span data-ttu-id="c90e7-1101">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1101">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="c90e7-1102">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="c90e7-1102">Az.PrivateDns</span></span>
* <span data-ttu-id="c90e7-1103">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-1103">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-1104">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-1104">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-1105">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1105">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="c90e7-1106">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1106">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="c90e7-1107">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1107">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="c90e7-1108">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c90e7-1108">Az.RedisCache</span></span>
* <span data-ttu-id="c90e7-1109">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1109">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="c90e7-1110">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1110">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="c90e7-1111">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1111">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-1112">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-1112">Az.Resources</span></span>
- <span data-ttu-id="c90e7-1113">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1113">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="c90e7-1114">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="c90e7-1114">Updated create policy definition help example</span></span>
- <span data-ttu-id="c90e7-1115">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1115">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="c90e7-1116">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1116">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="c90e7-1117">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1117">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-1118">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-1118">Az.Sql</span></span>
* <span data-ttu-id="c90e7-1119">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1119">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="c90e7-1120">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="c90e7-1120">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="c90e7-1121">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-1121">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="c90e7-1122">Geral</span><span class="sxs-lookup"><span data-stu-id="c90e7-1122">General</span></span>
* <span data-ttu-id="c90e7-1123">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-1123">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c90e7-1124">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-1124">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-1125">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1125">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="c90e7-1126">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="c90e7-1126">Az.Advisor</span></span>
* <span data-ttu-id="c90e7-1127">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1127">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c90e7-1128">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c90e7-1128">Az.Batch</span></span>
* <span data-ttu-id="c90e7-1129">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1129">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="c90e7-1130">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1130">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="c90e7-1131">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1131">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="c90e7-1132">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1132">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="c90e7-1133">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1133">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="c90e7-1134">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1134">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="c90e7-1135">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1135">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="c90e7-1136">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1136">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="c90e7-1137">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1137">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="c90e7-1138">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1138">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="c90e7-1139">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1139">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="c90e7-1140">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1140">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="c90e7-1141">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1141">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="c90e7-1142">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1142">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="c90e7-1143">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1143">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="c90e7-1144">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1144">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="c90e7-1145">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1145">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="c90e7-1146">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1146">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="c90e7-1147">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1147">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="c90e7-1148">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1148">This operation is no longer supported.</span></span>
* <span data-ttu-id="c90e7-1149">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1149">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="c90e7-1150">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1150">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="c90e7-1151">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1151">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="c90e7-1152">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1152">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="c90e7-1153">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1153">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="c90e7-1154">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1154">New non-verified images are also now returned.</span></span> <span data-ttu-id="c90e7-1155">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1155">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="c90e7-1156">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1156">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="c90e7-1157">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1157">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="c90e7-1158">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1158">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="c90e7-1159">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1159">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="c90e7-1160">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1160">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="c90e7-1161">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1161">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="c90e7-1162">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1162">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="c90e7-1163">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="c90e7-1163">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="c90e7-1164">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="c90e7-1164">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c90e7-1165">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c90e7-1165">Az.Cdn</span></span>
* <span data-ttu-id="c90e7-1166">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1166">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="c90e7-1167">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1167">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-1168">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-1168">Az.Compute</span></span>
* <span data-ttu-id="c90e7-1169">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="c90e7-1169">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="c90e7-1170">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-1170">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="c90e7-1171">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="c90e7-1171">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="c90e7-1172">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1172">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="c90e7-1173">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1173">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="c90e7-1174">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="c90e7-1174">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="c90e7-1175">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c90e7-1175">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="c90e7-1176">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="c90e7-1176">Breaking changes</span></span>
    - <span data-ttu-id="c90e7-1177">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="c90e7-1177">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="c90e7-1178">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="c90e7-1178">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-1179">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-1179">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-1180">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-1180">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c90e7-1181">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c90e7-1181">Az.DataLakeStore</span></span>
* <span data-ttu-id="c90e7-1182">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="c90e7-1182">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="c90e7-1183">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1183">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="c90e7-1184">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="c90e7-1184">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="c90e7-1185">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="c90e7-1185">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="c90e7-1186">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="c90e7-1186">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="c90e7-1187">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="c90e7-1187">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c90e7-1188">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c90e7-1188">Az.FrontDoor</span></span>
* <span data-ttu-id="c90e7-1189">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="c90e7-1189">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c90e7-1190">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c90e7-1190">Az.HDInsight</span></span>
* <span data-ttu-id="c90e7-1191">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1191">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="c90e7-1192">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1192">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="c90e7-1193">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-1193">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="c90e7-1194">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1194">Removed five cmdlets:</span></span>
    - <span data-ttu-id="c90e7-1195">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="c90e7-1195">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="c90e7-1196">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="c90e7-1196">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="c90e7-1197">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="c90e7-1197">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="c90e7-1198">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c90e7-1198">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="c90e7-1199">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c90e7-1199">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="c90e7-1200">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1200">Added three cmdlets:</span></span>
    - <span data-ttu-id="c90e7-1201">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1201">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="c90e7-1202">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1202">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="c90e7-1203">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1203">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="c90e7-1204">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1204">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="c90e7-1205">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1205">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="c90e7-1206">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1206">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="c90e7-1207">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1207">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="c90e7-1208">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1208">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="c90e7-1209">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1209">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="c90e7-1210">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1210">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="c90e7-1211">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1211">Added some scenario test cases.</span></span>
* <span data-ttu-id="c90e7-1212">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1212">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c90e7-1213">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-1213">Az.IotHub</span></span>
* <span data-ttu-id="c90e7-1214">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1214">Breaking changes:</span></span>
    - <span data-ttu-id="c90e7-1215">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1215">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="c90e7-1216">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1216">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="c90e7-1217">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1217">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="c90e7-1218">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1218">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="c90e7-1219">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1219">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="c90e7-1220">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1220">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="c90e7-1221">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1221">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="c90e7-1222">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1222">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="c90e7-1223">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1223">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="c90e7-1224">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1224">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="c90e7-1225">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1225">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="c90e7-1226">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1226">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-1227">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-1227">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-1228">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1228">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="c90e7-1229">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1229">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="c90e7-1230">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1230">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="c90e7-1231">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1231">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="c90e7-1232">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1232">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="c90e7-1233">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1233">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="c90e7-1234">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1234">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="c90e7-1235">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1235">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="c90e7-1236">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="c90e7-1236">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-1237">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-1237">Az.Resources</span></span>
* <span data-ttu-id="c90e7-1238">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="c90e7-1238">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-1239">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-1239">Az.Network</span></span>
* <span data-ttu-id="c90e7-1240">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1240">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="c90e7-1241">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1241">Updated cmdlet:</span></span>
        - <span data-ttu-id="c90e7-1242">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1242">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c90e7-1243">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1243">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c90e7-1244">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1244">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c90e7-1245">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1245">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c90e7-1246">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1246">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="c90e7-1247">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1247">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="c90e7-1248">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1248">New cmdlet:</span></span>
        - <span data-ttu-id="c90e7-1249">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="c90e7-1249">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="c90e7-1250">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1250">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="c90e7-1251">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c90e7-1251">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="c90e7-1252">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1252">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="c90e7-1253">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1253">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="c90e7-1254">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1254">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="c90e7-1255">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-1255">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="c90e7-1256">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-1256">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="c90e7-1257">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1257">New cmdlets added:</span></span>
        - <span data-ttu-id="c90e7-1258">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="c90e7-1258">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="c90e7-1259">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="c90e7-1259">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="c90e7-1260">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="c90e7-1260">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="c90e7-1261">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="c90e7-1261">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="c90e7-1262">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-1262">Set-AzVirtualHub</span></span>
* <span data-ttu-id="c90e7-1263">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="c90e7-1263">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="c90e7-1264">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1264">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="c90e7-1265">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="c90e7-1265">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="c90e7-1266">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="c90e7-1266">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="c90e7-1267">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="c90e7-1267">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="c90e7-1268">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="c90e7-1268">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="c90e7-1269">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1269">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="c90e7-1270">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1270">New cmdlets added:</span></span>
        - <span data-ttu-id="c90e7-1271">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1271">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="c90e7-1272">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1272">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="c90e7-1273">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="c90e7-1273">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="c90e7-1274">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="c90e7-1274">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="c90e7-1275">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="c90e7-1275">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="c90e7-1276">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="c90e7-1276">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="c90e7-1277">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="c90e7-1277">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="c90e7-1278">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="c90e7-1278">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="c90e7-1279">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1279">New cmdlets added:</span></span>
        - <span data-ttu-id="c90e7-1280">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="c90e7-1280">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="c90e7-1281">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="c90e7-1281">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="c90e7-1282">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="c90e7-1282">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="c90e7-1283">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="c90e7-1283">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="c90e7-1284">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="c90e7-1284">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="c90e7-1285">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-1285">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="c90e7-1286">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1286">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="c90e7-1287">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="c90e7-1287">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="c90e7-1288">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="c90e7-1288">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="c90e7-1289">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="c90e7-1289">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="c90e7-1290">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="c90e7-1290">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="c90e7-1291">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1291">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="c90e7-1292">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="c90e7-1292">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="c90e7-1293">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="c90e7-1293">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="c90e7-1294">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="c90e7-1294">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="c90e7-1295">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="c90e7-1295">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="c90e7-1296">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="c90e7-1296">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="c90e7-1297">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1297">New cmdlets added:</span></span>
        - <span data-ttu-id="c90e7-1298">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="c90e7-1298">New-AzIpGroup</span></span>
        - <span data-ttu-id="c90e7-1299">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="c90e7-1299">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="c90e7-1300">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="c90e7-1300">Get-AzIpGroup</span></span>
        - <span data-ttu-id="c90e7-1301">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="c90e7-1301">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c90e7-1302">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c90e7-1302">Az.ServiceFabric</span></span>
* <span data-ttu-id="c90e7-1303">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1303">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-1304">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-1304">Az.Sql</span></span>
* <span data-ttu-id="c90e7-1305">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1305">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="c90e7-1306">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1306">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="c90e7-1307">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1307">Removed deprecated aliases:</span></span>
* <span data-ttu-id="c90e7-1308">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="c90e7-1308">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="c90e7-1309">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="c90e7-1309">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="c90e7-1310">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c90e7-1310">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="c90e7-1311">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="c90e7-1311">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="c90e7-1312">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="c90e7-1312">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="c90e7-1313">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1313">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-1314">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-1314">Az.Storage</span></span>
* <span data-ttu-id="c90e7-1315">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="c90e7-1315">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="c90e7-1316">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-1316">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="c90e7-1317">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-1317">Set-AzStorageAccount</span></span>
* <span data-ttu-id="c90e7-1318">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="c90e7-1318">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="c90e7-1319">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="c90e7-1319">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="c90e7-1320">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="c90e7-1320">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="c90e7-1321">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-1321">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="c90e7-1322">Geral</span><span class="sxs-lookup"><span data-stu-id="c90e7-1322">General</span></span>
* <span data-ttu-id="c90e7-1323">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-1323">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c90e7-1324">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-1324">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-1325">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1325">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c90e7-1326">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c90e7-1326">Az.ApiManagement</span></span>
* <span data-ttu-id="c90e7-1327">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-1327">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="c90e7-1328">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="c90e7-1328">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c90e7-1329">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-1329">Az.Automation</span></span>
* <span data-ttu-id="c90e7-1330">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1330">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c90e7-1331">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c90e7-1331">Az.Batch</span></span>
* <span data-ttu-id="c90e7-1332">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1332">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-1333">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-1333">Az.Compute</span></span>
* <span data-ttu-id="c90e7-1334">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c90e7-1334">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="c90e7-1335">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="c90e7-1335">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="c90e7-1336">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1336">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="c90e7-1337">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1337">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-1338">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-1338">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-1339">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1339">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="c90e7-1340">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1340">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="c90e7-1341">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-1341">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c90e7-1342">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c90e7-1342">Az.DataLakeStore</span></span>
* <span data-ttu-id="c90e7-1343">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="c90e7-1343">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="c90e7-1344">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="c90e7-1344">Az.HealthcareApis</span></span>
* <span data-ttu-id="c90e7-1345">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-1345">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="c90e7-1346">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="c90e7-1346">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="c90e7-1347">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="c90e7-1347">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="c90e7-1348">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1348">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c90e7-1349">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-1349">Az.IotHub</span></span>
* <span data-ttu-id="c90e7-1350">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="c90e7-1350">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="c90e7-1351">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="c90e7-1351">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c90e7-1352">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-1352">Az.Monitor</span></span>
* <span data-ttu-id="c90e7-1353">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="c90e7-1353">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="c90e7-1354">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1354">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="c90e7-1355">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="c90e7-1355">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="c90e7-1356">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1356">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-1357">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-1357">Az.Network</span></span>
* <span data-ttu-id="c90e7-1358">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1358">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="c90e7-1359">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="c90e7-1359">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="c90e7-1360">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1360">New cmdlets added:</span></span>
        - <span data-ttu-id="c90e7-1361">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="c90e7-1361">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="c90e7-1362">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1362">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="c90e7-1363">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="c90e7-1363">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="c90e7-1364">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1364">Updated cmdlets:</span></span>
        - <span data-ttu-id="c90e7-1365">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1365">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="c90e7-1366">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1366">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="c90e7-1367">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1367">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="c90e7-1368">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="c90e7-1368">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="c90e7-1369">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="c90e7-1369">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="c90e7-1370">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1370">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="c90e7-1371">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1371">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="c90e7-1372">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c90e7-1372">Az.RedisCache</span></span>
* <span data-ttu-id="c90e7-1373">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1373">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-1374">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-1374">Az.Sql</span></span>
* <span data-ttu-id="c90e7-1375">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="c90e7-1375">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-1376">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-1376">Az.Storage</span></span>
* <span data-ttu-id="c90e7-1377">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-1377">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="c90e7-1378">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="c90e7-1378">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="c90e7-1379">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="c90e7-1379">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="c90e7-1380">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="c90e7-1380">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="c90e7-1381">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-1381">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="c90e7-1382">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="c90e7-1382">Az.StorageSync</span></span>
* <span data-ttu-id="c90e7-1383">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1383">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-1384">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-1384">Az.Websites</span></span>
* <span data-ttu-id="c90e7-1385">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="c90e7-1385">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="c90e7-1386">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-1386">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="c90e7-1387">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c90e7-1387">Az.ApiManagement</span></span>
* <span data-ttu-id="c90e7-1388">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1388">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="c90e7-1389">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1389">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="c90e7-1390">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1390">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c90e7-1391">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-1391">Az.Automation</span></span>
* <span data-ttu-id="c90e7-1392">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1392">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="c90e7-1393">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="c90e7-1393">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="c90e7-1394">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1394">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-1395">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-1395">Az.Compute</span></span>
* <span data-ttu-id="c90e7-1396">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1396">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="c90e7-1397">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1397">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="c90e7-1398">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1398">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="c90e7-1399">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1399">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="c90e7-1400">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1400">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="c90e7-1401">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1401">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="c90e7-1402">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1402">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="c90e7-1403">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1403">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="c90e7-1404">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1404">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-1405">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-1405">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-1406">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="c90e7-1406">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="c90e7-1407">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="c90e7-1407">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c90e7-1408">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c90e7-1408">Az.HDInsight</span></span>
* <span data-ttu-id="c90e7-1409">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="c90e7-1409">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c90e7-1410">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-1410">Az.IotHub</span></span>
* <span data-ttu-id="c90e7-1411">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1411">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="c90e7-1412">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1412">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="c90e7-1413">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1413">New cmdlets are:</span></span>
    - <span data-ttu-id="c90e7-1414">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="c90e7-1414">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="c90e7-1415">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="c90e7-1415">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="c90e7-1416">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="c90e7-1416">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="c90e7-1417">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="c90e7-1417">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c90e7-1418">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-1418">Az.Monitor</span></span>
* <span data-ttu-id="c90e7-1419">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="c90e7-1419">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="c90e7-1420">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1420">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="c90e7-1421">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1421">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="c90e7-1422">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1422">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="c90e7-1423">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1423">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="c90e7-1424">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1424">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="c90e7-1425">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1425">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="c90e7-1426">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1426">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="c90e7-1427">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1427">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="c90e7-1428">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1428">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="c90e7-1429">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1429">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="c90e7-1430">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1430">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="c90e7-1431">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="c90e7-1431">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="c90e7-1432">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="c90e7-1432">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="c90e7-1433">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="c90e7-1433">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="c90e7-1434">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="c90e7-1434">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="c90e7-1435">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="c90e7-1435">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="c90e7-1436">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="c90e7-1436">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="c90e7-1437">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1437">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="c90e7-1438">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="c90e7-1438">Overall improved help files</span></span>
* <span data-ttu-id="c90e7-1439">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1439">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-1440">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-1440">Az.Network</span></span>
* <span data-ttu-id="c90e7-1441">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1441">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="c90e7-1442">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="c90e7-1442">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="c90e7-1443">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="c90e7-1443">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="c90e7-1444">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="c90e7-1444">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="c90e7-1445">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="c90e7-1445">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="c90e7-1446">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="c90e7-1446">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="c90e7-1447">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="c90e7-1447">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="c90e7-1448">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="c90e7-1448">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="c90e7-1449">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="c90e7-1449">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="c90e7-1450">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="c90e7-1450">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="c90e7-1451">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="c90e7-1451">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="c90e7-1452">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="c90e7-1452">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="c90e7-1453">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="c90e7-1453">New cmdlets</span></span>
        - <span data-ttu-id="c90e7-1454">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="c90e7-1454">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="c90e7-1455">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1455">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="c90e7-1456">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1456">Updated cmdlet:</span></span>
        - <span data-ttu-id="c90e7-1457">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="c90e7-1457">New-VpnSite</span></span>
        - <span data-ttu-id="c90e7-1458">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="c90e7-1458">Update-VpnSite</span></span>
        - <span data-ttu-id="c90e7-1459">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1459">New-VpnConnection</span></span>
        - <span data-ttu-id="c90e7-1460">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1460">Update-VpnConnection</span></span>
* <span data-ttu-id="c90e7-1461">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="c90e7-1461">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-1462">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-1462">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-1463">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="c90e7-1463">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="c90e7-1464">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="c90e7-1464">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-1465">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-1465">Az.Resources</span></span>
* <span data-ttu-id="c90e7-1466">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1466">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c90e7-1467">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c90e7-1467">Az.ServiceFabric</span></span>
* <span data-ttu-id="c90e7-1468">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1468">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="c90e7-1469">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1469">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="c90e7-1470">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="c90e7-1470">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="c90e7-1471">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="c90e7-1471">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="c90e7-1472">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="c90e7-1472">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="c90e7-1473">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="c90e7-1473">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="c90e7-1474">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="c90e7-1474">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="c90e7-1475">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="c90e7-1475">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="c90e7-1476">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="c90e7-1476">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="c90e7-1477">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="c90e7-1477">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="c90e7-1478">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="c90e7-1478">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="c90e7-1479">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="c90e7-1479">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="c90e7-1480">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="c90e7-1480">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="c90e7-1481">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="c90e7-1481">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="c90e7-1482">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="c90e7-1482">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="c90e7-1483">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1483">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="c90e7-1484">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="c90e7-1484">Az.SignalR</span></span>
* <span data-ttu-id="c90e7-1485">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="c90e7-1485">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-1486">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-1486">Az.Sql</span></span>
* <span data-ttu-id="c90e7-1487">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1487">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="c90e7-1488">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="c90e7-1488">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="c90e7-1489">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c90e7-1489">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="c90e7-1490">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1490">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="c90e7-1491">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="c90e7-1491">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-1492">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-1492">Az.Storage</span></span>
* <span data-ttu-id="c90e7-1493">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1493">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="c90e7-1494">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="c90e7-1494">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="c90e7-1495">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c90e7-1495">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="c90e7-1496">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c90e7-1496">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="c90e7-1497">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1497">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="c90e7-1498">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c90e7-1498">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="c90e7-1499">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="c90e7-1499">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="c90e7-1500">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c90e7-1500">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="c90e7-1501">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c90e7-1501">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="c90e7-1502">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c90e7-1502">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="c90e7-1503">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c90e7-1503">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-1504">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-1504">Az.Websites</span></span>
* <span data-ttu-id="c90e7-1505">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="c90e7-1505">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="c90e7-1506">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="c90e7-1506">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="c90e7-1507">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1507">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="c90e7-1508">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-1508">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="c90e7-1509">Geral</span><span class="sxs-lookup"><span data-stu-id="c90e7-1509">General</span></span>
* <span data-ttu-id="c90e7-1510">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="c90e7-1510">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c90e7-1511">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-1511">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-1512">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="c90e7-1512">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="c90e7-1513">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="c90e7-1513">Az.Aks</span></span>
* <span data-ttu-id="c90e7-1514">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1514">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="c90e7-1515">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="c90e7-1515">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c90e7-1516">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c90e7-1516">Az.ApiManagement</span></span>
* <span data-ttu-id="c90e7-1517">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="c90e7-1517">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="c90e7-1518">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="c90e7-1518">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="c90e7-1519">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1519">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="c90e7-1520">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="c90e7-1520">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="c90e7-1521">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1521">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c90e7-1522">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c90e7-1522">Az.Batch</span></span>
* <span data-ttu-id="c90e7-1523">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="c90e7-1523">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c90e7-1524">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c90e7-1524">Az.Cdn</span></span>
* <span data-ttu-id="c90e7-1525">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="c90e7-1525">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-1526">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-1526">Az.Compute</span></span>
* <span data-ttu-id="c90e7-1527">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1527">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="c90e7-1528">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c90e7-1528">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="c90e7-1529">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="c90e7-1529">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="c90e7-1530">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="c90e7-1530">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="c90e7-1531">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="c90e7-1531">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="c90e7-1532">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="c90e7-1532">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="c90e7-1533">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="c90e7-1533">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="c90e7-1534">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1534">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-1535">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-1535">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-1536">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1536">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="c90e7-1537">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="c90e7-1537">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="c90e7-1538">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="c90e7-1538">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="c90e7-1539">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="c90e7-1539">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c90e7-1540">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c90e7-1540">Az.DataLakeStore</span></span>
* <span data-ttu-id="c90e7-1541">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1541">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c90e7-1542">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-1542">Az.EventHub</span></span>
* <span data-ttu-id="c90e7-1543">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-1543">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="c90e7-1544">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="c90e7-1544">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="c90e7-1545">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="c90e7-1545">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="c90e7-1546">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="c90e7-1546">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="c90e7-1547">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="c90e7-1547">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="c90e7-1548">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="c90e7-1548">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c90e7-1549">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-1549">Az.Monitor</span></span>
* <span data-ttu-id="c90e7-1550">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="c90e7-1550">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-1551">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-1551">Az.Network</span></span>
* <span data-ttu-id="c90e7-1552">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="c90e7-1552">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="c90e7-1553">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1553">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="c90e7-1554">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1554">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="c90e7-1555">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="c90e7-1555">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="c90e7-1556">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1556">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="c90e7-1557">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1557">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="c90e7-1558">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="c90e7-1558">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c90e7-1559">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-1559">Az.OperationalInsights</span></span>
* <span data-ttu-id="c90e7-1560">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1560">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="c90e7-1561">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="c90e7-1561">Added example</span></span>
    - <span data-ttu-id="c90e7-1562">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1562">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="c90e7-1563">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="c90e7-1563">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="c90e7-1564">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="c90e7-1564">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-1565">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-1565">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-1566">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1566">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-1567">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-1567">Az.Resources</span></span>
* <span data-ttu-id="c90e7-1568">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="c90e7-1568">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="c90e7-1569">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="c90e7-1569">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="c90e7-1570">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="c90e7-1570">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="c90e7-1571">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="c90e7-1571">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c90e7-1572">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c90e7-1572">Az.ServiceBus</span></span>
* <span data-ttu-id="c90e7-1573">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-1573">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="c90e7-1574">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="c90e7-1574">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="c90e7-1575">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="c90e7-1575">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c90e7-1576">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c90e7-1576">Az.ServiceFabric</span></span>
* <span data-ttu-id="c90e7-1577">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1577">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="c90e7-1578">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1578">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="c90e7-1579">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="c90e7-1579">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="c90e7-1580">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1580">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="c90e7-1581">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="c90e7-1581">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="c90e7-1582">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="c90e7-1582">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-1583">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-1583">Az.Sql</span></span>
* <span data-ttu-id="c90e7-1584">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1584">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-1585">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-1585">Az.Storage</span></span>
* <span data-ttu-id="c90e7-1586">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="c90e7-1586">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="c90e7-1587">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="c90e7-1587">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="c90e7-1588">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c90e7-1588">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="c90e7-1589">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="c90e7-1589">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="c90e7-1590">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="c90e7-1590">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="c90e7-1591">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="c90e7-1591">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-1592">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-1592">Az.Websites</span></span>
* <span data-ttu-id="c90e7-1593">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="c90e7-1593">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="c90e7-1594">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-1594">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c90e7-1595">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-1595">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-1596">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="c90e7-1596">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="c90e7-1597">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-1597">Az.ApplicationInsights</span></span>
* <span data-ttu-id="c90e7-1598">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1598">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c90e7-1599">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-1599">Az.Automation</span></span>
* <span data-ttu-id="c90e7-1600">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="c90e7-1600">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c90e7-1601">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-1601">Az.CognitiveServices</span></span>
* <span data-ttu-id="c90e7-1602">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1602">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-1603">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-1603">Az.Compute</span></span>
* <span data-ttu-id="c90e7-1604">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1604">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="c90e7-1605">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="c90e7-1605">Az.ContainerRegistry</span></span>
* <span data-ttu-id="c90e7-1606">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="c90e7-1606">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="c90e7-1607">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="c90e7-1607">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-1608">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-1608">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-1609">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-1609">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="c90e7-1610">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1610">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c90e7-1611">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-1611">Az.EventHub</span></span>
* <span data-ttu-id="c90e7-1612">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="c90e7-1612">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="c90e7-1613">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="c90e7-1613">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c90e7-1614">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c90e7-1614">Az.KeyVault</span></span>
* <span data-ttu-id="c90e7-1615">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="c90e7-1615">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="c90e7-1616">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c90e7-1616">Az.LogicApp</span></span>
* <span data-ttu-id="c90e7-1617">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="c90e7-1617">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="c90e7-1618">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="c90e7-1618">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="c90e7-1619">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-1619">Az.ManagedServices</span></span>
* <span data-ttu-id="c90e7-1620">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="c90e7-1620">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-1621">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-1621">Az.Network</span></span>
* <span data-ttu-id="c90e7-1622">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="c90e7-1622">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="c90e7-1623">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="c90e7-1623">New cmdlets</span></span>
        - <span data-ttu-id="c90e7-1624">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="c90e7-1624">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="c90e7-1625">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c90e7-1625">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="c90e7-1626">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1626">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c90e7-1627">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1627">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c90e7-1628">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1628">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c90e7-1629">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1629">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c90e7-1630">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="c90e7-1630">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="c90e7-1631">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c90e7-1631">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="c90e7-1632">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="c90e7-1632">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="c90e7-1633">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1633">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="c90e7-1634">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1634">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="c90e7-1635">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1635">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="c90e7-1636">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="c90e7-1636">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="c90e7-1637">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="c90e7-1637">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="c90e7-1638">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="c90e7-1638">Updated cmdlets</span></span>
        - <span data-ttu-id="c90e7-1639">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1639">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="c90e7-1640">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1640">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="c90e7-1641">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1641">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="c90e7-1642">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1642">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="c90e7-1643">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="c90e7-1643">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="c90e7-1644">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1644">Updated cmdlet:</span></span>
        - <span data-ttu-id="c90e7-1645">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1645">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="c90e7-1646">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1646">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="c90e7-1647">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1647">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="c90e7-1648">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="c90e7-1648">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="c90e7-1649">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1649">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="c90e7-1650">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1650">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c90e7-1651">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-1651">Az.OperationalInsights</span></span>
* <span data-ttu-id="c90e7-1652">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1652">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="c90e7-1653">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="c90e7-1653">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-1654">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-1654">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-1655">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1655">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="c90e7-1656">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1656">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="c90e7-1657">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1657">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="c90e7-1658">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1658">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="c90e7-1659">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1659">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="c90e7-1660">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1660">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="c90e7-1661">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1661">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="c90e7-1662">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1662">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="c90e7-1663">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-1663">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="c90e7-1664">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1664">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-1665">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-1665">Az.Resources</span></span>
- <span data-ttu-id="c90e7-1666">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1666">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="c90e7-1667">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="c90e7-1667">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c90e7-1668">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c90e7-1668">Az.ServiceBus</span></span>
* <span data-ttu-id="c90e7-1669">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="c90e7-1669">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="c90e7-1670">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="c90e7-1670">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-1671">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-1671">Az.Sql</span></span>
* <span data-ttu-id="c90e7-1672">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="c90e7-1672">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="c90e7-1673">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="c90e7-1673">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="c90e7-1674">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1674">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-1675">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-1675">Az.Storage</span></span>
* <span data-ttu-id="c90e7-1676">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="c90e7-1676">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="c90e7-1677">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="c90e7-1677">Az.StorageSync</span></span>
* <span data-ttu-id="c90e7-1678">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1678">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="c90e7-1679">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="c90e7-1679">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-1680">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-1680">Az.Websites</span></span>
* <span data-ttu-id="c90e7-1681">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="c90e7-1681">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="c90e7-1682">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="c90e7-1682">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="c90e7-1683">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="c90e7-1683">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="c90e7-1684">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-1684">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c90e7-1685">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-1685">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-1686">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="c90e7-1686">Add support for profile cmdlets</span></span>
* <span data-ttu-id="c90e7-1687">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="c90e7-1687">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="c90e7-1688">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="c90e7-1688">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="c90e7-1689">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="c90e7-1689">Az.Advisor</span></span>
* <span data-ttu-id="c90e7-1690">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="c90e7-1690">GA release of Az.Advisor</span></span>
* <span data-ttu-id="c90e7-1691">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="c90e7-1691">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c90e7-1692">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c90e7-1692">Az.ApiManagement</span></span>
* <span data-ttu-id="c90e7-1693">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="c90e7-1693">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="c90e7-1694">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="c90e7-1694">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="c90e7-1695">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="c90e7-1695">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="c90e7-1696">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1696">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="c90e7-1697">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="c90e7-1697">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="c90e7-1698">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="c90e7-1698">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="c90e7-1699">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="c90e7-1699">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c90e7-1700">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-1700">Az.Automation</span></span>
* <span data-ttu-id="c90e7-1701">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="c90e7-1701">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-1702">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-1702">Az.Compute</span></span>
* <span data-ttu-id="c90e7-1703">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1703">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-1704">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-1704">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-1705">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1705">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c90e7-1706">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c90e7-1706">Az.EventGrid</span></span>
* <span data-ttu-id="c90e7-1707">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1707">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c90e7-1708">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-1708">Az.IotHub</span></span>
* <span data-ttu-id="c90e7-1709">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1709">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-1710">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-1710">Az.Network</span></span>
* <span data-ttu-id="c90e7-1711">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="c90e7-1711">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="c90e7-1712">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1712">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c90e7-1713">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-1713">Az.PolicyInsights</span></span>
* <span data-ttu-id="c90e7-1714">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="c90e7-1714">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="c90e7-1715">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="c90e7-1715">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c90e7-1716">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-1716">Az.OperationalInsights</span></span>
* <span data-ttu-id="c90e7-1717">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="c90e7-1717">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-1718">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-1718">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-1719">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="c90e7-1719">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-1720">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-1720">Az.Resources</span></span>
    - <span data-ttu-id="c90e7-1721">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="c90e7-1721">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="c90e7-1722">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="c90e7-1722">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="c90e7-1723">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="c90e7-1723">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="c90e7-1724">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="c90e7-1724">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c90e7-1725">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c90e7-1725">Az.ServiceBus</span></span>
* <span data-ttu-id="c90e7-1726">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="c90e7-1726">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-1727">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-1727">Az.Sql</span></span>
* <span data-ttu-id="c90e7-1728">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="c90e7-1728">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="c90e7-1729">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1729">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="c90e7-1730">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="c90e7-1730">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="c90e7-1731">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="c90e7-1731">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="c90e7-1732">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="c90e7-1732">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="c90e7-1733">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="c90e7-1733">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="c90e7-1734">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="c90e7-1734">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="c90e7-1735">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="c90e7-1735">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="c90e7-1736">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="c90e7-1736">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-1737">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-1737">Az.Storage</span></span>
* <span data-ttu-id="c90e7-1738">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1738">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="c90e7-1739">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="c90e7-1739">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="c90e7-1740">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="c90e7-1740">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="c90e7-1741">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="c90e7-1741">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="c90e7-1742">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-1742">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="c90e7-1743">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-1743">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="c90e7-1744">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-1744">Set-AzStorageAccount</span></span>
* <span data-ttu-id="c90e7-1745">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="c90e7-1745">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="c90e7-1746">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="c90e7-1746">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="c90e7-1747">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="c90e7-1747">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="c90e7-1748">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="c90e7-1748">Az.StorageSync</span></span>
* <span data-ttu-id="c90e7-1749">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="c90e7-1749">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="c90e7-1750">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-1750">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c90e7-1751">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-1751">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-1752">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="c90e7-1752">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="c90e7-1753">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="c90e7-1753">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="c90e7-1754">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="c90e7-1754">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="c90e7-1755">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="c90e7-1755">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="c90e7-1756">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="c90e7-1756">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-1757">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-1757">Az.Compute</span></span>
* <span data-ttu-id="c90e7-1758">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1758">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="c90e7-1759">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1759">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="c90e7-1760">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="c90e7-1760">Az.Dns</span></span>
* <span data-ttu-id="c90e7-1761">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1761">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c90e7-1762">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c90e7-1762">Az.EventGrid</span></span>
* <span data-ttu-id="c90e7-1763">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1763">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="c90e7-1764">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1764">New cmdlets:</span></span>
    - <span data-ttu-id="c90e7-1765">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="c90e7-1765">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="c90e7-1766">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1766">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="c90e7-1767">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="c90e7-1767">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="c90e7-1768">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1768">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="c90e7-1769">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="c90e7-1769">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="c90e7-1770">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1770">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="c90e7-1771">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="c90e7-1771">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="c90e7-1772">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1772">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="c90e7-1773">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="c90e7-1773">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="c90e7-1774">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1774">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="c90e7-1775">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1775">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="c90e7-1776">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1776">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="c90e7-1777">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="c90e7-1777">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="c90e7-1778">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="c90e7-1778">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="c90e7-1779">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1779">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="c90e7-1780">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1780">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="c90e7-1781">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1781">Updated cmdlets:</span></span>
    - <span data-ttu-id="c90e7-1782">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1782">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="c90e7-1783">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1783">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="c90e7-1784">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1784">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="c90e7-1785">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="c90e7-1785">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="c90e7-1786">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1786">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="c90e7-1787">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="c90e7-1787">Event subscription expiration date,</span></span>
            - <span data-ttu-id="c90e7-1788">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1788">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="c90e7-1789">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1789">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="c90e7-1790">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="c90e7-1790">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="c90e7-1791">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1791">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="c90e7-1792">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1792">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="c90e7-1793">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="c90e7-1793">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="c90e7-1794">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1794">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="c90e7-1795">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1795">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c90e7-1796">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c90e7-1796">Az.FrontDoor</span></span>
* <span data-ttu-id="c90e7-1797">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="c90e7-1797">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="c90e7-1798">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="c90e7-1798">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="c90e7-1799">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="c90e7-1799">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="c90e7-1800">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="c90e7-1800">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-1801">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-1801">Az.Network</span></span>
* <span data-ttu-id="c90e7-1802">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="c90e7-1802">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="c90e7-1803">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="c90e7-1803">New cmdlets</span></span>
        - <span data-ttu-id="c90e7-1804">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="c90e7-1804">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="c90e7-1805">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="c90e7-1805">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="c90e7-1806">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="c90e7-1806">New cmdlets</span></span>
        - <span data-ttu-id="c90e7-1807">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="c90e7-1807">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="c90e7-1808">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c90e7-1808">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="c90e7-1809">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="c90e7-1809">New cmdlets</span></span>
        - <span data-ttu-id="c90e7-1810">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c90e7-1810">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="c90e7-1811">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c90e7-1811">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="c90e7-1812">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c90e7-1812">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="c90e7-1813">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-1813">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="c90e7-1814">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1814">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="c90e7-1815">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="c90e7-1815">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="c90e7-1816">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="c90e7-1816">New cmdlets</span></span>
        - <span data-ttu-id="c90e7-1817">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="c90e7-1817">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="c90e7-1818">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="c90e7-1818">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="c90e7-1819">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="c90e7-1819">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="c90e7-1820">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1820">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="c90e7-1821">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1821">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="c90e7-1822">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1822">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="c90e7-1823">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1823">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="c90e7-1824">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1824">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="c90e7-1825">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1825">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="c90e7-1826">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="c90e7-1826">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="c90e7-1827">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="c90e7-1827">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="c90e7-1828">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1828">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="c90e7-1829">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="c90e7-1829">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="c90e7-1830">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="c90e7-1830">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="c90e7-1831">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="c90e7-1831">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="c90e7-1832">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="c90e7-1832">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="c90e7-1833">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="c90e7-1833">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="c90e7-1834">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="c90e7-1834">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="c90e7-1835">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1835">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="c90e7-1836">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="c90e7-1836">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="c90e7-1837">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="c90e7-1837">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="c90e7-1838">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="c90e7-1838">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="c90e7-1839">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="c90e7-1839">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="c90e7-1840">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1840">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="c90e7-1841">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1841">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="c90e7-1842">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1842">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="c90e7-1843">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1843">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c90e7-1844">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-1844">Az.OperationalInsights</span></span>
* <span data-ttu-id="c90e7-1845">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1845">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-1846">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-1846">Az.Resources</span></span>
* <span data-ttu-id="c90e7-1847">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="c90e7-1847">Support for additional Template Export options</span></span>
    - <span data-ttu-id="c90e7-1848">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="c90e7-1848">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="c90e7-1849">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="c90e7-1849">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="c90e7-1850">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="c90e7-1850">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c90e7-1851">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c90e7-1851">Az.ServiceFabric</span></span>
* <span data-ttu-id="c90e7-1852">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="c90e7-1852">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-1853">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-1853">Az.Sql</span></span>
* <span data-ttu-id="c90e7-1854">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1854">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="c90e7-1855">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1855">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="c90e7-1856">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="c90e7-1856">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="c90e7-1857">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="c90e7-1857">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="c90e7-1858">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="c90e7-1858">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="c90e7-1859">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="c90e7-1859">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="c90e7-1860">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="c90e7-1860">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="c90e7-1861">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="c90e7-1861">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-1862">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-1862">Az.Storage</span></span>
* <span data-ttu-id="c90e7-1863">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="c90e7-1863">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="c90e7-1864">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-1864">New-AzStorageAccount</span></span>
* <span data-ttu-id="c90e7-1865">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="c90e7-1865">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="c90e7-1866">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="c90e7-1866">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-1867">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-1867">Az.Websites</span></span>
* <span data-ttu-id="c90e7-1868">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="c90e7-1868">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="c90e7-1869">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="c90e7-1869">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="c90e7-1870">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-1870">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="c90e7-1871">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c90e7-1871">Az.Cdn</span></span>
* <span data-ttu-id="c90e7-1872">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1872">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-1873">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-1873">Az.Compute</span></span>
* <span data-ttu-id="c90e7-1874">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1874">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="c90e7-1875">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="c90e7-1875">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c90e7-1876">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-1876">Az.EventHub</span></span>
* <span data-ttu-id="c90e7-1877">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="c90e7-1877">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="c90e7-1878">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="c90e7-1878">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-1879">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-1879">Az.Network</span></span>
* <span data-ttu-id="c90e7-1880">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="c90e7-1880">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="c90e7-1881">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="c90e7-1881">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c90e7-1882">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-1882">Az.PolicyInsights</span></span>
* <span data-ttu-id="c90e7-1883">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="c90e7-1883">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-1884">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-1884">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-1885">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="c90e7-1885">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c90e7-1886">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c90e7-1886">Az.ServiceBus</span></span>
* <span data-ttu-id="c90e7-1887">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="c90e7-1887">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c90e7-1888">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c90e7-1888">Az.ServiceFabric</span></span>
* <span data-ttu-id="c90e7-1889">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1889">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="c90e7-1890">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c90e7-1890">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-1891">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-1891">Az.Sql</span></span>
* <span data-ttu-id="c90e7-1892">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1892">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="c90e7-1893">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c90e7-1893">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="c90e7-1894">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="c90e7-1894">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="c90e7-1895">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1895">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-1896">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-1896">Az.Websites</span></span>
* <span data-ttu-id="c90e7-1897">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="c90e7-1897">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="c90e7-1898">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-1898">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="c90e7-1899">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c90e7-1899">Az.ApiManagement</span></span>
* <span data-ttu-id="c90e7-1900">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="c90e7-1900">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="c90e7-1901">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="c90e7-1901">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="c90e7-1902">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="c90e7-1902">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="c90e7-1903">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="c90e7-1903">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="c90e7-1904">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1904">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="c90e7-1905">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="c90e7-1905">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="c90e7-1906">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="c90e7-1906">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="c90e7-1907">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="c90e7-1907">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="c90e7-1908">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c90e7-1908">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="c90e7-1909">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="c90e7-1909">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="c90e7-1910">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="c90e7-1910">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="c90e7-1911">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="c90e7-1911">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="c90e7-1912">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="c90e7-1912">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="c90e7-1913">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="c90e7-1913">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="c90e7-1914">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="c90e7-1914">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="c90e7-1915">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="c90e7-1915">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="c90e7-1916">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="c90e7-1916">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="c90e7-1917">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="c90e7-1917">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="c90e7-1918">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1918">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="c90e7-1919">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="c90e7-1919">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="c90e7-1920">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="c90e7-1920">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="c90e7-1921">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1921">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="c90e7-1922">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1922">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="c90e7-1923">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c90e7-1923">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="c90e7-1924">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1924">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="c90e7-1925">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1925">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="c90e7-1926">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1926">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="c90e7-1927">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1927">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="c90e7-1928">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1928">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="c90e7-1929">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="c90e7-1929">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="c90e7-1930">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="c90e7-1930">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="c90e7-1931">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="c90e7-1931">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="c90e7-1932">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1932">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="c90e7-1933">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="c90e7-1933">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="c90e7-1934">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1934">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="c90e7-1935">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="c90e7-1935">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="c90e7-1936">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1936">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="c90e7-1937">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1937">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="c90e7-1938">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1938">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="c90e7-1939">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="c90e7-1939">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="c90e7-1940">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1940">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="c90e7-1941">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1941">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="c90e7-1942">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1942">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="c90e7-1943">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1943">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="c90e7-1944">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="c90e7-1944">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="c90e7-1945">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1945">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="c90e7-1946">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1946">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="c90e7-1947">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1947">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="c90e7-1948">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="c90e7-1948">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="c90e7-1949">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="c90e7-1949">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="c90e7-1950">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1950">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="c90e7-1951">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1951">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="c90e7-1952">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1952">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="c90e7-1953">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="c90e7-1953">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="c90e7-1954">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1954">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="c90e7-1955">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1955">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="c90e7-1956">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="c90e7-1956">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="c90e7-1957">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1957">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="c90e7-1958">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1958">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="c90e7-1959">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1959">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="c90e7-1960">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="c90e7-1960">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="c90e7-1961">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1961">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="c90e7-1962">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1962">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="c90e7-1963">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1963">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="c90e7-1964">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="c90e7-1964">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="c90e7-1965">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1965">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="c90e7-1966">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="c90e7-1966">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="c90e7-1967">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1967">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="c90e7-1968">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="c90e7-1968">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="c90e7-1969">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1969">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="c90e7-1970">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="c90e7-1970">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="c90e7-1971">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1971">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="c90e7-1972">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1972">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="c90e7-1973">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="c90e7-1973">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="c90e7-1974">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1974">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="c90e7-1975">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1975">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="c90e7-1976">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="c90e7-1976">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c90e7-1977">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-1977">Az.Automation</span></span>
* <span data-ttu-id="c90e7-1978">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1978">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="c90e7-1979">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="c90e7-1979">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="c90e7-1980">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="c90e7-1980">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="c90e7-1981">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1981">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="c90e7-1982">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="c90e7-1982">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="c90e7-1983">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1983">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="c90e7-1984">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1984">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-1985">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-1985">Az.Compute</span></span>
* <span data-ttu-id="c90e7-1986">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="c90e7-1986">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="c90e7-1987">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="c90e7-1987">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c90e7-1988">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c90e7-1988">Az.DataLakeStore</span></span>
* <span data-ttu-id="c90e7-1989">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-1989">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c90e7-1990">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-1990">Az.Monitor</span></span>
* <span data-ttu-id="c90e7-1991">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="c90e7-1991">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-1992">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-1992">Az.Network</span></span>
* <span data-ttu-id="c90e7-1993">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="c90e7-1993">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="c90e7-1994">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="c90e7-1994">Updated cmdlet:</span></span>
        - <span data-ttu-id="c90e7-1995">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="c90e7-1995">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="c90e7-1996">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="c90e7-1996">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-1997">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-1997">Az.Resources</span></span>
* <span data-ttu-id="c90e7-1998">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="c90e7-1998">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-1999">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-1999">Az.Sql</span></span>
* <span data-ttu-id="c90e7-2000">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="c90e7-2000">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="c90e7-2001">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-2001">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c90e7-2002">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-2002">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-2003">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="c90e7-2003">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c90e7-2004">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2004">Az.CognitiveServices</span></span>
* <span data-ttu-id="c90e7-2005">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2005">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="c90e7-2006">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2006">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-2007">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-2007">Az.Compute</span></span>
* <span data-ttu-id="c90e7-2008">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2008">Proximity placement group feature.</span></span>
    - <span data-ttu-id="c90e7-2009">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="c90e7-2009">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="c90e7-2010">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-2010">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="c90e7-2011">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2011">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="c90e7-2012">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2012">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="c90e7-2013">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c90e7-2013">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="c90e7-2014">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="c90e7-2014">Breaking changes</span></span>
    - <span data-ttu-id="c90e7-2015">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2015">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="c90e7-2016">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2016">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="c90e7-2017">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="c90e7-2017">Az.DeploymentManager</span></span>
* <span data-ttu-id="c90e7-2018">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-2018">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="c90e7-2019">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="c90e7-2019">Az.Dns</span></span>
* <span data-ttu-id="c90e7-2020">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="c90e7-2020">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="c90e7-2021">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2021">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="c90e7-2022">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2022">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c90e7-2023">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c90e7-2023">Az.FrontDoor</span></span>
* <span data-ttu-id="c90e7-2024">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="c90e7-2024">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="c90e7-2025">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="c90e7-2025">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="c90e7-2026">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c90e7-2026">Az.HDInsight</span></span>
* <span data-ttu-id="c90e7-2027">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c90e7-2027">Removed two cmdlets:</span></span>
    - <span data-ttu-id="c90e7-2028">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c90e7-2028">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="c90e7-2029">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c90e7-2029">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="c90e7-2030">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c90e7-2030">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="c90e7-2031">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="c90e7-2031">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="c90e7-2032">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2032">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="c90e7-2033">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2033">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c90e7-2034">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-2034">Az.Monitor</span></span>
* <span data-ttu-id="c90e7-2035">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="c90e7-2035">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="c90e7-2036">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="c90e7-2036">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="c90e7-2037">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="c90e7-2037">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="c90e7-2038">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="c90e7-2038">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="c90e7-2039">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="c90e7-2039">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="c90e7-2040">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="c90e7-2040">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="c90e7-2041">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="c90e7-2041">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="c90e7-2042">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c90e7-2042">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c90e7-2043">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c90e7-2043">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c90e7-2044">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c90e7-2044">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c90e7-2045">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c90e7-2045">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c90e7-2046">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c90e7-2046">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c90e7-2047">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="c90e7-2047">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="c90e7-2048">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="c90e7-2048">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-2049">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-2049">Az.Network</span></span>
* <span data-ttu-id="c90e7-2050">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="c90e7-2050">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="c90e7-2051">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="c90e7-2051">New cmdlets</span></span>
        - <span data-ttu-id="c90e7-2052">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c90e7-2052">New-AzNatGateway</span></span>
        - <span data-ttu-id="c90e7-2053">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c90e7-2053">Get-AzNatGateway</span></span>
        - <span data-ttu-id="c90e7-2054">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c90e7-2054">Set-AzNatGateway</span></span>
        - <span data-ttu-id="c90e7-2055">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c90e7-2055">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="c90e7-2056">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="c90e7-2056">Updated cmdlets</span></span>
        - <span data-ttu-id="c90e7-2057">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="c90e7-2057">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="c90e7-2058">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="c90e7-2058">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="c90e7-2059">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2059">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="c90e7-2060">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2060">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="c90e7-2061">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2061">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c90e7-2062">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-2062">Az.PolicyInsights</span></span>
* <span data-ttu-id="c90e7-2063">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2063">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="c90e7-2064">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2064">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="c90e7-2065">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="c90e7-2065">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-2066">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2066">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-2067">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2067">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="c90e7-2068">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2068">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="c90e7-2069">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2069">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="c90e7-2070">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2070">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="c90e7-2071">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2071">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="c90e7-2072">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2072">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="c90e7-2073">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="c90e7-2073">Az.Relay</span></span>
* <span data-ttu-id="c90e7-2074">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="c90e7-2074">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c90e7-2075">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c90e7-2075">Az.ServiceBus</span></span>
* <span data-ttu-id="c90e7-2076">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="c90e7-2076">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-2077">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-2077">Az.Storage</span></span>
* <span data-ttu-id="c90e7-2078">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="c90e7-2078">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="c90e7-2079">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2079">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="c90e7-2080">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="c90e7-2080">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="c90e7-2081">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-2081">New-AzStorageAccount</span></span>
* <span data-ttu-id="c90e7-2082">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="c90e7-2082">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="c90e7-2083">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-2083">New-AzStorageAccount</span></span>
    - <span data-ttu-id="c90e7-2084">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-2084">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="c90e7-2085">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-2085">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-2086">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-2086">Az.Websites</span></span>
* <span data-ttu-id="c90e7-2087">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="c90e7-2087">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="c90e7-2088">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="c90e7-2088">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="c90e7-2089">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-2089">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c90e7-2090">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="c90e7-2090">Highlights since the last major release</span></span>
* <span data-ttu-id="c90e7-2091">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="c90e7-2091">General availability of `Az` module</span></span>
* <span data-ttu-id="c90e7-2092">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="c90e7-2092">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="c90e7-2093">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="c90e7-2093">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="c90e7-2094">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-2094">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="c90e7-2095">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="c90e7-2095">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c90e7-2096">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-2096">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="c90e7-2097">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="c90e7-2097">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c90e7-2098">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-2098">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-2099">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="c90e7-2099">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c90e7-2100">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c90e7-2100">Az.Batch</span></span>
* <span data-ttu-id="c90e7-2101">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2101">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c90e7-2102">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c90e7-2102">Az.Cdn</span></span>
* <span data-ttu-id="c90e7-2103">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2103">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c90e7-2104">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2104">Az.CognitiveServices</span></span>
* <span data-ttu-id="c90e7-2105">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2105">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-2106">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-2106">Az.Compute</span></span>
* <span data-ttu-id="c90e7-2107">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="c90e7-2107">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="c90e7-2108">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2108">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c90e7-2109">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="c90e7-2109">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-2110">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-2110">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-2111">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2111">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c90e7-2112">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c90e7-2112">Az.DataLakeStore</span></span>
* <span data-ttu-id="c90e7-2113">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2113">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c90e7-2114">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c90e7-2114">Az.EventGrid</span></span>
* <span data-ttu-id="c90e7-2115">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2115">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c90e7-2116">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-2116">Az.EventHub</span></span>
* <span data-ttu-id="c90e7-2117">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="c90e7-2117">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c90e7-2118">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c90e7-2118">Az.HDInsight</span></span>
* <span data-ttu-id="c90e7-2119">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2119">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c90e7-2120">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-2120">Az.IotHub</span></span>
* <span data-ttu-id="c90e7-2121">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2121">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c90e7-2122">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c90e7-2122">Az.KeyVault</span></span>
* <span data-ttu-id="c90e7-2123">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2123">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c90e7-2124">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="c90e7-2124">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="c90e7-2125">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="c90e7-2125">Az.MachineLearning</span></span>
* <span data-ttu-id="c90e7-2126">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2126">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="c90e7-2127">Az.Media</span><span class="sxs-lookup"><span data-stu-id="c90e7-2127">Az.Media</span></span>
* <span data-ttu-id="c90e7-2128">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2128">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c90e7-2129">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-2129">Az.Monitor</span></span>
  * <span data-ttu-id="c90e7-2130">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="c90e7-2130">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="c90e7-2131">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="c90e7-2131">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="c90e7-2132">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="c90e7-2132">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="c90e7-2133">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="c90e7-2133">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="c90e7-2134">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="c90e7-2134">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="c90e7-2135">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="c90e7-2135">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="c90e7-2136">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="c90e7-2136">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-2137">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-2137">Az.Network</span></span>
* <span data-ttu-id="c90e7-2138">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2138">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c90e7-2139">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="c90e7-2139">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="c90e7-2140">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="c90e7-2140">Az.NotificationHubs</span></span>
* <span data-ttu-id="c90e7-2141">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2141">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c90e7-2142">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-2142">Az.OperationalInsights</span></span>
* <span data-ttu-id="c90e7-2143">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2143">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="c90e7-2144">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="c90e7-2144">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="c90e7-2145">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2145">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-2146">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2146">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-2147">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2147">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c90e7-2148">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-2148">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="c90e7-2149">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="c90e7-2149">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="c90e7-2150">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="c90e7-2150">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="c90e7-2151">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c90e7-2151">Az.RedisCache</span></span>
* <span data-ttu-id="c90e7-2152">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2152">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-2153">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-2153">Az.Resources</span></span>
* <span data-ttu-id="c90e7-2154">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="c90e7-2154">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-2155">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-2155">Az.Sql</span></span>
* <span data-ttu-id="c90e7-2156">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="c90e7-2156">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="c90e7-2157">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2157">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c90e7-2158">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2158">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="c90e7-2159">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2159">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="c90e7-2160">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2160">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="c90e7-2161">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2161">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="c90e7-2162">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="c90e7-2162">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-2163">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-2163">Az.Websites</span></span>
* <span data-ttu-id="c90e7-2164">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="c90e7-2164">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="c90e7-2165">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2165">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c90e7-2166">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2166">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="c90e7-2167">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2167">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="c90e7-2168">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-2168">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c90e7-2169">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="c90e7-2169">Highlights since the last major release</span></span>
* <span data-ttu-id="c90e7-2170">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="c90e7-2170">General availability of `Az` module</span></span>
* <span data-ttu-id="c90e7-2171">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="c90e7-2171">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="c90e7-2172">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="c90e7-2172">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="c90e7-2173">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-2173">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="c90e7-2174">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="c90e7-2174">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c90e7-2175">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-2175">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="c90e7-2176">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="c90e7-2176">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c90e7-2177">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-2177">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-2178">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="c90e7-2178">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c90e7-2179">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2179">Az.AnalysisServices</span></span>
* <span data-ttu-id="c90e7-2180">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="c90e7-2180">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="c90e7-2181">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="c90e7-2181">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c90e7-2182">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-2182">Az.Automation</span></span>
* <span data-ttu-id="c90e7-2183">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2183">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="c90e7-2184">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2184">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="c90e7-2185">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-2185">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-2186">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-2186">Az.Compute</span></span>
* <span data-ttu-id="c90e7-2187">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-2187">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="c90e7-2188">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2188">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="c90e7-2189">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c90e7-2189">Az.ContainerInstance</span></span>
* <span data-ttu-id="c90e7-2190">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="c90e7-2190">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-2191">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-2191">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-2192">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="c90e7-2192">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="c90e7-2193">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2193">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-2194">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-2194">Az.Resources</span></span>
* <span data-ttu-id="c90e7-2195">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="c90e7-2195">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="c90e7-2196">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="c90e7-2196">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="c90e7-2197">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="c90e7-2197">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="c90e7-2198">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="c90e7-2198">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="c90e7-2199">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="c90e7-2199">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="c90e7-2200">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="c90e7-2200">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-2201">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-2201">Az.Sql</span></span>
* <span data-ttu-id="c90e7-2202">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2202">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-2203">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-2203">Az.Storage</span></span>
* <span data-ttu-id="c90e7-2204">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-2204">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="c90e7-2205">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="c90e7-2205">New-AzStorageContext</span></span>
* <span data-ttu-id="c90e7-2206">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="c90e7-2206">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="c90e7-2207">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="c90e7-2207">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="c90e7-2208">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="c90e7-2208">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="c90e7-2209">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="c90e7-2209">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="c90e7-2210">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="c90e7-2210">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="c90e7-2211">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="c90e7-2211">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="c90e7-2212">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c90e7-2212">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="c90e7-2213">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c90e7-2213">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="c90e7-2214">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c90e7-2214">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="c90e7-2215">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c90e7-2215">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="c90e7-2216">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-2216">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c90e7-2217">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="c90e7-2217">Highlights since the last major release</span></span>
* <span data-ttu-id="c90e7-2218">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="c90e7-2218">General availability of `Az` module</span></span>
* <span data-ttu-id="c90e7-2219">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="c90e7-2219">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="c90e7-2220">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="c90e7-2220">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="c90e7-2221">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-2221">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="c90e7-2222">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="c90e7-2222">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c90e7-2223">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-2223">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="c90e7-2224">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="c90e7-2224">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c90e7-2225">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-2225">Az.Automation</span></span>
* <span data-ttu-id="c90e7-2226">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="c90e7-2226">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="c90e7-2227">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="c90e7-2227">Dynamic grouping</span></span>
    * <span data-ttu-id="c90e7-2228">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="c90e7-2228">Pre-Post script</span></span>
    * <span data-ttu-id="c90e7-2229">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="c90e7-2229">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-2230">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-2230">Az.Compute</span></span>
* <span data-ttu-id="c90e7-2231">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="c90e7-2231">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="c90e7-2232">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2232">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c90e7-2233">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c90e7-2233">Az.KeyVault</span></span>
* <span data-ttu-id="c90e7-2234">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="c90e7-2234">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-2235">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-2235">Az.Network</span></span>
* <span data-ttu-id="c90e7-2236">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="c90e7-2236">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="c90e7-2237">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="c90e7-2237">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-2238">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2238">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-2239">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="c90e7-2239">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="c90e7-2240">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="c90e7-2240">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-2241">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-2241">Az.Resources</span></span>
* <span data-ttu-id="c90e7-2242">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="c90e7-2242">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="c90e7-2243">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="c90e7-2243">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-2244">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-2244">Az.Sql</span></span>
* <span data-ttu-id="c90e7-2245">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2245">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-2246">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-2246">Az.Storage</span></span>
* <span data-ttu-id="c90e7-2247">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="c90e7-2247">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="c90e7-2248">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="c90e7-2248">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="c90e7-2249">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="c90e7-2249">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="c90e7-2250">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="c90e7-2250">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="c90e7-2251">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="c90e7-2251">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="c90e7-2252">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="c90e7-2252">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="c90e7-2253">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="c90e7-2253">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-2254">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-2254">Az.Websites</span></span>
* <span data-ttu-id="c90e7-2255">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="c90e7-2255">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="c90e7-2256">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-2256">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c90e7-2257">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-2257">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-2258">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="c90e7-2258">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="c90e7-2259">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-2259">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c90e7-2260">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-2260">Az.Automation</span></span>
* <span data-ttu-id="c90e7-2261">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-2261">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="c90e7-2262">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2262">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="c90e7-2263">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="c90e7-2263">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c90e7-2264">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c90e7-2264">Az.Cdn</span></span>
* <span data-ttu-id="c90e7-2265">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2265">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-2266">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-2266">Az.Compute</span></span>
* <span data-ttu-id="c90e7-2267">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="c90e7-2267">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-2268">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-2268">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-2269">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="c90e7-2269">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="c90e7-2270">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c90e7-2270">Az.LogicApp</span></span>
* <span data-ttu-id="c90e7-2271">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="c90e7-2271">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-2272">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-2272">Az.Network</span></span>
* <span data-ttu-id="c90e7-2273">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-2273">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-2274">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2274">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-2275">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-2275">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="c90e7-2276">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="c90e7-2276">SDK Update</span></span>
* <span data-ttu-id="c90e7-2277">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="c90e7-2277">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="c90e7-2278">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="c90e7-2278">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-2279">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-2279">Az.Resources</span></span>
* <span data-ttu-id="c90e7-2280">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="c90e7-2280">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="c90e7-2281">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="c90e7-2281">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="c90e7-2282">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="c90e7-2282">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="c90e7-2283">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="c90e7-2283">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="c90e7-2284">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="c90e7-2284">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="c90e7-2285">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="c90e7-2285">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-2286">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-2286">Az.Sql</span></span>
* <span data-ttu-id="c90e7-2287">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2287">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="c90e7-2288">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2288">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-2289">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-2289">Az.Storage</span></span>
* <span data-ttu-id="c90e7-2290">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-2290">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="c90e7-2291">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-2291">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="c90e7-2292">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2292">Az.AnalysisServices</span></span>
* <span data-ttu-id="c90e7-2293">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="c90e7-2293">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c90e7-2294">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-2294">Az.Automation</span></span>
* <span data-ttu-id="c90e7-2295">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="c90e7-2295">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="c90e7-2296">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="c90e7-2296">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="c90e7-2297">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="c90e7-2297">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c90e7-2298">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2298">Az.CognitiveServices</span></span>
* <span data-ttu-id="c90e7-2299">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2299">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-2300">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-2300">Az.Compute</span></span>
* <span data-ttu-id="c90e7-2301">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="c90e7-2301">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="c90e7-2302">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="c90e7-2302">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="c90e7-2303">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="c90e7-2303">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="c90e7-2304">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2304">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c90e7-2305">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c90e7-2305">Az.DataLakeStore</span></span>
* <span data-ttu-id="c90e7-2306">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="c90e7-2306">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c90e7-2307">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-2307">Az.EventHub</span></span>
* <span data-ttu-id="c90e7-2308">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="c90e7-2308">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c90e7-2309">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c90e7-2309">Az.KeyVault</span></span>
* <span data-ttu-id="c90e7-2310">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="c90e7-2310">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="c90e7-2311">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c90e7-2311">Az.LogicApp</span></span>
* <span data-ttu-id="c90e7-2312">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="c90e7-2312">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="c90e7-2313">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2313">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="c90e7-2314">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="c90e7-2314">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="c90e7-2315">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c90e7-2315">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="c90e7-2316">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c90e7-2316">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="c90e7-2317">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c90e7-2317">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="c90e7-2318">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c90e7-2318">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="c90e7-2319">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="c90e7-2319">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="c90e7-2320">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c90e7-2320">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="c90e7-2321">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c90e7-2321">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="c90e7-2322">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c90e7-2322">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="c90e7-2323">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c90e7-2323">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="c90e7-2324">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-2324">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c90e7-2325">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-2325">Az.Monitor</span></span>
* <span data-ttu-id="c90e7-2326">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="c90e7-2326">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-2327">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-2327">Az.Network</span></span>
* <span data-ttu-id="c90e7-2328">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="c90e7-2328">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c90e7-2329">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-2329">Az.OperationalInsights</span></span>
* <span data-ttu-id="c90e7-2330">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2330">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="c90e7-2331">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2331">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="c90e7-2332">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2332">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-2333">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-2333">Az.Resources</span></span>
* <span data-ttu-id="c90e7-2334">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="c90e7-2334">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="c90e7-2335">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="c90e7-2335">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="c90e7-2336">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="c90e7-2336">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="c90e7-2337">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="c90e7-2337">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-2338">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-2338">Az.Sql</span></span>
* <span data-ttu-id="c90e7-2339">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="c90e7-2339">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="c90e7-2340">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="c90e7-2340">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-2341">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-2341">Az.Websites</span></span>
* <span data-ttu-id="c90e7-2342">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="c90e7-2342">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="c90e7-2343">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-2343">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c90e7-2344">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-2344">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-2345">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="c90e7-2345">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c90e7-2346">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2346">Az.AnalysisServices</span></span>
<span data-ttu-id="c90e7-2347">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2347">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-2348">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-2348">Az.Compute</span></span>
* <span data-ttu-id="c90e7-2349">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="c90e7-2349">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="c90e7-2350">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="c90e7-2350">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="c90e7-2351">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="c90e7-2351">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-2352">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2352">Az.RecoveryServices</span></span>
<span data-ttu-id="c90e7-2353">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2353">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-2354">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-2354">Az.Resources</span></span>
* <span data-ttu-id="c90e7-2355">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="c90e7-2355">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="c90e7-2356">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="c90e7-2356">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="c90e7-2357">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="c90e7-2357">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="c90e7-2358">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="c90e7-2358">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-2359">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-2359">Az.Sql</span></span>
* <span data-ttu-id="c90e7-2360">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="c90e7-2360">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="c90e7-2361">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="c90e7-2361">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="c90e7-2362">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="c90e7-2362">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="c90e7-2363">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-2363">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c90e7-2364">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-2364">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-2365">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="c90e7-2365">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c90e7-2366">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2366">Az.AnalysisServices</span></span>
* <span data-ttu-id="c90e7-2367">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="c90e7-2367">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-2368">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2368">Az.RecoveryServices</span></span>
* <span data-ttu-id="c90e7-2369">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="c90e7-2369">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="c90e7-2370">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-2370">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c90e7-2371">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-2371">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-2372">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="c90e7-2372">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c90e7-2373">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2373">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c90e7-2374">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="c90e7-2374">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="c90e7-2375">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="c90e7-2375">Az.Aks</span></span>
* <span data-ttu-id="c90e7-2376">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2376">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c90e7-2377">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-2377">Az.Automation</span></span>
* <span data-ttu-id="c90e7-2378">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="c90e7-2378">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="c90e7-2379">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2379">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c90e7-2380">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c90e7-2380">Az.Cdn</span></span>
* <span data-ttu-id="c90e7-2381">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2381">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-2382">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-2382">Az.Compute</span></span>
* <span data-ttu-id="c90e7-2383">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="c90e7-2383">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="c90e7-2384">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c90e7-2384">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="c90e7-2385">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="c90e7-2385">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="c90e7-2386">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="c90e7-2386">Az.ContainerRegistry</span></span>
* <span data-ttu-id="c90e7-2387">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2387">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c90e7-2388">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c90e7-2388">Az.DataFactory</span></span>
* <span data-ttu-id="c90e7-2389">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="c90e7-2389">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c90e7-2390">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c90e7-2390">Az.DataLakeStore</span></span>
* <span data-ttu-id="c90e7-2391">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="c90e7-2391">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="c90e7-2392">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="c90e7-2392">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="c90e7-2393">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2393">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c90e7-2394">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-2394">Az.IotHub</span></span>
* <span data-ttu-id="c90e7-2395">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2395">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c90e7-2396">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c90e7-2396">Az.KeyVault</span></span>
* <span data-ttu-id="c90e7-2397">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2397">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-2398">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-2398">Az.Network</span></span>
* <span data-ttu-id="c90e7-2399">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2399">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-2400">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-2400">Az.Resources</span></span>
* <span data-ttu-id="c90e7-2401">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="c90e7-2401">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="c90e7-2402">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2402">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="c90e7-2403">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="c90e7-2403">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="c90e7-2404">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="c90e7-2404">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="c90e7-2405">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="c90e7-2405">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="c90e7-2406">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="c90e7-2406">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="c90e7-2407">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="c90e7-2407">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c90e7-2408">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c90e7-2408">Az.ServiceFabric</span></span>
* <span data-ttu-id="c90e7-2409">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="c90e7-2409">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="c90e7-2410">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2410">Fix some error messages.</span></span>
* <span data-ttu-id="c90e7-2411">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2411">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="c90e7-2412">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2412">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="c90e7-2413">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="c90e7-2413">Az.SignalR</span></span>
* <span data-ttu-id="c90e7-2414">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2414">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-2415">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-2415">Az.Sql</span></span>
* <span data-ttu-id="c90e7-2416">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2416">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c90e7-2417">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="c90e7-2417">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="c90e7-2418">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="c90e7-2418">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="c90e7-2419">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="c90e7-2419">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-2420">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-2420">Az.Storage</span></span>
* <span data-ttu-id="c90e7-2421">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2421">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c90e7-2422">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2422">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="c90e7-2423">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="c90e7-2423">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="c90e7-2424">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="c90e7-2424">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="c90e7-2425">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c90e7-2425">Az.TrafficManager</span></span>
* <span data-ttu-id="c90e7-2426">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2426">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-2427">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-2427">Az.Websites</span></span>
* <span data-ttu-id="c90e7-2428">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2428">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c90e7-2429">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2429">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="c90e7-2430">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="c90e7-2430">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="c90e7-2431">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="c90e7-2431">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c90e7-2432">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-2432">Az.Accounts</span></span>
* <span data-ttu-id="c90e7-2433">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="c90e7-2433">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-2434">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-2434">Az.Compute</span></span>
* <span data-ttu-id="c90e7-2435">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="c90e7-2435">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="c90e7-2436">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="c90e7-2436">Updated the description of ID in help files</span></span>
* <span data-ttu-id="c90e7-2437">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-2437">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c90e7-2438">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c90e7-2438">Az.DataLakeStore</span></span>
* <span data-ttu-id="c90e7-2439">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2439">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="c90e7-2440">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="c90e7-2440">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c90e7-2441">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c90e7-2441">Az.EventGrid</span></span>
* <span data-ttu-id="c90e7-2442">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2442">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="c90e7-2443">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="c90e7-2443">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="c90e7-2444">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="c90e7-2444">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="c90e7-2445">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="c90e7-2445">Event Time-To-Live,</span></span>
        - <span data-ttu-id="c90e7-2446">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="c90e7-2446">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="c90e7-2447">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2447">Dead letter endpoint.</span></span>
    - <span data-ttu-id="c90e7-2448">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="c90e7-2448">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="c90e7-2449">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="c90e7-2449">Event Time-To-Live,</span></span>
        - <span data-ttu-id="c90e7-2450">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="c90e7-2450">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="c90e7-2451">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2451">Dead letter endpoint.</span></span>
* <span data-ttu-id="c90e7-2452">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2452">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="c90e7-2453">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2453">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c90e7-2454">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-2454">Az.IotHub</span></span>
* <span data-ttu-id="c90e7-2455">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="c90e7-2455">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="c90e7-2456">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c90e7-2456">Az.LogicApp</span></span>
* <span data-ttu-id="c90e7-2457">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="c90e7-2457">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-2458">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-2458">Az.Resources</span></span>
* <span data-ttu-id="c90e7-2459">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="c90e7-2459">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="c90e7-2460">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="c90e7-2460">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="c90e7-2461">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="c90e7-2461">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="c90e7-2462">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="c90e7-2462">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="c90e7-2463">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="c90e7-2463">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="c90e7-2464">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="c90e7-2464">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="c90e7-2465">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="c90e7-2465">Az.SignalR</span></span>
* <span data-ttu-id="c90e7-2466">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-2466">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-2467">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-2467">Az.Sql</span></span>
* <span data-ttu-id="c90e7-2468">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2468">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c90e7-2469">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-2469">Az.Storage</span></span>
* <span data-ttu-id="c90e7-2470">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="c90e7-2470">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="c90e7-2471">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="c90e7-2471">New-AzStorageContext</span></span>
* <span data-ttu-id="c90e7-2472">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="c90e7-2472">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="c90e7-2473">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="c90e7-2473">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-2474">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-2474">Az.Websites</span></span>
* <span data-ttu-id="c90e7-2475">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="c90e7-2475">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="c90e7-2476">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-2476">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="c90e7-2477">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="c90e7-2477">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="c90e7-2478">Geral</span><span class="sxs-lookup"><span data-stu-id="c90e7-2478">General</span></span>

- <span data-ttu-id="c90e7-2479">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="c90e7-2479">General Availability of Az Module</span></span>
- <span data-ttu-id="c90e7-2480">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="c90e7-2480">Online help for each module</span></span>
- <span data-ttu-id="c90e7-2481">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="c90e7-2481">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="c90e7-2482">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="c90e7-2482">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="c90e7-2483">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-2483">Az.Accounts</span></span>
- <span data-ttu-id="c90e7-2484">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="c90e7-2484">Changed from Az.Profile</span></span>
- <span data-ttu-id="c90e7-2485">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="c90e7-2485">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="c90e7-2486">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c90e7-2486">Az.ApiManagement</span></span>
- <span data-ttu-id="c90e7-2487">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="c90e7-2487">Fixes for #7002</span></span>
- <span data-ttu-id="c90e7-2488">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c90e7-2488">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="c90e7-2489">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c90e7-2489">Az.Batch</span></span>
- <span data-ttu-id="c90e7-2490">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2490">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="c90e7-2491">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2491">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="c90e7-2492">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c90e7-2492">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="c90e7-2493">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="c90e7-2493">Az.Billing</span></span>
- <span data-ttu-id="c90e7-2494">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c90e7-2494">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="c90e7-2495">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2495">Az.CognitivServices</span></span>
- <span data-ttu-id="c90e7-2496">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-2496">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="c90e7-2497">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="c90e7-2497">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="c90e7-2498">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c90e7-2498">Az.ContainerInstance</span></span>
- <span data-ttu-id="c90e7-2499">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="c90e7-2499">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="c90e7-2500">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="c90e7-2500">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="c90e7-2501">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c90e7-2501">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="c90e7-2502">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c90e7-2502">Az.DataLakeStore</span></span>
- <span data-ttu-id="c90e7-2503">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c90e7-2503">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="c90e7-2504">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c90e7-2504">Az.Monitor</span></span>
- <span data-ttu-id="c90e7-2505">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c90e7-2505">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="c90e7-2506">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c90e7-2506">Az.KeyVault</span></span>
- <span data-ttu-id="c90e7-2507">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="c90e7-2507">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="c90e7-2508">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="c90e7-2508">Az.MachineLearning</span></span>
- <span data-ttu-id="c90e7-2509">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="c90e7-2509">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="c90e7-2510">Az.Media</span><span class="sxs-lookup"><span data-stu-id="c90e7-2510">Az.Media</span></span>
- <span data-ttu-id="c90e7-2511">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="c90e7-2511">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="c90e7-2512">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-2512">Az.Network</span></span>
<span data-ttu-id="c90e7-2513">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="c90e7-2513">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="c90e7-2514">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="c90e7-2514">New cmdlets added:</span></span>
        - <span data-ttu-id="c90e7-2515">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-2515">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c90e7-2516">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-2516">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c90e7-2517">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-2517">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c90e7-2518">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-2518">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c90e7-2519">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-2519">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c90e7-2520">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="c90e7-2520">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="c90e7-2521">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-2521">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="c90e7-2522">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="c90e7-2522">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="c90e7-2523">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c90e7-2523">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="c90e7-2524">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="c90e7-2524">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="c90e7-2525">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="c90e7-2525">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="c90e7-2526">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="c90e7-2526">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="c90e7-2527">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-2527">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="c90e7-2528">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-2528">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="c90e7-2529">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2529">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="c90e7-2530">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="c90e7-2530">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="c90e7-2531">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="c90e7-2531">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="c90e7-2532">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="c90e7-2532">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="c90e7-2533">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="c90e7-2533">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="c90e7-2534">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="c90e7-2534">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="c90e7-2535">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c90e7-2535">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="c90e7-2536">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-2536">Az.OperationalInsights</span></span>
- <span data-ttu-id="c90e7-2537">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c90e7-2537">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="c90e7-2538">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="c90e7-2538">Az.Profile</span></span>
- <span data-ttu-id="c90e7-2539">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c90e7-2539">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-2540">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2540">Az.RecoveryServices</span></span>
- <span data-ttu-id="c90e7-2541">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c90e7-2541">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="c90e7-2542">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-2542">Az.Resources</span></span>
- <span data-ttu-id="c90e7-2543">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c90e7-2543">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="c90e7-2544">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c90e7-2544">Az.ServiceFabric</span></span>
- <span data-ttu-id="c90e7-2545">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="c90e7-2545">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="c90e7-2546">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c90e7-2546">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="c90e7-2547">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="c90e7-2547">Az.SIgnalR</span></span>
- <span data-ttu-id="c90e7-2548">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="c90e7-2548">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="c90e7-2549">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-2549">Az.Sql</span></span>
- <span data-ttu-id="c90e7-2550">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="c90e7-2550">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="c90e7-2551">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="c90e7-2551">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="c90e7-2552">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c90e7-2552">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="c90e7-2553">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-2553">Az.Storage</span></span>
- <span data-ttu-id="c90e7-2554">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c90e7-2554">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="c90e7-2555">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-2555">Az.Websites</span></span>
- <span data-ttu-id="c90e7-2556">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="c90e7-2556">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="c90e7-2557">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="c90e7-2557">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="c90e7-2558">Geral</span><span class="sxs-lookup"><span data-stu-id="c90e7-2558">General</span></span>

* <span data-ttu-id="c90e7-2559">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="c90e7-2559">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="c90e7-2560">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-2560">Az.Compute</span></span>

* <span data-ttu-id="c90e7-2561">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2561">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="c90e7-2562">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c90e7-2562">Az.DataLakeStore</span></span>

* <span data-ttu-id="c90e7-2563">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="c90e7-2563">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="c90e7-2564">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c90e7-2564">Az.FrontDoor</span></span>

* <span data-ttu-id="c90e7-2565">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="c90e7-2565">Fixed some broken links</span></span>
    - <span data-ttu-id="c90e7-2566">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2566">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="c90e7-2567">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2567">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="c90e7-2568">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2568">Az.RecoveryServices</span></span>

* <span data-ttu-id="c90e7-2569">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2569">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="c90e7-2570">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2570">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="c90e7-2571">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-2571">Az.Resources</span></span>

* <span data-ttu-id="c90e7-2572">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="c90e7-2572">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="c90e7-2573">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2573">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="c90e7-2574">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-2574">Az.Sql</span></span>

* <span data-ttu-id="c90e7-2575">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="c90e7-2575">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="c90e7-2576">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="c90e7-2576">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="c90e7-2577">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2577">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="c90e7-2578">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-2578">Az.Storage</span></span>

* <span data-ttu-id="c90e7-2579">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c90e7-2579">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="c90e7-2580">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="c90e7-2580">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="c90e7-2581">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="c90e7-2581">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="c90e7-2582">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="c90e7-2582">Support Static Website configuration</span></span>
    - <span data-ttu-id="c90e7-2583">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="c90e7-2583">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="c90e7-2584">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="c90e7-2584">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="c90e7-2585">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-2585">Az.Websites</span></span>

* <span data-ttu-id="c90e7-2586">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="c90e7-2586">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="c90e7-2587">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2587">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="c90e7-2588">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2588">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="c90e7-2589">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="c90e7-2589">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="c90e7-2590">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c90e7-2590">Az.ApiManagement</span></span>
* <span data-ttu-id="c90e7-2591">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2591">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="c90e7-2592">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c90e7-2592">Az.Automation</span></span>
* <span data-ttu-id="c90e7-2593">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="c90e7-2593">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="c90e7-2594">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="c90e7-2594">Added Update Management cmdlets</span></span>
* <span data-ttu-id="c90e7-2595">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="c90e7-2595">Added Source Control cmdlets</span></span>
* <span data-ttu-id="c90e7-2596">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="c90e7-2596">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="c90e7-2597">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="c90e7-2597">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="c90e7-2598">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-2598">Az.Compute</span></span>
* <span data-ttu-id="c90e7-2599">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="c90e7-2599">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="c90e7-2600">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2600">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="c90e7-2601">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c90e7-2601">Az.ContainerInstance</span></span>
* <span data-ttu-id="c90e7-2602">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2602">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="c90e7-2603">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="c90e7-2603">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="c90e7-2604">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="c90e7-2604">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="c90e7-2605">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-2605">Az.Network</span></span>
* <span data-ttu-id="c90e7-2606">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="c90e7-2606">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="c90e7-2607">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="c90e7-2607">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="c90e7-2608">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2608">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="c90e7-2609">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="c90e7-2609">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="c90e7-2610">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="c90e7-2610">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="c90e7-2611">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2611">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="c90e7-2612">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2612">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="c90e7-2613">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="c90e7-2613">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="c90e7-2614">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="c90e7-2614">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="c90e7-2615">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="c90e7-2615">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="c90e7-2616">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="c90e7-2616">Az.Relay</span></span>
* <span data-ttu-id="c90e7-2617">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2617">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="c90e7-2618">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-2618">Az.Resources</span></span>
* <span data-ttu-id="c90e7-2619">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="c90e7-2619">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="c90e7-2620">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="c90e7-2620">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="c90e7-2621">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="c90e7-2621">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="c90e7-2622">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c90e7-2622">Az.ServiceFabric</span></span>
* <span data-ttu-id="c90e7-2623">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="c90e7-2623">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="c90e7-2624">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-2624">Az.Sql</span></span>
* <span data-ttu-id="c90e7-2625">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-2625">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="c90e7-2626">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c90e7-2626">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c90e7-2627">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c90e7-2627">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c90e7-2628">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c90e7-2628">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c90e7-2629">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c90e7-2629">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c90e7-2630">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c90e7-2630">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="c90e7-2631">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c90e7-2631">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="c90e7-2632">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c90e7-2632">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="c90e7-2633">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c90e7-2633">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="c90e7-2634">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2634">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="c90e7-2635">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2635">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="c90e7-2636">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2636">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="c90e7-2637">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2637">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="c90e7-2638">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2638">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="c90e7-2639">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2639">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="c90e7-2640">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2640">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="c90e7-2641">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="c90e7-2641">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="c90e7-2642">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="c90e7-2642">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="c90e7-2643">Geral</span><span class="sxs-lookup"><span data-stu-id="c90e7-2643">General</span></span>
* <span data-ttu-id="c90e7-2644">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="c90e7-2644">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="c90e7-2645">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="c90e7-2645">Az.Profile</span></span>
* <span data-ttu-id="c90e7-2646">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="c90e7-2646">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="c90e7-2647">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="c90e7-2647">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="c90e7-2648">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="c90e7-2648">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="c90e7-2649">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="c90e7-2649">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="c90e7-2650">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="c90e7-2650">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="c90e7-2651">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="c90e7-2651">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="c90e7-2652">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="c90e7-2652">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="c90e7-2653">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2653">Az.CognitiveServices</span></span>
* <span data-ttu-id="c90e7-2654">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2654">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-2655">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-2655">Az.Compute</span></span>
* <span data-ttu-id="c90e7-2656">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="c90e7-2656">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="c90e7-2657">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="c90e7-2657">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="c90e7-2658">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2658">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c90e7-2659">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c90e7-2659">Az.DataLakeStore</span></span>
* <span data-ttu-id="c90e7-2660">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2660">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="c90e7-2661">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2661">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="c90e7-2662">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="c90e7-2662">Az.Insights</span></span>
* <span data-ttu-id="c90e7-2663">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="c90e7-2663">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="c90e7-2664">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="c90e7-2664">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="c90e7-2665">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="c90e7-2665">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="c90e7-2666">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="c90e7-2666">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-2667">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-2667">Az.Network</span></span>
* <span data-ttu-id="c90e7-2668">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="c90e7-2668">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="c90e7-2669">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="c90e7-2669">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="c90e7-2670">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="c90e7-2670">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="c90e7-2671">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="c90e7-2671">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="c90e7-2672">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="c90e7-2672">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="c90e7-2673">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="c90e7-2673">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="c90e7-2674">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="c90e7-2674">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c90e7-2675">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c90e7-2675">Az.PolicyInsights</span></span>
* <span data-ttu-id="c90e7-2676">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="c90e7-2676">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-2677">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-2677">Az.Resources</span></span>
* <span data-ttu-id="c90e7-2678">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="c90e7-2678">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="c90e7-2679">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="c90e7-2679">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c90e7-2680">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c90e7-2680">Az.ServiceBus</span></span>
* <span data-ttu-id="c90e7-2681">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2681">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c90e7-2682">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c90e7-2682">Az.ServiceFabric</span></span>
* <span data-ttu-id="c90e7-2683">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2683">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="c90e7-2684">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="c90e7-2684">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="c90e7-2685">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="c90e7-2685">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="c90e7-2686">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="c90e7-2686">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="c90e7-2687">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2687">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="c90e7-2688">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="c90e7-2688">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="c90e7-2689">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="c90e7-2689">Az.Profile</span></span>
* <span data-ttu-id="c90e7-2690">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="c90e7-2690">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="c90e7-2691">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="c90e7-2691">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-2692">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-2692">Az.Compute</span></span>
* <span data-ttu-id="c90e7-2693">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="c90e7-2693">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="c90e7-2694">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2694">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c90e7-2695">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c90e7-2695">Az.DataLakeStore</span></span>
* <span data-ttu-id="c90e7-2696">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="c90e7-2696">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="c90e7-2697">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2697">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="c90e7-2698">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2698">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="c90e7-2699">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2699">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="c90e7-2700">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2700">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-2701">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-2701">Az.Network</span></span>
* <span data-ttu-id="c90e7-2702">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2702">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="c90e7-2703">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2703">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-2704">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-2704">Az.Resources</span></span>
* <span data-ttu-id="c90e7-2705">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2705">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="c90e7-2706">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="c90e7-2706">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="c90e7-2707">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="c90e7-2707">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="c90e7-2708">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="c90e7-2708">Azure.Storage</span></span>
* <span data-ttu-id="c90e7-2709">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="c90e7-2709">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="c90e7-2710">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="c90e7-2710">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="c90e7-2711">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="c90e7-2711">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="c90e7-2712">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2712">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="c90e7-2713">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="c90e7-2713">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c90e7-2714">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c90e7-2714">Az.CognitiveServices</span></span>
* <span data-ttu-id="c90e7-2715">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2715">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c90e7-2716">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c90e7-2716">Az.Compute</span></span>
* <span data-ttu-id="c90e7-2717">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="c90e7-2717">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="c90e7-2718">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2718">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="c90e7-2719">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="c90e7-2719">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="c90e7-2720">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="c90e7-2720">Az.DataFactoryV2</span></span>
* <span data-ttu-id="c90e7-2721">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2721">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c90e7-2722">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c90e7-2722">Az.Network</span></span>
* <span data-ttu-id="c90e7-2723">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2723">Added NetworkProfile functionality.</span></span> <span data-ttu-id="c90e7-2724">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="c90e7-2724">new cmdlets added</span></span>
    - <span data-ttu-id="c90e7-2725">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c90e7-2725">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="c90e7-2726">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c90e7-2726">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="c90e7-2727">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c90e7-2727">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="c90e7-2728">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c90e7-2728">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="c90e7-2729">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-2729">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="c90e7-2730">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-2730">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="c90e7-2731">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="c90e7-2731">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="c90e7-2732">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="c90e7-2732">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="c90e7-2733">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="c90e7-2733">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="c90e7-2734">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c90e7-2734">Az.RedisCache</span></span>
* <span data-ttu-id="c90e7-2735">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="c90e7-2735">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="c90e7-2736">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="c90e7-2736">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="c90e7-2737">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c90e7-2737">Az.Resources</span></span>
* <span data-ttu-id="c90e7-2738">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="c90e7-2738">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="c90e7-2739">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="c90e7-2739">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="c90e7-2740">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c90e7-2740">Az.Sql</span></span>
* <span data-ttu-id="c90e7-2741">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="c90e7-2741">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c90e7-2742">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c90e7-2742">Az.Websites</span></span>
* <span data-ttu-id="c90e7-2743">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="c90e7-2743">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="c90e7-2744">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="c90e7-2744">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="c90e7-2745">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="c90e7-2745">0.2.0 - September 2018</span></span>
 <span data-ttu-id="c90e7-2746">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="c90e7-2746">Initial Release</span></span>
