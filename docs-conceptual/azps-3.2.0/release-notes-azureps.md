---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/15/2019
ms.openlocfilehash: f77d901169b0d98b2425a2e50d33a1789150b770
ms.sourcegitcommit: e598dc45a26ff5a71112383252b350d750144a47
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/17/2019
ms.locfileid: "75182558"
---
## <a name="320---december-2019"></a><span data-ttu-id="24b38-103">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-103">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="24b38-104">Geral</span><span class="sxs-lookup"><span data-stu-id="24b38-104">General</span></span>
* <span data-ttu-id="24b38-105">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="24b38-105">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="24b38-106">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-106">Az.Accounts</span></span>
* <span data-ttu-id="24b38-107">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="24b38-107">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="24b38-108">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="24b38-108">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="24b38-109">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="24b38-109">Az.Batch</span></span>
* <span data-ttu-id="24b38-110">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="24b38-110">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="24b38-111">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="24b38-111">Az.DataFactory</span></span>
* <span data-ttu-id="24b38-112">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="24b38-112">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="24b38-113">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="24b38-113">Az.FrontDoor</span></span>
* <span data-ttu-id="24b38-114">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="24b38-114">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="24b38-115">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="24b38-115">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="24b38-116">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="24b38-116">Az.HealthcareApis</span></span>
* <span data-ttu-id="24b38-117">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="24b38-117">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="24b38-118">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="24b38-118">Az.KeyVault</span></span>
* <span data-ttu-id="24b38-119">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="24b38-119">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="24b38-120">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="24b38-120">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="24b38-121">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="24b38-121">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="24b38-122">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="24b38-122">Az.Monitor</span></span>
* <span data-ttu-id="24b38-123">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="24b38-123">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="24b38-124">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="24b38-124">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="24b38-125">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="24b38-125">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-126">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-126">Az.Network</span></span>
* <span data-ttu-id="24b38-127">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="24b38-127">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-128">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-128">Az.Resources</span></span>
* <span data-ttu-id="24b38-129">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="24b38-129">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="24b38-130">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="24b38-130">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-131">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-131">Az.Sql</span></span>
* <span data-ttu-id="24b38-132">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="24b38-132">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="24b38-133">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-133">Az.Storage</span></span>
* <span data-ttu-id="24b38-134">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="24b38-134">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="24b38-135">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="24b38-135">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="24b38-136">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="24b38-136">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="24b38-137">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="24b38-137">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="24b38-138">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="24b38-138">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="24b38-139">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="24b38-139">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="24b38-140">Suporte de partilha de QuotaGiB em mais de 5120 cmdlets de Partilha de Ficheiros do plano de gestão e adição do alias do parâmetro "Quota" ao parâmetro "QuotaGiB"</span><span class="sxs-lookup"><span data-stu-id="24b38-140">Support Share QuotaGiB more than 5120 in Management plane File Share cmdlets, and add parameter alias 'Quota' to parameter 'QuotaGiB'</span></span> 
    - <span data-ttu-id="24b38-141">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="24b38-141">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="24b38-142">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="24b38-142">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="24b38-143">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="24b38-143">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="24b38-144">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="24b38-144">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="24b38-145">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="24b38-145">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="24b38-146">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="24b38-146">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="24b38-147">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-147">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="24b38-148">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="24b38-148">Highlights since the last major release</span></span>
* <span data-ttu-id="24b38-149">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="24b38-149">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="24b38-150">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="24b38-150">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-151">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-151">Az.Compute</span></span>
* <span data-ttu-id="24b38-152">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="24b38-152">VM Reapply feature</span></span>
    - <span data-ttu-id="24b38-153">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="24b38-153">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="24b38-154">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="24b38-154">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="24b38-155">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="24b38-155">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="24b38-156">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="24b38-156">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="24b38-157">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="24b38-157">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="24b38-158">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="24b38-158">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="24b38-159">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="24b38-159">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="24b38-160">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="24b38-160">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="24b38-161">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="24b38-161">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="24b38-162">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="24b38-162">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="24b38-163">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="24b38-163">Az.DataBoxEdge</span></span>
* <span data-ttu-id="24b38-164">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="24b38-164">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="24b38-165">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="24b38-165">Get the Order</span></span>
* <span data-ttu-id="24b38-166">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="24b38-166">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="24b38-167">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="24b38-167">Create new Order</span></span>
* <span data-ttu-id="24b38-168">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="24b38-168">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="24b38-169">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="24b38-169">Remove the Order</span></span>
* <span data-ttu-id="24b38-170">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="24b38-170">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="24b38-171">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="24b38-171">Now creates Local Share</span></span>
* <span data-ttu-id="24b38-172">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="24b38-172">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="24b38-173">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="24b38-173">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="24b38-174">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="24b38-174">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="24b38-175">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="24b38-175">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="24b38-176">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="24b38-176">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="24b38-177">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="24b38-177">Gets the information about Triggers</span></span>
* <span data-ttu-id="24b38-178">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="24b38-178">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="24b38-179">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="24b38-179">Create new Triggers</span></span>
* <span data-ttu-id="24b38-180">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="24b38-180">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="24b38-181">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="24b38-181">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="24b38-182">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="24b38-182">Az.DataFactory</span></span>
* <span data-ttu-id="24b38-183">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="24b38-183">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="24b38-184">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="24b38-184">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="24b38-185">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="24b38-185">Az.DataLakeStore</span></span>
* <span data-ttu-id="24b38-186">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="24b38-186">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="24b38-187">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="24b38-187">Az.EventHub</span></span>
* <span data-ttu-id="24b38-188">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="24b38-188">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="24b38-189">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="24b38-189">Az.FrontDoor</span></span>
* <span data-ttu-id="24b38-190">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="24b38-190">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="24b38-191">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="24b38-191">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="24b38-192">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="24b38-192">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="24b38-193">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="24b38-193">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-194">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-194">Az.Network</span></span>
* <span data-ttu-id="24b38-195">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="24b38-195">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="24b38-196">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="24b38-196">Az.PrivateDns</span></span>
* <span data-ttu-id="24b38-197">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="24b38-197">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="24b38-198">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="24b38-198">Az.RecoveryServices</span></span>
* <span data-ttu-id="24b38-199">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="24b38-199">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="24b38-200">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="24b38-200">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="24b38-201">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="24b38-201">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="24b38-202">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="24b38-202">Az.RedisCache</span></span>
* <span data-ttu-id="24b38-203">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="24b38-203">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="24b38-204">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="24b38-204">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="24b38-205">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="24b38-205">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-206">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-206">Az.Resources</span></span>
- <span data-ttu-id="24b38-207">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="24b38-207">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="24b38-208">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="24b38-208">Updated create policy definition help example</span></span>
- <span data-ttu-id="24b38-209">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="24b38-209">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="24b38-210">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="24b38-210">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="24b38-211">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="24b38-211">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-212">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-212">Az.Sql</span></span>
* <span data-ttu-id="24b38-213">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="24b38-213">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="24b38-214">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="24b38-214">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="24b38-215">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-215">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="24b38-216">Geral</span><span class="sxs-lookup"><span data-stu-id="24b38-216">General</span></span>
* <span data-ttu-id="24b38-217">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="24b38-217">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="24b38-218">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-218">Az.Accounts</span></span>
* <span data-ttu-id="24b38-219">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="24b38-219">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="24b38-220">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="24b38-220">Az.Advisor</span></span>
* <span data-ttu-id="24b38-221">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="24b38-221">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="24b38-222">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="24b38-222">Az.Batch</span></span>
* <span data-ttu-id="24b38-223">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="24b38-223">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="24b38-224">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="24b38-224">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="24b38-225">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="24b38-225">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="24b38-226">O parâmetro `-ResourceFile` de **New-AzBatchTask** agora assume uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="24b38-226">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="24b38-227">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="24b38-227">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="24b38-228">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="24b38-228">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="24b38-229">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="24b38-229">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="24b38-230">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="24b38-230">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="24b38-231">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="24b38-231">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="24b38-232">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="24b38-232">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="24b38-233">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="24b38-233">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="24b38-234">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="24b38-234">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="24b38-235">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="24b38-235">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="24b38-236">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="24b38-236">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="24b38-237">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="24b38-237">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="24b38-238">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="24b38-238">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="24b38-239">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="24b38-239">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="24b38-240">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="24b38-240">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="24b38-241">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="24b38-241">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="24b38-242">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="24b38-242">This operation is no longer supported.</span></span>
* <span data-ttu-id="24b38-243">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="24b38-243">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="24b38-244">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="24b38-244">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="24b38-245">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="24b38-245">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="24b38-246">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="24b38-246">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span> 
  - <span data-ttu-id="24b38-247">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="24b38-247">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="24b38-248">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="24b38-248">New non-verified images are also now returned.</span></span> <span data-ttu-id="24b38-249">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="24b38-249">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="24b38-250">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="24b38-250">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="24b38-251">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="24b38-251">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="24b38-252">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="24b38-252">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="24b38-253">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="24b38-253">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="24b38-254">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="24b38-254">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="24b38-255">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="24b38-255">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="24b38-256">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="24b38-256">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="24b38-257">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="24b38-257">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="24b38-258">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="24b38-258">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="24b38-259">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="24b38-259">Az.Cdn</span></span>
* <span data-ttu-id="24b38-260">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="24b38-260">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="24b38-261">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="24b38-261">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-262">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-262">Az.Compute</span></span>
* <span data-ttu-id="24b38-263">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="24b38-263">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="24b38-264">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="24b38-264">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="24b38-265">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span><span class="sxs-lookup"><span data-stu-id="24b38-265">DiskEncryptionSetId parameter is added to the following cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span></span>        
        <span data-ttu-id="24b38-266">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="24b38-266">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="24b38-267">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-267">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="24b38-268">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-268">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="24b38-269">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="24b38-269">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="24b38-270">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="24b38-270">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="24b38-271">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="24b38-271">Breaking changes</span></span>
    - <span data-ttu-id="24b38-272">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="24b38-272">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="24b38-273">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="24b38-273">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="24b38-274">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="24b38-274">Az.DataFactory</span></span>
* <span data-ttu-id="24b38-275">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="24b38-275">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="24b38-276">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="24b38-276">Az.DataLakeStore</span></span>
* <span data-ttu-id="24b38-277">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha)) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="24b38-277">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="24b38-278">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="24b38-278">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="24b38-279">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="24b38-279">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="24b38-280">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="24b38-280">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="24b38-281">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="24b38-281">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="24b38-282">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="24b38-282">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="24b38-283">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="24b38-283">Az.FrontDoor</span></span>
* <span data-ttu-id="24b38-284">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="24b38-284">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="24b38-285">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="24b38-285">Az.HDInsight</span></span>
* <span data-ttu-id="24b38-286">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="24b38-286">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="24b38-287">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="24b38-287">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="24b38-288">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="24b38-288">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="24b38-289">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="24b38-289">Removed five cmdlets:</span></span>
    - <span data-ttu-id="24b38-290">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="24b38-290">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="24b38-291">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="24b38-291">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="24b38-292">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="24b38-292">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="24b38-293">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="24b38-293">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="24b38-294">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="24b38-294">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="24b38-295">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="24b38-295">Added three cmdlets:</span></span>
    - <span data-ttu-id="24b38-296">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="24b38-296">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="24b38-297">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="24b38-297">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="24b38-298">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="24b38-298">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="24b38-299">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="24b38-299">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="24b38-300">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="24b38-300">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="24b38-301">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="24b38-301">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="24b38-302">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="24b38-302">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="24b38-303">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="24b38-303">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="24b38-304">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="24b38-304">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="24b38-305">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="24b38-305">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="24b38-306">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="24b38-306">Added some scenario test cases.</span></span>
* <span data-ttu-id="24b38-307">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="24b38-307">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="24b38-308">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="24b38-308">Az.IotHub</span></span>
* <span data-ttu-id="24b38-309">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="24b38-309">Breaking changes:</span></span>
    - <span data-ttu-id="24b38-310">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="24b38-310">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="24b38-311">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="24b38-311">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="24b38-312">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="24b38-312">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="24b38-313">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="24b38-313">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="24b38-314">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="24b38-314">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="24b38-315">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="24b38-315">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="24b38-316">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="24b38-316">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="24b38-317">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="24b38-317">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="24b38-318">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="24b38-318">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="24b38-319">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="24b38-319">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="24b38-320">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="24b38-320">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="24b38-321">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="24b38-321">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="24b38-322">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="24b38-322">Az.RecoveryServices</span></span>
* <span data-ttu-id="24b38-323">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="24b38-323">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="24b38-324">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="24b38-324">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="24b38-325">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="24b38-325">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="24b38-326">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="24b38-326">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="24b38-327">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="24b38-327">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="24b38-328">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="24b38-328">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="24b38-329">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="24b38-329">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="24b38-330">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="24b38-330">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="24b38-331">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="24b38-331">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-332">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-332">Az.Resources</span></span>
* <span data-ttu-id="24b38-333">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="24b38-333">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-334">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-334">Az.Network</span></span>
* <span data-ttu-id="24b38-335">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="24b38-335">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="24b38-336">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="24b38-336">Updated cmdlet:</span></span>
        - <span data-ttu-id="24b38-337">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-337">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="24b38-338">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-338">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="24b38-339">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-339">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="24b38-340">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-340">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="24b38-341">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-341">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="24b38-342">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="24b38-342">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="24b38-343">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="24b38-343">New cmdlet:</span></span>
        - <span data-ttu-id="24b38-344">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="24b38-344">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="24b38-345">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="24b38-345">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="24b38-346">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="24b38-346">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="24b38-347">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-347">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="24b38-348">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="24b38-348">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="24b38-349">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="24b38-349">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="24b38-350">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="24b38-350">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="24b38-351">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="24b38-351">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="24b38-352">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="24b38-352">New cmdlets added:</span></span>
        - <span data-ttu-id="24b38-353">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="24b38-353">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="24b38-354">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="24b38-354">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="24b38-355">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="24b38-355">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="24b38-356">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="24b38-356">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="24b38-357">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="24b38-357">Set-AzVirtualHub</span></span>
* <span data-ttu-id="24b38-358">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="24b38-358">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="24b38-359">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="24b38-359">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="24b38-360">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="24b38-360">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="24b38-361">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="24b38-361">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="24b38-362">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="24b38-362">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="24b38-363">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="24b38-363">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="24b38-364">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-364">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="24b38-365">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="24b38-365">New cmdlets added:</span></span>
        - <span data-ttu-id="24b38-366">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-366">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="24b38-367">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="24b38-367">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="24b38-368">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="24b38-368">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="24b38-369">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="24b38-369">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="24b38-370">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="24b38-370">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="24b38-371">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="24b38-371">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="24b38-372">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="24b38-372">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="24b38-373">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="24b38-373">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="24b38-374">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="24b38-374">New cmdlets added:</span></span>
        - <span data-ttu-id="24b38-375">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="24b38-375">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="24b38-376">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="24b38-376">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="24b38-377">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="24b38-377">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="24b38-378">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="24b38-378">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="24b38-379">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="24b38-379">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="24b38-380">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="24b38-380">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="24b38-381">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="24b38-381">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="24b38-382">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="24b38-382">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="24b38-383">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="24b38-383">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="24b38-384">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="24b38-384">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="24b38-385">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="24b38-385">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="24b38-386">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="24b38-386">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="24b38-387">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="24b38-387">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="24b38-388">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="24b38-388">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="24b38-389">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="24b38-389">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="24b38-390">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="24b38-390">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="24b38-391">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="24b38-391">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="24b38-392">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="24b38-392">New cmdlets added:</span></span>
        - <span data-ttu-id="24b38-393">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="24b38-393">New-AzIpGroup</span></span>
        - <span data-ttu-id="24b38-394">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="24b38-394">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="24b38-395">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="24b38-395">Get-AzIpGroup</span></span>
        - <span data-ttu-id="24b38-396">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="24b38-396">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="24b38-397">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="24b38-397">Az.ServiceFabric</span></span>
* <span data-ttu-id="24b38-398">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="24b38-398">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-399">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-399">Az.Sql</span></span>
* <span data-ttu-id="24b38-400">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="24b38-400">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="24b38-401">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="24b38-401">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="24b38-402">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="24b38-402">Removed deprecated aliases:</span></span>
* <span data-ttu-id="24b38-403">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="24b38-403">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="24b38-404">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="24b38-404">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="24b38-405">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="24b38-405">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="24b38-406">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="24b38-406">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="24b38-407">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="24b38-407">Deprecate Advanced Threat Detection Settings cmdlets</span></span> 
* <span data-ttu-id="24b38-408">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="24b38-408">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="24b38-409">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-409">Az.Storage</span></span>
* <span data-ttu-id="24b38-410">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="24b38-410">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="24b38-411">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="24b38-411">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="24b38-412">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="24b38-412">Set-AzStorageAccount</span></span>
* <span data-ttu-id="24b38-413">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="24b38-413">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="24b38-414">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="24b38-414">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="24b38-415">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="24b38-415">Close-AzStorageFileHandle</span></span>
    
## <a name="280---october-2019"></a><span data-ttu-id="24b38-416">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-416">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="24b38-417">Geral</span><span class="sxs-lookup"><span data-stu-id="24b38-417">General</span></span>
* <span data-ttu-id="24b38-418">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="24b38-418">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="24b38-419">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-419">Az.Accounts</span></span>
* <span data-ttu-id="24b38-420">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="24b38-420">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="24b38-421">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="24b38-421">Az.ApiManagement</span></span>
* <span data-ttu-id="24b38-422">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="24b38-422">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="24b38-423">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="24b38-423">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="24b38-424">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="24b38-424">Az.Automation</span></span>
* <span data-ttu-id="24b38-425">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="24b38-425">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="24b38-426">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="24b38-426">Az.Batch</span></span>
* <span data-ttu-id="24b38-427">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="24b38-427">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-428">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-428">Az.Compute</span></span>
* <span data-ttu-id="24b38-429">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="24b38-429">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="24b38-430">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="24b38-430">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="24b38-431">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="24b38-431">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="24b38-432">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="24b38-432">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="24b38-433">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="24b38-433">Az.DataFactory</span></span>
* <span data-ttu-id="24b38-434">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="24b38-434">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="24b38-435">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="24b38-435">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="24b38-436">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="24b38-436">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="24b38-437">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="24b38-437">Az.DataLakeStore</span></span>
* <span data-ttu-id="24b38-438">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="24b38-438">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="24b38-439">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="24b38-439">Az.HealthcareApis</span></span>
* <span data-ttu-id="24b38-440">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="24b38-440">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="24b38-441">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="24b38-441">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="24b38-442">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="24b38-442">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="24b38-443">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="24b38-443">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="24b38-444">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="24b38-444">Az.IotHub</span></span>
* <span data-ttu-id="24b38-445">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="24b38-445">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="24b38-446">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="24b38-446">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="24b38-447">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="24b38-447">Az.Monitor</span></span>
* <span data-ttu-id="24b38-448">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="24b38-448">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="24b38-449">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="24b38-449">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="24b38-450">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="24b38-450">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="24b38-451">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="24b38-451">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-452">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-452">Az.Network</span></span>
* <span data-ttu-id="24b38-453">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="24b38-453">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="24b38-454">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="24b38-454">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="24b38-455">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="24b38-455">New cmdlets added:</span></span>
        - <span data-ttu-id="24b38-456">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="24b38-456">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="24b38-457">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-457">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="24b38-458">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="24b38-458">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="24b38-459">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="24b38-459">Updated cmdlets:</span></span>
        - <span data-ttu-id="24b38-460">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-460">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="24b38-461">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-461">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="24b38-462">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-462">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="24b38-463">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="24b38-463">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="24b38-464">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="24b38-464">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="24b38-465">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="24b38-465">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="24b38-466">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="24b38-466">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="24b38-467">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="24b38-467">Az.RedisCache</span></span>
* <span data-ttu-id="24b38-468">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="24b38-468">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-469">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-469">Az.Sql</span></span>
* <span data-ttu-id="24b38-470">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="24b38-470">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="24b38-471">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-471">Az.Storage</span></span>
* <span data-ttu-id="24b38-472">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="24b38-472">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="24b38-473">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="24b38-473">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="24b38-474">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="24b38-474">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="24b38-475">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="24b38-475">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="24b38-476">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="24b38-476">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="24b38-477">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="24b38-477">Az.StorageSync</span></span>
* <span data-ttu-id="24b38-478">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="24b38-478">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="24b38-479">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="24b38-479">Az.Websites</span></span>
* <span data-ttu-id="24b38-480">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="24b38-480">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="24b38-481">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-481">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="24b38-482">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="24b38-482">Az.ApiManagement</span></span>
* <span data-ttu-id="24b38-483">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="24b38-483">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="24b38-484">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="24b38-484">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="24b38-485">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="24b38-485">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="24b38-486">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="24b38-486">Az.Automation</span></span>
* <span data-ttu-id="24b38-487">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="24b38-487">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="24b38-488">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="24b38-488">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="24b38-489">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="24b38-489">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-490">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-490">Az.Compute</span></span>
* <span data-ttu-id="24b38-491">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-491">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="24b38-492">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-492">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="24b38-493">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="24b38-493">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="24b38-494">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="24b38-494">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="24b38-495">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="24b38-495">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="24b38-496">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="24b38-496">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="24b38-497">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="24b38-497">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="24b38-498">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="24b38-498">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="24b38-499">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="24b38-499">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="24b38-500">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="24b38-500">Az.DataFactory</span></span>
* <span data-ttu-id="24b38-501">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="24b38-501">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="24b38-502">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="24b38-502">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="24b38-503">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="24b38-503">Az.HDInsight</span></span>
* <span data-ttu-id="24b38-504">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="24b38-504">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="24b38-505">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="24b38-505">Az.IotHub</span></span>
* <span data-ttu-id="24b38-506">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="24b38-506">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="24b38-507">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="24b38-507">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="24b38-508">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="24b38-508">New cmdlets are:</span></span>
    - <span data-ttu-id="24b38-509">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="24b38-509">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="24b38-510">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="24b38-510">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="24b38-511">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="24b38-511">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="24b38-512">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="24b38-512">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="24b38-513">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="24b38-513">Az.Monitor</span></span>
* <span data-ttu-id="24b38-514">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="24b38-514">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="24b38-515">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="24b38-515">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="24b38-516">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="24b38-516">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="24b38-517">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="24b38-517">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="24b38-518">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="24b38-518">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="24b38-519">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="24b38-519">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="24b38-520">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="24b38-520">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="24b38-521">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="24b38-521">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="24b38-522">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="24b38-522">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="24b38-523">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="24b38-523">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="24b38-524">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="24b38-524">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="24b38-525">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="24b38-525">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="24b38-526">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="24b38-526">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="24b38-527">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="24b38-527">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="24b38-528">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="24b38-528">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="24b38-529">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="24b38-529">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="24b38-530">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="24b38-530">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="24b38-531">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="24b38-531">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="24b38-532">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="24b38-532">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="24b38-533">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="24b38-533">Overall improved help files</span></span>
* <span data-ttu-id="24b38-534">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="24b38-534">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-535">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-535">Az.Network</span></span>
* <span data-ttu-id="24b38-536">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="24b38-536">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="24b38-537">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="24b38-537">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="24b38-538">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="24b38-538">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="24b38-539">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="24b38-539">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="24b38-540">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="24b38-540">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="24b38-541">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="24b38-541">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="24b38-542">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="24b38-542">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="24b38-543">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="24b38-543">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="24b38-544">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="24b38-544">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="24b38-545">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="24b38-545">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="24b38-546">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="24b38-546">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="24b38-547">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="24b38-547">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="24b38-548">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="24b38-548">New cmdlets</span></span>
        - <span data-ttu-id="24b38-549">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="24b38-549">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="24b38-550">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-550">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="24b38-551">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="24b38-551">Updated cmdlet:</span></span>
        - <span data-ttu-id="24b38-552">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="24b38-552">New-VpnSite</span></span>
        - <span data-ttu-id="24b38-553">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="24b38-553">Update-VpnSite</span></span>
        - <span data-ttu-id="24b38-554">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-554">New-VpnConnection</span></span>
        - <span data-ttu-id="24b38-555">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-555">Update-VpnConnection</span></span>
* <span data-ttu-id="24b38-556">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="24b38-556">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="24b38-557">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="24b38-557">Az.RecoveryServices</span></span>
* <span data-ttu-id="24b38-558">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="24b38-558">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="24b38-559">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="24b38-559">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-560">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-560">Az.Resources</span></span>
* <span data-ttu-id="24b38-561">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="24b38-561">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="24b38-562">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="24b38-562">Az.ServiceFabric</span></span>
* <span data-ttu-id="24b38-563">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="24b38-563">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="24b38-564">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="24b38-564">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="24b38-565">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="24b38-565">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="24b38-566">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="24b38-566">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="24b38-567">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="24b38-567">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="24b38-568">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="24b38-568">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="24b38-569">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="24b38-569">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="24b38-570">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="24b38-570">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="24b38-571">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="24b38-571">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="24b38-572">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="24b38-572">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="24b38-573">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="24b38-573">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="24b38-574">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="24b38-574">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="24b38-575">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="24b38-575">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="24b38-576">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="24b38-576">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="24b38-577">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="24b38-577">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="24b38-578">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="24b38-578">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="24b38-579">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="24b38-579">Az.SignalR</span></span>
* <span data-ttu-id="24b38-580">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="24b38-580">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-581">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-581">Az.Sql</span></span>
* <span data-ttu-id="24b38-582">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="24b38-582">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="24b38-583">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="24b38-583">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="24b38-584">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="24b38-584">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="24b38-585">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="24b38-585">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="24b38-586">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="24b38-586">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="24b38-587">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-587">Az.Storage</span></span>
* <span data-ttu-id="24b38-588">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="24b38-588">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="24b38-589">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="24b38-589">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="24b38-590">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="24b38-590">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="24b38-591">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="24b38-591">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="24b38-592">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="24b38-592">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="24b38-593">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="24b38-593">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="24b38-594">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="24b38-594">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="24b38-595">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="24b38-595">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="24b38-596">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="24b38-596">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="24b38-597">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="24b38-597">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="24b38-598">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="24b38-598">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="24b38-599">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="24b38-599">Az.Websites</span></span>
* <span data-ttu-id="24b38-600">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="24b38-600">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="24b38-601">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="24b38-601">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="24b38-602">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="24b38-602">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="24b38-603">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-603">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="24b38-604">Geral</span><span class="sxs-lookup"><span data-stu-id="24b38-604">General</span></span>
* <span data-ttu-id="24b38-605">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="24b38-605">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="24b38-606">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-606">Az.Accounts</span></span>
* <span data-ttu-id="24b38-607">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="24b38-607">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="24b38-608">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="24b38-608">Az.Aks</span></span>
* <span data-ttu-id="24b38-609">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="24b38-609">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="24b38-610">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="24b38-610">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="24b38-611">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="24b38-611">Az.ApiManagement</span></span>
* <span data-ttu-id="24b38-612">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="24b38-612">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="24b38-613">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="24b38-613">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="24b38-614">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="24b38-614">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="24b38-615">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="24b38-615">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="24b38-616">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="24b38-616">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="24b38-617">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="24b38-617">Az.Batch</span></span>
* <span data-ttu-id="24b38-618">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="24b38-618">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="24b38-619">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="24b38-619">Az.Cdn</span></span>
* <span data-ttu-id="24b38-620">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="24b38-620">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-621">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-621">Az.Compute</span></span>
* <span data-ttu-id="24b38-622">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-622">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="24b38-623">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="24b38-623">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="24b38-624">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="24b38-624">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="24b38-625">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="24b38-625">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="24b38-626">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="24b38-626">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="24b38-627">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="24b38-627">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="24b38-628">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="24b38-628">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="24b38-629">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="24b38-629">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="24b38-630">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="24b38-630">Az.DataFactory</span></span>
* <span data-ttu-id="24b38-631">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="24b38-631">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="24b38-632">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="24b38-632">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="24b38-633">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="24b38-633">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="24b38-634">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="24b38-634">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="24b38-635">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="24b38-635">Az.DataLakeStore</span></span>
* <span data-ttu-id="24b38-636">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="24b38-636">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="24b38-637">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="24b38-637">Az.EventHub</span></span>
* <span data-ttu-id="24b38-638">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="24b38-638">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="24b38-639">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="24b38-639">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="24b38-640">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="24b38-640">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="24b38-641">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="24b38-641">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="24b38-642">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="24b38-642">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="24b38-643">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="24b38-643">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="24b38-644">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="24b38-644">Az.Monitor</span></span>
* <span data-ttu-id="24b38-645">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="24b38-645">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-646">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-646">Az.Network</span></span>
* <span data-ttu-id="24b38-647">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="24b38-647">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="24b38-648">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="24b38-648">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="24b38-649">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="24b38-649">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="24b38-650">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="24b38-650">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="24b38-651">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="24b38-651">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="24b38-652">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="24b38-652">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="24b38-653">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="24b38-653">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="24b38-654">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="24b38-654">Az.OperationalInsights</span></span>
* <span data-ttu-id="24b38-655">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="24b38-655">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="24b38-656">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="24b38-656">Added example</span></span>
    - <span data-ttu-id="24b38-657">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="24b38-657">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="24b38-658">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="24b38-658">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="24b38-659">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="24b38-659">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="24b38-660">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="24b38-660">Az.RecoveryServices</span></span>
* <span data-ttu-id="24b38-661">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="24b38-661">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-662">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-662">Az.Resources</span></span>
* <span data-ttu-id="24b38-663">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="24b38-663">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="24b38-664">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="24b38-664">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="24b38-665">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="24b38-665">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="24b38-666">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="24b38-666">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="24b38-667">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="24b38-667">Az.ServiceBus</span></span>
* <span data-ttu-id="24b38-668">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="24b38-668">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="24b38-669">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="24b38-669">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="24b38-670">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="24b38-670">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="24b38-671">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="24b38-671">Az.ServiceFabric</span></span>
* <span data-ttu-id="24b38-672">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="24b38-672">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="24b38-673">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="24b38-673">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="24b38-674">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="24b38-674">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="24b38-675">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="24b38-675">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="24b38-676">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="24b38-676">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="24b38-677">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="24b38-677">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-678">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-678">Az.Sql</span></span>
* <span data-ttu-id="24b38-679">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="24b38-679">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="24b38-680">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-680">Az.Storage</span></span>
* <span data-ttu-id="24b38-681">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="24b38-681">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="24b38-682">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="24b38-682">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="24b38-683">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="24b38-683">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="24b38-684">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="24b38-684">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="24b38-685">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="24b38-685">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="24b38-686">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="24b38-686">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="24b38-687">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="24b38-687">Az.Websites</span></span>
* <span data-ttu-id="24b38-688">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="24b38-688">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="24b38-689">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-689">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="24b38-690">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-690">Az.Accounts</span></span>
* <span data-ttu-id="24b38-691">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="24b38-691">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="24b38-692">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="24b38-692">Az.ApplicationInsights</span></span>
* <span data-ttu-id="24b38-693">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="24b38-693">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="24b38-694">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="24b38-694">Az.Automation</span></span>
* <span data-ttu-id="24b38-695">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="24b38-695">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="24b38-696">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="24b38-696">Az.CognitiveServices</span></span>
* <span data-ttu-id="24b38-697">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="24b38-697">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-698">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-698">Az.Compute</span></span>
* <span data-ttu-id="24b38-699">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="24b38-699">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="24b38-700">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="24b38-700">Az.ContainerRegistry</span></span>
* <span data-ttu-id="24b38-701">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="24b38-701">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="24b38-702">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="24b38-702">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="24b38-703">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="24b38-703">Az.DataFactory</span></span>
* <span data-ttu-id="24b38-704">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="24b38-704">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="24b38-705">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="24b38-705">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="24b38-706">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="24b38-706">Az.EventHub</span></span>
* <span data-ttu-id="24b38-707">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="24b38-707">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="24b38-708">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="24b38-708">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="24b38-709">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="24b38-709">Az.KeyVault</span></span>
* <span data-ttu-id="24b38-710">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="24b38-710">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="24b38-711">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="24b38-711">Az.LogicApp</span></span>
* <span data-ttu-id="24b38-712">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="24b38-712">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="24b38-713">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="24b38-713">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="24b38-714">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="24b38-714">Az.ManagedServices</span></span>
* <span data-ttu-id="24b38-715">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="24b38-715">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-716">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-716">Az.Network</span></span>
* <span data-ttu-id="24b38-717">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="24b38-717">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="24b38-718">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="24b38-718">New cmdlets</span></span>
        - <span data-ttu-id="24b38-719">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="24b38-719">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="24b38-720">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="24b38-720">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="24b38-721">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-721">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="24b38-722">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-722">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="24b38-723">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-723">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="24b38-724">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-724">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="24b38-725">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="24b38-725">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="24b38-726">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="24b38-726">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="24b38-727">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="24b38-727">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="24b38-728">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-728">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="24b38-729">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="24b38-729">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="24b38-730">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="24b38-730">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="24b38-731">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="24b38-731">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="24b38-732">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="24b38-732">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="24b38-733">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="24b38-733">Updated cmdlets</span></span>
        - <span data-ttu-id="24b38-734">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-734">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="24b38-735">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-735">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="24b38-736">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-736">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="24b38-737">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-737">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="24b38-738">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="24b38-738">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="24b38-739">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="24b38-739">Updated cmdlet:</span></span>
        - <span data-ttu-id="24b38-740">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-740">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="24b38-741">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-741">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="24b38-742">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-742">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="24b38-743">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="24b38-743">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="24b38-744">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="24b38-744">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="24b38-745">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="24b38-745">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="24b38-746">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="24b38-746">Az.OperationalInsights</span></span>
* <span data-ttu-id="24b38-747">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="24b38-747">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="24b38-748">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="24b38-748">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="24b38-749">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="24b38-749">Az.RecoveryServices</span></span>
* <span data-ttu-id="24b38-750">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="24b38-750">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="24b38-751">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="24b38-751">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="24b38-752">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="24b38-752">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="24b38-753">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="24b38-753">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="24b38-754">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="24b38-754">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="24b38-755">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="24b38-755">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="24b38-756">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="24b38-756">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="24b38-757">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="24b38-757">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="24b38-758">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="24b38-758">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="24b38-759">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="24b38-759">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-760">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-760">Az.Resources</span></span>
- <span data-ttu-id="24b38-761">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="24b38-761">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="24b38-762">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="24b38-762">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="24b38-763">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="24b38-763">Az.ServiceBus</span></span>
* <span data-ttu-id="24b38-764">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="24b38-764">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="24b38-765">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="24b38-765">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-766">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-766">Az.Sql</span></span>
* <span data-ttu-id="24b38-767">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="24b38-767">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="24b38-768">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="24b38-768">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="24b38-769">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="24b38-769">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="24b38-770">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-770">Az.Storage</span></span>
* <span data-ttu-id="24b38-771">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="24b38-771">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="24b38-772">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="24b38-772">Az.StorageSync</span></span>
* <span data-ttu-id="24b38-773">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="24b38-773">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="24b38-774">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="24b38-774">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="24b38-775">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="24b38-775">Az.Websites</span></span>
* <span data-ttu-id="24b38-776">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="24b38-776">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="24b38-777">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="24b38-777">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="24b38-778">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="24b38-778">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="24b38-779">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-779">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="24b38-780">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-780">Az.Accounts</span></span>
* <span data-ttu-id="24b38-781">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="24b38-781">Add support for profile cmdlets</span></span>
* <span data-ttu-id="24b38-782">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="24b38-782">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="24b38-783">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="24b38-783">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="24b38-784">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="24b38-784">Az.Advisor</span></span>
* <span data-ttu-id="24b38-785">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="24b38-785">GA release of Az.Advisor</span></span>
* <span data-ttu-id="24b38-786">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="24b38-786">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="24b38-787">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="24b38-787">Az.ApiManagement</span></span>
* <span data-ttu-id="24b38-788">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="24b38-788">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="24b38-789">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="24b38-789">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="24b38-790">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="24b38-790">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="24b38-791">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="24b38-791">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="24b38-792">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="24b38-792">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="24b38-793">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="24b38-793">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="24b38-794">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="24b38-794">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="24b38-795">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="24b38-795">Az.Automation</span></span>
* <span data-ttu-id="24b38-796">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="24b38-796">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-797">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-797">Az.Compute</span></span>
* <span data-ttu-id="24b38-798">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-798">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="24b38-799">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="24b38-799">Az.DataFactory</span></span>
* <span data-ttu-id="24b38-800">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="24b38-800">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="24b38-801">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="24b38-801">Az.EventGrid</span></span>
* <span data-ttu-id="24b38-802">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="24b38-802">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="24b38-803">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="24b38-803">Az.IotHub</span></span>
* <span data-ttu-id="24b38-804">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="24b38-804">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-805">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-805">Az.Network</span></span>
* <span data-ttu-id="24b38-806">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="24b38-806">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="24b38-807">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="24b38-807">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="24b38-808">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="24b38-808">Az.PolicyInsights</span></span>
* <span data-ttu-id="24b38-809">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="24b38-809">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="24b38-810">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="24b38-810">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="24b38-811">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="24b38-811">Az.OperationalInsights</span></span>
* <span data-ttu-id="24b38-812">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="24b38-812">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="24b38-813">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="24b38-813">Az.RecoveryServices</span></span>
* <span data-ttu-id="24b38-814">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="24b38-814">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-815">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-815">Az.Resources</span></span>
    - <span data-ttu-id="24b38-816">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="24b38-816">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="24b38-817">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="24b38-817">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="24b38-818">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="24b38-818">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="24b38-819">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="24b38-819">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="24b38-820">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="24b38-820">Az.ServiceBus</span></span>
* <span data-ttu-id="24b38-821">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="24b38-821">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-822">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-822">Az.Sql</span></span>
* <span data-ttu-id="24b38-823">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="24b38-823">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="24b38-824">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="24b38-824">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="24b38-825">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="24b38-825">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="24b38-826">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="24b38-826">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="24b38-827">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="24b38-827">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="24b38-828">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="24b38-828">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="24b38-829">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="24b38-829">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="24b38-830">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="24b38-830">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="24b38-831">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="24b38-831">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="24b38-832">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-832">Az.Storage</span></span>
* <span data-ttu-id="24b38-833">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="24b38-833">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="24b38-834">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="24b38-834">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="24b38-835">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="24b38-835">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="24b38-836">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="24b38-836">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="24b38-837">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="24b38-837">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="24b38-838">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="24b38-838">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="24b38-839">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="24b38-839">Set-AzStorageAccount</span></span>
* <span data-ttu-id="24b38-840">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="24b38-840">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="24b38-841">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="24b38-841">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="24b38-842">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="24b38-842">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="24b38-843">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="24b38-843">Az.StorageSync</span></span>
* <span data-ttu-id="24b38-844">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="24b38-844">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="24b38-845">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-845">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="24b38-846">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-846">Az.Accounts</span></span>
* <span data-ttu-id="24b38-847">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="24b38-847">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="24b38-848">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="24b38-848">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="24b38-849">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="24b38-849">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="24b38-850">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="24b38-850">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="24b38-851">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="24b38-851">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-852">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-852">Az.Compute</span></span>
* <span data-ttu-id="24b38-853">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="24b38-853">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="24b38-854">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="24b38-854">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="24b38-855">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="24b38-855">Az.Dns</span></span>
* <span data-ttu-id="24b38-856">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="24b38-856">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="24b38-857">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="24b38-857">Az.EventGrid</span></span>
* <span data-ttu-id="24b38-858">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="24b38-858">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="24b38-859">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="24b38-859">New cmdlets:</span></span>
    - <span data-ttu-id="24b38-860">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="24b38-860">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="24b38-861">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="24b38-861">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="24b38-862">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="24b38-862">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="24b38-863">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="24b38-863">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="24b38-864">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="24b38-864">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="24b38-865">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="24b38-865">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="24b38-866">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="24b38-866">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="24b38-867">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="24b38-867">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="24b38-868">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="24b38-868">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="24b38-869">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="24b38-869">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="24b38-870">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="24b38-870">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="24b38-871">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="24b38-871">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="24b38-872">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="24b38-872">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="24b38-873">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="24b38-873">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="24b38-874">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="24b38-874">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="24b38-875">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="24b38-875">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="24b38-876">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="24b38-876">Updated cmdlets:</span></span>
    - <span data-ttu-id="24b38-877">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="24b38-877">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="24b38-878">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="24b38-878">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="24b38-879">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="24b38-879">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="24b38-880">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="24b38-880">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="24b38-881">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="24b38-881">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="24b38-882">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="24b38-882">Event subscription expiration date,</span></span>
            - <span data-ttu-id="24b38-883">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="24b38-883">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="24b38-884">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="24b38-884">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="24b38-885">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="24b38-885">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="24b38-886">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="24b38-886">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="24b38-887">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="24b38-887">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="24b38-888">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="24b38-888">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="24b38-889">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="24b38-889">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="24b38-890">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="24b38-890">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="24b38-891">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="24b38-891">Az.FrontDoor</span></span>
* <span data-ttu-id="24b38-892">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="24b38-892">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="24b38-893">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="24b38-893">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="24b38-894">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="24b38-894">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="24b38-895">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="24b38-895">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-896">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-896">Az.Network</span></span>
* <span data-ttu-id="24b38-897">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="24b38-897">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="24b38-898">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="24b38-898">New cmdlets</span></span>
        - <span data-ttu-id="24b38-899">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="24b38-899">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="24b38-900">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="24b38-900">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="24b38-901">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="24b38-901">New cmdlets</span></span> 
        - <span data-ttu-id="24b38-902">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="24b38-902">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="24b38-903">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="24b38-903">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="24b38-904">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="24b38-904">New cmdlets</span></span> 
        - <span data-ttu-id="24b38-905">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="24b38-905">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="24b38-906">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="24b38-906">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="24b38-907">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="24b38-907">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="24b38-908">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-908">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="24b38-909">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-909">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="24b38-910">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="24b38-910">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="24b38-911">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="24b38-911">New cmdlets</span></span>
        - <span data-ttu-id="24b38-912">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="24b38-912">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="24b38-913">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="24b38-913">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="24b38-914">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="24b38-914">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="24b38-915">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-915">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="24b38-916">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="24b38-916">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="24b38-917">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="24b38-917">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="24b38-918">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="24b38-918">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="24b38-919">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="24b38-919">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="24b38-920">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="24b38-920">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="24b38-921">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="24b38-921">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="24b38-922">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="24b38-922">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="24b38-923">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="24b38-923">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="24b38-924">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="24b38-924">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="24b38-925">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="24b38-925">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="24b38-926">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="24b38-926">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="24b38-927">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="24b38-927">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="24b38-928">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="24b38-928">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="24b38-929">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="24b38-929">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="24b38-930">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="24b38-930">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="24b38-931">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="24b38-931">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="24b38-932">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="24b38-932">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="24b38-933">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="24b38-933">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="24b38-934">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="24b38-934">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="24b38-935">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="24b38-935">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="24b38-936">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="24b38-936">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="24b38-937">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="24b38-937">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="24b38-938">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="24b38-938">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="24b38-939">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="24b38-939">Az.OperationalInsights</span></span>
* <span data-ttu-id="24b38-940">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="24b38-940">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-941">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-941">Az.Resources</span></span>
* <span data-ttu-id="24b38-942">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="24b38-942">Support for additional Template Export options</span></span>
    - <span data-ttu-id="24b38-943">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="24b38-943">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="24b38-944">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="24b38-944">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="24b38-945">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="24b38-945">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="24b38-946">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="24b38-946">Az.ServiceFabric</span></span>
* <span data-ttu-id="24b38-947">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="24b38-947">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-948">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-948">Az.Sql</span></span>
* <span data-ttu-id="24b38-949">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="24b38-949">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="24b38-950">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="24b38-950">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="24b38-951">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="24b38-951">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="24b38-952">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="24b38-952">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="24b38-953">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="24b38-953">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="24b38-954">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="24b38-954">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="24b38-955">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="24b38-955">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="24b38-956">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="24b38-956">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="24b38-957">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-957">Az.Storage</span></span>
* <span data-ttu-id="24b38-958">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="24b38-958">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="24b38-959">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="24b38-959">New-AzStorageAccount</span></span>
* <span data-ttu-id="24b38-960">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="24b38-960">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="24b38-961">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="24b38-961">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="24b38-962">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="24b38-962">Az.Websites</span></span>
* <span data-ttu-id="24b38-963">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="24b38-963">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="24b38-964">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="24b38-964">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="24b38-965">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-965">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="24b38-966">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="24b38-966">Az.Cdn</span></span>
* <span data-ttu-id="24b38-967">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="24b38-967">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-968">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-968">Az.Compute</span></span>
* <span data-ttu-id="24b38-969">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="24b38-969">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="24b38-970">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="24b38-970">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="24b38-971">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="24b38-971">Az.EventHub</span></span>
* <span data-ttu-id="24b38-972">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="24b38-972">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="24b38-973">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="24b38-973">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-974">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-974">Az.Network</span></span>
* <span data-ttu-id="24b38-975">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="24b38-975">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="24b38-976">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="24b38-976">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="24b38-977">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="24b38-977">Az.PolicyInsights</span></span>
* <span data-ttu-id="24b38-978">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="24b38-978">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="24b38-979">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="24b38-979">Az.RecoveryServices</span></span>
* <span data-ttu-id="24b38-980">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="24b38-980">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="24b38-981">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="24b38-981">Az.ServiceBus</span></span>
* <span data-ttu-id="24b38-982">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="24b38-982">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="24b38-983">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="24b38-983">Az.ServiceFabric</span></span>
* <span data-ttu-id="24b38-984">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="24b38-984">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="24b38-985">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="24b38-985">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-986">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-986">Az.Sql</span></span>
* <span data-ttu-id="24b38-987">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="24b38-987">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="24b38-988">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="24b38-988">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="24b38-989">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="24b38-989">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="24b38-990">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="24b38-990">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="24b38-991">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="24b38-991">Az.Websites</span></span>
* <span data-ttu-id="24b38-992">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="24b38-992">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="24b38-993">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-993">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="24b38-994">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="24b38-994">Az.ApiManagement</span></span>
* <span data-ttu-id="24b38-995">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="24b38-995">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="24b38-996">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="24b38-996">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="24b38-997">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="24b38-997">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="24b38-998">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="24b38-998">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="24b38-999">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="24b38-999">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="24b38-1000">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="24b38-1000">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="24b38-1001">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="24b38-1001">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="24b38-1002">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="24b38-1002">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="24b38-1003">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="24b38-1003">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="24b38-1004">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="24b38-1004">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="24b38-1005">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="24b38-1005">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="24b38-1006">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="24b38-1006">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="24b38-1007">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="24b38-1007">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="24b38-1008">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="24b38-1008">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="24b38-1009">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="24b38-1009">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="24b38-1010">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="24b38-1010">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="24b38-1011">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="24b38-1011">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="24b38-1012">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="24b38-1012">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="24b38-1013">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="24b38-1013">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="24b38-1014">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="24b38-1014">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="24b38-1015">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="24b38-1015">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="24b38-1016">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="24b38-1016">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="24b38-1017">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="24b38-1017">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="24b38-1018">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="24b38-1018">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="24b38-1019">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="24b38-1019">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="24b38-1020">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="24b38-1020">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="24b38-1021">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="24b38-1021">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="24b38-1022">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="24b38-1022">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="24b38-1023">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="24b38-1023">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="24b38-1024">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="24b38-1024">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="24b38-1025">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="24b38-1025">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="24b38-1026">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="24b38-1026">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="24b38-1027">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="24b38-1027">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="24b38-1028">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="24b38-1028">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="24b38-1029">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="24b38-1029">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="24b38-1030">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="24b38-1030">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="24b38-1031">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="24b38-1031">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="24b38-1032">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="24b38-1032">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="24b38-1033">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="24b38-1033">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="24b38-1034">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="24b38-1034">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="24b38-1035">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="24b38-1035">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="24b38-1036">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="24b38-1036">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="24b38-1037">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="24b38-1037">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="24b38-1038">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="24b38-1038">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="24b38-1039">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="24b38-1039">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="24b38-1040">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="24b38-1040">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="24b38-1041">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="24b38-1041">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="24b38-1042">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="24b38-1042">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="24b38-1043">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="24b38-1043">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="24b38-1044">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="24b38-1044">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="24b38-1045">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="24b38-1045">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="24b38-1046">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="24b38-1046">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="24b38-1047">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="24b38-1047">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="24b38-1048">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="24b38-1048">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="24b38-1049">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="24b38-1049">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="24b38-1050">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="24b38-1050">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="24b38-1051">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="24b38-1051">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="24b38-1052">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="24b38-1052">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="24b38-1053">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="24b38-1053">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="24b38-1054">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="24b38-1054">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="24b38-1055">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="24b38-1055">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="24b38-1056">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="24b38-1056">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="24b38-1057">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="24b38-1057">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="24b38-1058">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="24b38-1058">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="24b38-1059">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="24b38-1059">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="24b38-1060">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="24b38-1060">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="24b38-1061">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="24b38-1061">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="24b38-1062">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="24b38-1062">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="24b38-1063">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="24b38-1063">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="24b38-1064">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="24b38-1064">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="24b38-1065">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="24b38-1065">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="24b38-1066">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="24b38-1066">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="24b38-1067">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="24b38-1067">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="24b38-1068">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="24b38-1068">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="24b38-1069">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="24b38-1069">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="24b38-1070">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="24b38-1070">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="24b38-1071">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="24b38-1071">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="24b38-1072">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="24b38-1072">Az.Automation</span></span>
* <span data-ttu-id="24b38-1073">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="24b38-1073">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="24b38-1074">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="24b38-1074">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="24b38-1075">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="24b38-1075">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="24b38-1076">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="24b38-1076">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="24b38-1077">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="24b38-1077">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="24b38-1078">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="24b38-1078">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="24b38-1079">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="24b38-1079">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-1080">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-1080">Az.Compute</span></span>
* <span data-ttu-id="24b38-1081">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="24b38-1081">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="24b38-1082">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="24b38-1082">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="24b38-1083">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="24b38-1083">Az.DataLakeStore</span></span>
* <span data-ttu-id="24b38-1084">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="24b38-1084">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="24b38-1085">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="24b38-1085">Az.Monitor</span></span>
* <span data-ttu-id="24b38-1086">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="24b38-1086">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-1087">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1087">Az.Network</span></span>
* <span data-ttu-id="24b38-1088">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="24b38-1088">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="24b38-1089">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="24b38-1089">Updated cmdlet:</span></span>
        - <span data-ttu-id="24b38-1090">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="24b38-1090">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="24b38-1091">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="24b38-1091">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-1092">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-1092">Az.Resources</span></span>
* <span data-ttu-id="24b38-1093">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="24b38-1093">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-1094">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-1094">Az.Sql</span></span>
* <span data-ttu-id="24b38-1095">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="24b38-1095">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="24b38-1096">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-1096">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="24b38-1097">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-1097">Az.Accounts</span></span>
* <span data-ttu-id="24b38-1098">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="24b38-1098">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="24b38-1099">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1099">Az.CognitiveServices</span></span>
* <span data-ttu-id="24b38-1100">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="24b38-1100">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="24b38-1101">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="24b38-1101">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-1102">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-1102">Az.Compute</span></span>
* <span data-ttu-id="24b38-1103">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="24b38-1103">Proximity placement group feature.</span></span>
    - <span data-ttu-id="24b38-1104">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="24b38-1104">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="24b38-1105">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-1105">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="24b38-1106">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="24b38-1106">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="24b38-1107">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="24b38-1107">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="24b38-1108">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="24b38-1108">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="24b38-1109">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="24b38-1109">Breaking changes</span></span>
    - <span data-ttu-id="24b38-1110">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="24b38-1110">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="24b38-1111">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="24b38-1111">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="24b38-1112">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="24b38-1112">Az.DeploymentManager</span></span>
* <span data-ttu-id="24b38-1113">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="24b38-1113">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="24b38-1114">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="24b38-1114">Az.Dns</span></span>
* <span data-ttu-id="24b38-1115">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="24b38-1115">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="24b38-1116">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="24b38-1116">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="24b38-1117">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="24b38-1117">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="24b38-1118">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="24b38-1118">Az.FrontDoor</span></span>
* <span data-ttu-id="24b38-1119">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="24b38-1119">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="24b38-1120">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="24b38-1120">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="24b38-1121">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="24b38-1121">Az.HDInsight</span></span>
* <span data-ttu-id="24b38-1122">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="24b38-1122">Removed two cmdlets:</span></span>
    - <span data-ttu-id="24b38-1123">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="24b38-1123">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="24b38-1124">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="24b38-1124">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="24b38-1125">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="24b38-1125">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="24b38-1126">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="24b38-1126">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="24b38-1127">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="24b38-1127">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="24b38-1128">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="24b38-1128">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="24b38-1129">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="24b38-1129">Az.Monitor</span></span>
* <span data-ttu-id="24b38-1130">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="24b38-1130">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="24b38-1131">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="24b38-1131">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="24b38-1132">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="24b38-1132">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="24b38-1133">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="24b38-1133">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="24b38-1134">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="24b38-1134">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="24b38-1135">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="24b38-1135">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="24b38-1136">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="24b38-1136">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="24b38-1137">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="24b38-1137">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="24b38-1138">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="24b38-1138">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="24b38-1139">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="24b38-1139">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="24b38-1140">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="24b38-1140">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="24b38-1141">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="24b38-1141">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="24b38-1142">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="24b38-1142">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="24b38-1143">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="24b38-1143">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-1144">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1144">Az.Network</span></span>
* <span data-ttu-id="24b38-1145">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="24b38-1145">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="24b38-1146">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="24b38-1146">New cmdlets</span></span>
        - <span data-ttu-id="24b38-1147">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="24b38-1147">New-AzNatGateway</span></span>
        - <span data-ttu-id="24b38-1148">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="24b38-1148">Get-AzNatGateway</span></span>
        - <span data-ttu-id="24b38-1149">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="24b38-1149">Set-AzNatGateway</span></span>
        - <span data-ttu-id="24b38-1150">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="24b38-1150">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="24b38-1151">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="24b38-1151">Updated cmdlets</span></span>
        - <span data-ttu-id="24b38-1152">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="24b38-1152">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="24b38-1153">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="24b38-1153">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="24b38-1154">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="24b38-1154">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="24b38-1155">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="24b38-1155">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="24b38-1156">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="24b38-1156">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="24b38-1157">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="24b38-1157">Az.PolicyInsights</span></span>
* <span data-ttu-id="24b38-1158">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="24b38-1158">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="24b38-1159">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="24b38-1159">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="24b38-1160">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="24b38-1160">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="24b38-1161">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1161">Az.RecoveryServices</span></span>
* <span data-ttu-id="24b38-1162">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="24b38-1162">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="24b38-1163">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="24b38-1163">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="24b38-1164">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="24b38-1164">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="24b38-1165">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="24b38-1165">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="24b38-1166">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="24b38-1166">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="24b38-1167">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="24b38-1167">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="24b38-1168">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="24b38-1168">Az.Relay</span></span>
* <span data-ttu-id="24b38-1169">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="24b38-1169">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="24b38-1170">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="24b38-1170">Az.ServiceBus</span></span>
* <span data-ttu-id="24b38-1171">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="24b38-1171">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="24b38-1172">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-1172">Az.Storage</span></span>
* <span data-ttu-id="24b38-1173">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage.*" para "Microsoft.Azure.Storage.*")</span><span class="sxs-lookup"><span data-stu-id="24b38-1173">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="24b38-1174">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="24b38-1174">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="24b38-1175">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="24b38-1175">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="24b38-1176">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="24b38-1176">New-AzStorageAccount</span></span>
* <span data-ttu-id="24b38-1177">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="24b38-1177">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="24b38-1178">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="24b38-1178">New-AzStorageAccount</span></span>
    - <span data-ttu-id="24b38-1179">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="24b38-1179">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="24b38-1180">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="24b38-1180">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="24b38-1181">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="24b38-1181">Az.Websites</span></span>
* <span data-ttu-id="24b38-1182">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="24b38-1182">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="24b38-1183">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="24b38-1183">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="24b38-1184">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-1184">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="24b38-1185">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="24b38-1185">Highlights since the last major release</span></span>
* <span data-ttu-id="24b38-1186">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="24b38-1186">General availability of `Az` module</span></span>
* <span data-ttu-id="24b38-1187">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="24b38-1187">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="24b38-1188">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="24b38-1188">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="24b38-1189">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1189">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="24b38-1190">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="24b38-1190">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="24b38-1191">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="24b38-1191">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="24b38-1192">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="24b38-1192">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="24b38-1193">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-1193">Az.Accounts</span></span>
* <span data-ttu-id="24b38-1194">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="24b38-1194">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="24b38-1195">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="24b38-1195">Az.Batch</span></span>
* <span data-ttu-id="24b38-1196">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1196">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="24b38-1197">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="24b38-1197">Az.Cdn</span></span>
* <span data-ttu-id="24b38-1198">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1198">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="24b38-1199">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1199">Az.CognitiveServices</span></span>
* <span data-ttu-id="24b38-1200">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1200">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-1201">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-1201">Az.Compute</span></span>
* <span data-ttu-id="24b38-1202">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="24b38-1202">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="24b38-1203">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1203">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="24b38-1204">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="24b38-1204">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="24b38-1205">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="24b38-1205">Az.DataFactory</span></span>
* <span data-ttu-id="24b38-1206">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="24b38-1206">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="24b38-1207">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="24b38-1207">Az.DataLakeStore</span></span>
* <span data-ttu-id="24b38-1208">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1208">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="24b38-1209">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="24b38-1209">Az.EventGrid</span></span>
* <span data-ttu-id="24b38-1210">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="24b38-1210">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="24b38-1211">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="24b38-1211">Az.EventHub</span></span>
* <span data-ttu-id="24b38-1212">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="24b38-1212">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="24b38-1213">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="24b38-1213">Az.HDInsight</span></span>
* <span data-ttu-id="24b38-1214">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1214">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="24b38-1215">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="24b38-1215">Az.IotHub</span></span>
* <span data-ttu-id="24b38-1216">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1216">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="24b38-1217">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="24b38-1217">Az.KeyVault</span></span>
* <span data-ttu-id="24b38-1218">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1218">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="24b38-1219">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="24b38-1219">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="24b38-1220">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="24b38-1220">Az.MachineLearning</span></span>
* <span data-ttu-id="24b38-1221">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1221">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="24b38-1222">Az.Media</span><span class="sxs-lookup"><span data-stu-id="24b38-1222">Az.Media</span></span>
* <span data-ttu-id="24b38-1223">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1223">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="24b38-1224">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="24b38-1224">Az.Monitor</span></span>
  * <span data-ttu-id="24b38-1225">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="24b38-1225">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="24b38-1226">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="24b38-1226">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="24b38-1227">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="24b38-1227">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="24b38-1228">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="24b38-1228">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="24b38-1229">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="24b38-1229">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="24b38-1230">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="24b38-1230">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="24b38-1231">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="24b38-1231">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-1232">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1232">Az.Network</span></span>
* <span data-ttu-id="24b38-1233">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1233">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="24b38-1234">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="24b38-1234">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="24b38-1235">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="24b38-1235">Az.NotificationHubs</span></span>
* <span data-ttu-id="24b38-1236">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1236">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="24b38-1237">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="24b38-1237">Az.OperationalInsights</span></span>
* <span data-ttu-id="24b38-1238">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1238">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="24b38-1239">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="24b38-1239">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="24b38-1240">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1240">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="24b38-1241">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1241">Az.RecoveryServices</span></span>
* <span data-ttu-id="24b38-1242">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1242">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="24b38-1243">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="24b38-1243">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="24b38-1244">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="24b38-1244">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="24b38-1245">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="24b38-1245">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="24b38-1246">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="24b38-1246">Az.RedisCache</span></span>
* <span data-ttu-id="24b38-1247">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1247">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-1248">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-1248">Az.Resources</span></span>
* <span data-ttu-id="24b38-1249">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="24b38-1249">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-1250">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-1250">Az.Sql</span></span>
* <span data-ttu-id="24b38-1251">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="24b38-1251">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="24b38-1252">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1252">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="24b38-1253">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="24b38-1253">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="24b38-1254">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="24b38-1254">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="24b38-1255">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="24b38-1255">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="24b38-1256">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="24b38-1256">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="24b38-1257">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="24b38-1257">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="24b38-1258">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="24b38-1258">Az.Websites</span></span>
* <span data-ttu-id="24b38-1259">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="24b38-1259">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="24b38-1260">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="24b38-1260">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="24b38-1261">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="24b38-1261">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="24b38-1262">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="24b38-1262">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="24b38-1263">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-1263">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="24b38-1264">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="24b38-1264">Highlights since the last major release</span></span>
* <span data-ttu-id="24b38-1265">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="24b38-1265">General availability of `Az` module</span></span>
* <span data-ttu-id="24b38-1266">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="24b38-1266">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="24b38-1267">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="24b38-1267">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="24b38-1268">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1268">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="24b38-1269">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="24b38-1269">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="24b38-1270">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="24b38-1270">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="24b38-1271">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="24b38-1271">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="24b38-1272">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-1272">Az.Accounts</span></span>
* <span data-ttu-id="24b38-1273">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="24b38-1273">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="24b38-1274">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1274">Az.AnalysisServices</span></span>
* <span data-ttu-id="24b38-1275">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="24b38-1275">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="24b38-1276">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="24b38-1276">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="24b38-1277">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="24b38-1277">Az.Automation</span></span>
* <span data-ttu-id="24b38-1278">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="24b38-1278">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="24b38-1279">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="24b38-1279">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="24b38-1280">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="24b38-1280">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-1281">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-1281">Az.Compute</span></span>
* <span data-ttu-id="24b38-1282">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-1282">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="24b38-1283">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="24b38-1283">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="24b38-1284">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="24b38-1284">Az.ContainerInstance</span></span>
* <span data-ttu-id="24b38-1285">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="24b38-1285">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="24b38-1286">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="24b38-1286">Az.DataFactory</span></span>
* <span data-ttu-id="24b38-1287">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="24b38-1287">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="24b38-1288">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="24b38-1288">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-1289">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-1289">Az.Resources</span></span>
* <span data-ttu-id="24b38-1290">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="24b38-1290">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="24b38-1291">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="24b38-1291">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="24b38-1292">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="24b38-1292">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="24b38-1293">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="24b38-1293">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="24b38-1294">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="24b38-1294">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="24b38-1295">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="24b38-1295">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-1296">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-1296">Az.Sql</span></span>
* <span data-ttu-id="24b38-1297">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="24b38-1297">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="24b38-1298">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-1298">Az.Storage</span></span>
* <span data-ttu-id="24b38-1299">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="24b38-1299">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="24b38-1300">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="24b38-1300">New-AzStorageContext</span></span>
* <span data-ttu-id="24b38-1301">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="24b38-1301">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="24b38-1302">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="24b38-1302">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="24b38-1303">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="24b38-1303">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="24b38-1304">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="24b38-1304">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="24b38-1305">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="24b38-1305">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="24b38-1306">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="24b38-1306">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="24b38-1307">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="24b38-1307">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="24b38-1308">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="24b38-1308">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="24b38-1309">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="24b38-1309">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="24b38-1310">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="24b38-1310">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="24b38-1311">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-1311">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="24b38-1312">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="24b38-1312">Highlights since the last major release</span></span>
* <span data-ttu-id="24b38-1313">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="24b38-1313">General availability of `Az` module</span></span>
* <span data-ttu-id="24b38-1314">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="24b38-1314">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="24b38-1315">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="24b38-1315">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="24b38-1316">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1316">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="24b38-1317">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="24b38-1317">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="24b38-1318">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="24b38-1318">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="24b38-1319">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="24b38-1319">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="24b38-1320">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="24b38-1320">Az.Automation</span></span>
* <span data-ttu-id="24b38-1321">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="24b38-1321">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="24b38-1322">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="24b38-1322">Dynamic grouping</span></span>
    * <span data-ttu-id="24b38-1323">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="24b38-1323">Pre-Post script</span></span>
    * <span data-ttu-id="24b38-1324">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="24b38-1324">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-1325">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-1325">Az.Compute</span></span>
* <span data-ttu-id="24b38-1326">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="24b38-1326">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="24b38-1327">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="24b38-1327">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="24b38-1328">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="24b38-1328">Az.KeyVault</span></span>
* <span data-ttu-id="24b38-1329">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="24b38-1329">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-1330">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1330">Az.Network</span></span>
* <span data-ttu-id="24b38-1331">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="24b38-1331">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="24b38-1332">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="24b38-1332">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="24b38-1333">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1333">Az.RecoveryServices</span></span>
* <span data-ttu-id="24b38-1334">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="24b38-1334">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="24b38-1335">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="24b38-1335">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-1336">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-1336">Az.Resources</span></span>
* <span data-ttu-id="24b38-1337">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="24b38-1337">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="24b38-1338">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="24b38-1338">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-1339">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-1339">Az.Sql</span></span>
* <span data-ttu-id="24b38-1340">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="24b38-1340">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="24b38-1341">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-1341">Az.Storage</span></span>
* <span data-ttu-id="24b38-1342">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="24b38-1342">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="24b38-1343">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="24b38-1343">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="24b38-1344">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="24b38-1344">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="24b38-1345">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="24b38-1345">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="24b38-1346">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="24b38-1346">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="24b38-1347">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="24b38-1347">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="24b38-1348">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="24b38-1348">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="24b38-1349">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="24b38-1349">Az.Websites</span></span>
* <span data-ttu-id="24b38-1350">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="24b38-1350">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="24b38-1351">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-1351">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="24b38-1352">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-1352">Az.Accounts</span></span>
* <span data-ttu-id="24b38-1353">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="24b38-1353">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="24b38-1354">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="24b38-1354">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="24b38-1355">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="24b38-1355">Az.Automation</span></span>
* <span data-ttu-id="24b38-1356">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="24b38-1356">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="24b38-1357">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="24b38-1357">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="24b38-1358">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="24b38-1358">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="24b38-1359">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="24b38-1359">Az.Cdn</span></span>
* <span data-ttu-id="24b38-1360">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="24b38-1360">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-1361">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-1361">Az.Compute</span></span>
* <span data-ttu-id="24b38-1362">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="24b38-1362">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="24b38-1363">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="24b38-1363">Az.DataFactory</span></span>
* <span data-ttu-id="24b38-1364">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="24b38-1364">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="24b38-1365">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="24b38-1365">Az.LogicApp</span></span>
* <span data-ttu-id="24b38-1366">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="24b38-1366">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-1367">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1367">Az.Network</span></span>
* <span data-ttu-id="24b38-1368">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1368">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="24b38-1369">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1369">Az.RecoveryServices</span></span>
* <span data-ttu-id="24b38-1370">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="24b38-1370">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="24b38-1371">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="24b38-1371">SDK Update</span></span>
* <span data-ttu-id="24b38-1372">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="24b38-1372">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="24b38-1373">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="24b38-1373">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-1374">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-1374">Az.Resources</span></span>
* <span data-ttu-id="24b38-1375">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="24b38-1375">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="24b38-1376">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="24b38-1376">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="24b38-1377">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="24b38-1377">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="24b38-1378">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="24b38-1378">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="24b38-1379">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="24b38-1379">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="24b38-1380">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="24b38-1380">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-1381">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-1381">Az.Sql</span></span>
* <span data-ttu-id="24b38-1382">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="24b38-1382">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="24b38-1383">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="24b38-1383">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="24b38-1384">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-1384">Az.Storage</span></span>
* <span data-ttu-id="24b38-1385">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="24b38-1385">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="24b38-1386">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-1386">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="24b38-1387">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1387">Az.AnalysisServices</span></span>
* <span data-ttu-id="24b38-1388">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="24b38-1388">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="24b38-1389">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="24b38-1389">Az.Automation</span></span>
* <span data-ttu-id="24b38-1390">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="24b38-1390">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="24b38-1391">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="24b38-1391">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="24b38-1392">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="24b38-1392">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="24b38-1393">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1393">Az.CognitiveServices</span></span>
* <span data-ttu-id="24b38-1394">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="24b38-1394">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-1395">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-1395">Az.Compute</span></span>
* <span data-ttu-id="24b38-1396">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="24b38-1396">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="24b38-1397">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="24b38-1397">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="24b38-1398">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="24b38-1398">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="24b38-1399">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="24b38-1399">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="24b38-1400">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="24b38-1400">Az.DataLakeStore</span></span>
* <span data-ttu-id="24b38-1401">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="24b38-1401">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="24b38-1402">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="24b38-1402">Az.EventHub</span></span>
* <span data-ttu-id="24b38-1403">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="24b38-1403">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="24b38-1404">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="24b38-1404">Az.KeyVault</span></span>
* <span data-ttu-id="24b38-1405">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="24b38-1405">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="24b38-1406">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="24b38-1406">Az.LogicApp</span></span>
* <span data-ttu-id="24b38-1407">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="24b38-1407">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="24b38-1408">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="24b38-1408">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="24b38-1409">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="24b38-1409">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="24b38-1410">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="24b38-1410">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="24b38-1411">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="24b38-1411">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="24b38-1412">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="24b38-1412">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="24b38-1413">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="24b38-1413">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="24b38-1414">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="24b38-1414">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="24b38-1415">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="24b38-1415">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="24b38-1416">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="24b38-1416">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="24b38-1417">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="24b38-1417">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="24b38-1418">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="24b38-1418">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="24b38-1419">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="24b38-1419">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="24b38-1420">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="24b38-1420">Az.Monitor</span></span>
* <span data-ttu-id="24b38-1421">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="24b38-1421">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-1422">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1422">Az.Network</span></span>
* <span data-ttu-id="24b38-1423">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="24b38-1423">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="24b38-1424">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="24b38-1424">Az.OperationalInsights</span></span>
* <span data-ttu-id="24b38-1425">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="24b38-1425">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="24b38-1426">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="24b38-1426">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="24b38-1427">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="24b38-1427">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="24b38-1428">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-1428">Az.Resources</span></span>
* <span data-ttu-id="24b38-1429">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="24b38-1429">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="24b38-1430">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="24b38-1430">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="24b38-1431">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="24b38-1431">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="24b38-1432">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="24b38-1432">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-1433">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-1433">Az.Sql</span></span>
* <span data-ttu-id="24b38-1434">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="24b38-1434">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="24b38-1435">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="24b38-1435">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="24b38-1436">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="24b38-1436">Az.Websites</span></span>
* <span data-ttu-id="24b38-1437">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="24b38-1437">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="24b38-1438">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-1438">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="24b38-1439">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-1439">Az.Accounts</span></span>
* <span data-ttu-id="24b38-1440">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="24b38-1440">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="24b38-1441">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1441">Az.AnalysisServices</span></span>
<span data-ttu-id="24b38-1442">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="24b38-1442">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-1443">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-1443">Az.Compute</span></span>
* <span data-ttu-id="24b38-1444">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="24b38-1444">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="24b38-1445">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="24b38-1445">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="24b38-1446">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="24b38-1446">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="24b38-1447">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1447">Az.RecoveryServices</span></span>
<span data-ttu-id="24b38-1448">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="24b38-1448">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-1449">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-1449">Az.Resources</span></span>
* <span data-ttu-id="24b38-1450">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="24b38-1450">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="24b38-1451">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="24b38-1451">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="24b38-1452">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="24b38-1452">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="24b38-1453">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="24b38-1453">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-1454">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-1454">Az.Sql</span></span>
* <span data-ttu-id="24b38-1455">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="24b38-1455">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="24b38-1456">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="24b38-1456">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="24b38-1457">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="24b38-1457">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="24b38-1458">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-1458">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="24b38-1459">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-1459">Az.Accounts</span></span>
* <span data-ttu-id="24b38-1460">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="24b38-1460">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="24b38-1461">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1461">Az.AnalysisServices</span></span>
* <span data-ttu-id="24b38-1462">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="24b38-1462">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="24b38-1463">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1463">Az.RecoveryServices</span></span>
* <span data-ttu-id="24b38-1464">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="24b38-1464">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="24b38-1465">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-1465">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="24b38-1466">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-1466">Az.Accounts</span></span>
* <span data-ttu-id="24b38-1467">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="24b38-1467">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="24b38-1468">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="24b38-1468">Update incorrect online help URLs</span></span>
* <span data-ttu-id="24b38-1469">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="24b38-1469">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="24b38-1470">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="24b38-1470">Az.Aks</span></span>
* <span data-ttu-id="24b38-1471">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="24b38-1471">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="24b38-1472">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="24b38-1472">Az.Automation</span></span>
* <span data-ttu-id="24b38-1473">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="24b38-1473">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="24b38-1474">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="24b38-1474">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="24b38-1475">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="24b38-1475">Az.Cdn</span></span>
* <span data-ttu-id="24b38-1476">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="24b38-1476">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-1477">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-1477">Az.Compute</span></span>
* <span data-ttu-id="24b38-1478">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="24b38-1478">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="24b38-1479">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="24b38-1479">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="24b38-1480">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="24b38-1480">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="24b38-1481">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="24b38-1481">Az.ContainerRegistry</span></span>
* <span data-ttu-id="24b38-1482">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="24b38-1482">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="24b38-1483">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="24b38-1483">Az.DataFactory</span></span>
* <span data-ttu-id="24b38-1484">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="24b38-1484">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="24b38-1485">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="24b38-1485">Az.DataLakeStore</span></span>
* <span data-ttu-id="24b38-1486">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="24b38-1486">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="24b38-1487">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="24b38-1487">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="24b38-1488">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="24b38-1488">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="24b38-1489">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="24b38-1489">Az.IotHub</span></span>
* <span data-ttu-id="24b38-1490">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="24b38-1490">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="24b38-1491">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="24b38-1491">Az.KeyVault</span></span>
* <span data-ttu-id="24b38-1492">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="24b38-1492">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-1493">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1493">Az.Network</span></span>
* <span data-ttu-id="24b38-1494">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="24b38-1494">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-1495">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-1495">Az.Resources</span></span>
* <span data-ttu-id="24b38-1496">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="24b38-1496">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="24b38-1497">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="24b38-1497">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="24b38-1498">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="24b38-1498">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="24b38-1499">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="24b38-1499">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="24b38-1500">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="24b38-1500">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="24b38-1501">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="24b38-1501">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="24b38-1502">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="24b38-1502">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="24b38-1503">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="24b38-1503">Az.ServiceFabric</span></span>
* <span data-ttu-id="24b38-1504">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="24b38-1504">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="24b38-1505">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="24b38-1505">Fix some error messages.</span></span>
* <span data-ttu-id="24b38-1506">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="24b38-1506">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="24b38-1507">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="24b38-1507">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="24b38-1508">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="24b38-1508">Az.SignalR</span></span>
* <span data-ttu-id="24b38-1509">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="24b38-1509">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-1510">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-1510">Az.Sql</span></span>
* <span data-ttu-id="24b38-1511">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="24b38-1511">Update incorrect online help URLs</span></span>
* <span data-ttu-id="24b38-1512">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="24b38-1512">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="24b38-1513">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="24b38-1513">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="24b38-1514">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="24b38-1514">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="24b38-1515">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-1515">Az.Storage</span></span>
* <span data-ttu-id="24b38-1516">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="24b38-1516">Update incorrect online help URLs</span></span>
* <span data-ttu-id="24b38-1517">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="24b38-1517">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="24b38-1518">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="24b38-1518">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="24b38-1519">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="24b38-1519">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="24b38-1520">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="24b38-1520">Az.TrafficManager</span></span>
* <span data-ttu-id="24b38-1521">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="24b38-1521">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="24b38-1522">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="24b38-1522">Az.Websites</span></span>
* <span data-ttu-id="24b38-1523">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="24b38-1523">Update incorrect online help URLs</span></span>
* <span data-ttu-id="24b38-1524">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="24b38-1524">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="24b38-1525">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="24b38-1525">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="24b38-1526">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="24b38-1526">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="24b38-1527">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-1527">Az.Accounts</span></span>
* <span data-ttu-id="24b38-1528">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="24b38-1528">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-1529">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-1529">Az.Compute</span></span>
* <span data-ttu-id="24b38-1530">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="24b38-1530">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="24b38-1531">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="24b38-1531">Updated the description of ID in help files</span></span>
* <span data-ttu-id="24b38-1532">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-1532">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="24b38-1533">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="24b38-1533">Az.DataLakeStore</span></span>
* <span data-ttu-id="24b38-1534">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="24b38-1534">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="24b38-1535">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="24b38-1535">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="24b38-1536">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="24b38-1536">Az.EventGrid</span></span>
* <span data-ttu-id="24b38-1537">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="24b38-1537">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="24b38-1538">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="24b38-1538">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="24b38-1539">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="24b38-1539">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="24b38-1540">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="24b38-1540">Event Time-To-Live,</span></span>
        - <span data-ttu-id="24b38-1541">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="24b38-1541">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="24b38-1542">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="24b38-1542">Dead letter endpoint.</span></span>
    - <span data-ttu-id="24b38-1543">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="24b38-1543">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="24b38-1544">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="24b38-1544">Event Time-To-Live,</span></span>
        - <span data-ttu-id="24b38-1545">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="24b38-1545">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="24b38-1546">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="24b38-1546">Dead letter endpoint.</span></span>
* <span data-ttu-id="24b38-1547">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="24b38-1547">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="24b38-1548">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="24b38-1548">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="24b38-1549">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="24b38-1549">Az.IotHub</span></span>
* <span data-ttu-id="24b38-1550">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="24b38-1550">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="24b38-1551">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="24b38-1551">Az.LogicApp</span></span>
* <span data-ttu-id="24b38-1552">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="24b38-1552">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-1553">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-1553">Az.Resources</span></span>
* <span data-ttu-id="24b38-1554">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="24b38-1554">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="24b38-1555">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="24b38-1555">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="24b38-1556">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="24b38-1556">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="24b38-1557">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="24b38-1557">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="24b38-1558">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="24b38-1558">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="24b38-1559">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="24b38-1559">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="24b38-1560">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="24b38-1560">Az.SignalR</span></span>
* <span data-ttu-id="24b38-1561">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-1561">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-1562">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-1562">Az.Sql</span></span>
* <span data-ttu-id="24b38-1563">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="24b38-1563">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="24b38-1564">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-1564">Az.Storage</span></span>
* <span data-ttu-id="24b38-1565">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="24b38-1565">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="24b38-1566">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="24b38-1566">New-AzStorageContext</span></span>
* <span data-ttu-id="24b38-1567">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="24b38-1567">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="24b38-1568">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="24b38-1568">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="24b38-1569">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="24b38-1569">Az.Websites</span></span>
* <span data-ttu-id="24b38-1570">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="24b38-1570">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="24b38-1571">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-1571">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="24b38-1572">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="24b38-1572">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="24b38-1573">Geral</span><span class="sxs-lookup"><span data-stu-id="24b38-1573">General</span></span>

- <span data-ttu-id="24b38-1574">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="24b38-1574">General Availability of Az Module</span></span>
- <span data-ttu-id="24b38-1575">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="24b38-1575">Online help for each module</span></span>
- <span data-ttu-id="24b38-1576">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="24b38-1576">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="24b38-1577">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="24b38-1577">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="24b38-1578">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-1578">Az.Accounts</span></span>
- <span data-ttu-id="24b38-1579">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="24b38-1579">Changed from Az.Profile</span></span>
- <span data-ttu-id="24b38-1580">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="24b38-1580">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="24b38-1581">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="24b38-1581">Az.ApiManagement</span></span>
- <span data-ttu-id="24b38-1582">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="24b38-1582">Fixes for #7002</span></span>
- <span data-ttu-id="24b38-1583">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="24b38-1583">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="24b38-1584">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="24b38-1584">Az.Batch</span></span>
- <span data-ttu-id="24b38-1585">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="24b38-1585">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="24b38-1586">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="24b38-1586">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="24b38-1587">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="24b38-1587">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="24b38-1588">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="24b38-1588">Az.Billing</span></span>
- <span data-ttu-id="24b38-1589">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="24b38-1589">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="24b38-1590">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1590">Az.CognitivServices</span></span>
- <span data-ttu-id="24b38-1591">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="24b38-1591">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="24b38-1592">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="24b38-1592">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="24b38-1593">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="24b38-1593">Az.ContainerInstance</span></span>
- <span data-ttu-id="24b38-1594">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="24b38-1594">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="24b38-1595">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="24b38-1595">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="24b38-1596">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="24b38-1596">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="24b38-1597">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="24b38-1597">Az.DataLakeStore</span></span>
- <span data-ttu-id="24b38-1598">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="24b38-1598">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="24b38-1599">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="24b38-1599">Az.Monitor</span></span>
- <span data-ttu-id="24b38-1600">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="24b38-1600">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="24b38-1601">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="24b38-1601">Az.KeyVault</span></span>
- <span data-ttu-id="24b38-1602">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="24b38-1602">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="24b38-1603">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="24b38-1603">Az.MachineLearning</span></span>
- <span data-ttu-id="24b38-1604">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="24b38-1604">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="24b38-1605">Az.Media</span><span class="sxs-lookup"><span data-stu-id="24b38-1605">Az.Media</span></span>
- <span data-ttu-id="24b38-1606">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="24b38-1606">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="24b38-1607">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1607">Az.Network</span></span>
<span data-ttu-id="24b38-1608">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="24b38-1608">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="24b38-1609">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="24b38-1609">New cmdlets added:</span></span>
        - <span data-ttu-id="24b38-1610">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="24b38-1610">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="24b38-1611">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="24b38-1611">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="24b38-1612">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="24b38-1612">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="24b38-1613">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="24b38-1613">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="24b38-1614">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="24b38-1614">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="24b38-1615">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="24b38-1615">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="24b38-1616">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="24b38-1616">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="24b38-1617">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="24b38-1617">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="24b38-1618">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="24b38-1618">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="24b38-1619">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="24b38-1619">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="24b38-1620">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="24b38-1620">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="24b38-1621">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="24b38-1621">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="24b38-1622">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-1622">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="24b38-1623">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-1623">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="24b38-1624">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="24b38-1624">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="24b38-1625">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="24b38-1625">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="24b38-1626">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="24b38-1626">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="24b38-1627">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="24b38-1627">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="24b38-1628">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="24b38-1628">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="24b38-1629">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="24b38-1629">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="24b38-1630">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="24b38-1630">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="24b38-1631">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="24b38-1631">Az.OperationalInsights</span></span>
- <span data-ttu-id="24b38-1632">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="24b38-1632">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="24b38-1633">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="24b38-1633">Az.Profile</span></span>
- <span data-ttu-id="24b38-1634">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="24b38-1634">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="24b38-1635">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1635">Az.RecoveryServices</span></span>
- <span data-ttu-id="24b38-1636">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="24b38-1636">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="24b38-1637">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-1637">Az.Resources</span></span>
- <span data-ttu-id="24b38-1638">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="24b38-1638">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="24b38-1639">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="24b38-1639">Az.ServiceFabric</span></span>
- <span data-ttu-id="24b38-1640">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="24b38-1640">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="24b38-1641">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="24b38-1641">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="24b38-1642">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="24b38-1642">Az.SIgnalR</span></span>
- <span data-ttu-id="24b38-1643">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="24b38-1643">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="24b38-1644">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-1644">Az.Sql</span></span>
- <span data-ttu-id="24b38-1645">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="24b38-1645">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="24b38-1646">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="24b38-1646">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="24b38-1647">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="24b38-1647">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="24b38-1648">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-1648">Az.Storage</span></span>
- <span data-ttu-id="24b38-1649">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="24b38-1649">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="24b38-1650">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="24b38-1650">Az.Websites</span></span>
- <span data-ttu-id="24b38-1651">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="24b38-1651">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="24b38-1652">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="24b38-1652">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="24b38-1653">Geral</span><span class="sxs-lookup"><span data-stu-id="24b38-1653">General</span></span>

* <span data-ttu-id="24b38-1654">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="24b38-1654">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="24b38-1655">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-1655">Az.Compute</span></span>

* <span data-ttu-id="24b38-1656">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="24b38-1656">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="24b38-1657">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="24b38-1657">Az.DataLakeStore</span></span>

* <span data-ttu-id="24b38-1658">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="24b38-1658">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="24b38-1659">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="24b38-1659">Az.FrontDoor</span></span>

* <span data-ttu-id="24b38-1660">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="24b38-1660">Fixed some broken links</span></span>
    - <span data-ttu-id="24b38-1661">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="24b38-1661">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="24b38-1662">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="24b38-1662">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="24b38-1663">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1663">Az.RecoveryServices</span></span>

* <span data-ttu-id="24b38-1664">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="24b38-1664">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="24b38-1665">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="24b38-1665">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="24b38-1666">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-1666">Az.Resources</span></span>

* <span data-ttu-id="24b38-1667">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="24b38-1667">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="24b38-1668">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="24b38-1668">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="24b38-1669">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-1669">Az.Sql</span></span>

* <span data-ttu-id="24b38-1670">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="24b38-1670">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="24b38-1671">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="24b38-1671">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="24b38-1672">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="24b38-1672">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="24b38-1673">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-1673">Az.Storage</span></span>

* <span data-ttu-id="24b38-1674">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="24b38-1674">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="24b38-1675">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="24b38-1675">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="24b38-1676">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="24b38-1676">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="24b38-1677">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="24b38-1677">Support Static Website configuration</span></span>
    - <span data-ttu-id="24b38-1678">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="24b38-1678">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="24b38-1679">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="24b38-1679">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="24b38-1680">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="24b38-1680">Az.Websites</span></span>

* <span data-ttu-id="24b38-1681">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="24b38-1681">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="24b38-1682">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="24b38-1682">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="24b38-1683">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="24b38-1683">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="24b38-1684">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="24b38-1684">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="24b38-1685">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="24b38-1685">Az.ApiManagement</span></span>
* <span data-ttu-id="24b38-1686">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="24b38-1686">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="24b38-1687">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="24b38-1687">Az.Automation</span></span>
* <span data-ttu-id="24b38-1688">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="24b38-1688">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="24b38-1689">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="24b38-1689">Added Update Management cmdlets</span></span>
* <span data-ttu-id="24b38-1690">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="24b38-1690">Added Source Control cmdlets</span></span>
* <span data-ttu-id="24b38-1691">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="24b38-1691">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="24b38-1692">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="24b38-1692">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="24b38-1693">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-1693">Az.Compute</span></span>
* <span data-ttu-id="24b38-1694">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="24b38-1694">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="24b38-1695">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="24b38-1695">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="24b38-1696">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="24b38-1696">Az.ContainerInstance</span></span>
* <span data-ttu-id="24b38-1697">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="24b38-1697">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="24b38-1698">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="24b38-1698">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="24b38-1699">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="24b38-1699">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="24b38-1700">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1700">Az.Network</span></span>
* <span data-ttu-id="24b38-1701">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="24b38-1701">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="24b38-1702">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="24b38-1702">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="24b38-1703">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="24b38-1703">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="24b38-1704">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="24b38-1704">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="24b38-1705">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="24b38-1705">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="24b38-1706">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="24b38-1706">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="24b38-1707">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="24b38-1707">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="24b38-1708">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="24b38-1708">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="24b38-1709">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="24b38-1709">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="24b38-1710">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="24b38-1710">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="24b38-1711">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="24b38-1711">Az.Relay</span></span>
* <span data-ttu-id="24b38-1712">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="24b38-1712">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="24b38-1713">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-1713">Az.Resources</span></span>
* <span data-ttu-id="24b38-1714">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="24b38-1714">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="24b38-1715">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="24b38-1715">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="24b38-1716">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="24b38-1716">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="24b38-1717">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="24b38-1717">Az.ServiceFabric</span></span>
* <span data-ttu-id="24b38-1718">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="24b38-1718">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="24b38-1719">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-1719">Az.Sql</span></span>
* <span data-ttu-id="24b38-1720">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="24b38-1720">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="24b38-1721">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="24b38-1721">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="24b38-1722">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="24b38-1722">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="24b38-1723">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="24b38-1723">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="24b38-1724">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="24b38-1724">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="24b38-1725">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="24b38-1725">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="24b38-1726">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="24b38-1726">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="24b38-1727">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="24b38-1727">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="24b38-1728">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="24b38-1728">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="24b38-1729">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="24b38-1729">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="24b38-1730">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="24b38-1730">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="24b38-1731">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="24b38-1731">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="24b38-1732">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="24b38-1732">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="24b38-1733">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="24b38-1733">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="24b38-1734">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="24b38-1734">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="24b38-1735">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="24b38-1735">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="24b38-1736">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="24b38-1736">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="24b38-1737">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="24b38-1737">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="24b38-1738">Geral</span><span class="sxs-lookup"><span data-stu-id="24b38-1738">General</span></span>
* <span data-ttu-id="24b38-1739">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="24b38-1739">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="24b38-1740">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="24b38-1740">Az.Profile</span></span>
* <span data-ttu-id="24b38-1741">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="24b38-1741">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="24b38-1742">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="24b38-1742">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="24b38-1743">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="24b38-1743">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="24b38-1744">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="24b38-1744">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="24b38-1745">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="24b38-1745">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="24b38-1746">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="24b38-1746">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="24b38-1747">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="24b38-1747">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="24b38-1748">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1748">Az.CognitiveServices</span></span>
* <span data-ttu-id="24b38-1749">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="24b38-1749">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-1750">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-1750">Az.Compute</span></span>
* <span data-ttu-id="24b38-1751">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="24b38-1751">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="24b38-1752">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="24b38-1752">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="24b38-1753">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="24b38-1753">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="24b38-1754">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="24b38-1754">Az.DataLakeStore</span></span>
* <span data-ttu-id="24b38-1755">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="24b38-1755">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="24b38-1756">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="24b38-1756">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="24b38-1757">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="24b38-1757">Az.Insights</span></span>
* <span data-ttu-id="24b38-1758">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="24b38-1758">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="24b38-1759">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="24b38-1759">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="24b38-1760">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="24b38-1760">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="24b38-1761">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="24b38-1761">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-1762">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1762">Az.Network</span></span>
* <span data-ttu-id="24b38-1763">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="24b38-1763">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="24b38-1764">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="24b38-1764">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="24b38-1765">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="24b38-1765">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="24b38-1766">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="24b38-1766">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="24b38-1767">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="24b38-1767">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="24b38-1768">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="24b38-1768">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="24b38-1769">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="24b38-1769">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="24b38-1770">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="24b38-1770">Az.PolicyInsights</span></span>
* <span data-ttu-id="24b38-1771">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="24b38-1771">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-1772">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-1772">Az.Resources</span></span>
* <span data-ttu-id="24b38-1773">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="24b38-1773">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="24b38-1774">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="24b38-1774">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="24b38-1775">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="24b38-1775">Az.ServiceBus</span></span>
* <span data-ttu-id="24b38-1776">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="24b38-1776">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="24b38-1777">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="24b38-1777">Az.ServiceFabric</span></span>
* <span data-ttu-id="24b38-1778">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="24b38-1778">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="24b38-1779">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="24b38-1779">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="24b38-1780">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="24b38-1780">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="24b38-1781">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="24b38-1781">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="24b38-1782">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="24b38-1782">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="24b38-1783">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="24b38-1783">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="24b38-1784">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="24b38-1784">Az.Profile</span></span>
* <span data-ttu-id="24b38-1785">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="24b38-1785">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="24b38-1786">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="24b38-1786">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-1787">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-1787">Az.Compute</span></span>
* <span data-ttu-id="24b38-1788">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="24b38-1788">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="24b38-1789">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="24b38-1789">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="24b38-1790">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="24b38-1790">Az.DataLakeStore</span></span>
* <span data-ttu-id="24b38-1791">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="24b38-1791">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="24b38-1792">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="24b38-1792">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="24b38-1793">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="24b38-1793">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="24b38-1794">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="24b38-1794">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="24b38-1795">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="24b38-1795">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-1796">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1796">Az.Network</span></span>
* <span data-ttu-id="24b38-1797">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="24b38-1797">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="24b38-1798">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="24b38-1798">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-1799">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-1799">Az.Resources</span></span>
* <span data-ttu-id="24b38-1800">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="24b38-1800">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="24b38-1801">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="24b38-1801">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="24b38-1802">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="24b38-1802">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="24b38-1803">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="24b38-1803">Azure.Storage</span></span>
* <span data-ttu-id="24b38-1804">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="24b38-1804">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="24b38-1805">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="24b38-1805">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="24b38-1806">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="24b38-1806">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="24b38-1807">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="24b38-1807">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="24b38-1808">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="24b38-1808">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="24b38-1809">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="24b38-1809">Az.CognitiveServices</span></span>
* <span data-ttu-id="24b38-1810">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="24b38-1810">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="24b38-1811">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="24b38-1811">Az.Compute</span></span>
* <span data-ttu-id="24b38-1812">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="24b38-1812">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="24b38-1813">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="24b38-1813">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="24b38-1814">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="24b38-1814">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="24b38-1815">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="24b38-1815">Az.DataFactoryV2</span></span>
* <span data-ttu-id="24b38-1816">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="24b38-1816">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="24b38-1817">Az.Network</span><span class="sxs-lookup"><span data-stu-id="24b38-1817">Az.Network</span></span>
* <span data-ttu-id="24b38-1818">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="24b38-1818">Added NetworkProfile functionality.</span></span> <span data-ttu-id="24b38-1819">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="24b38-1819">new cmdlets added</span></span>
    - <span data-ttu-id="24b38-1820">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="24b38-1820">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="24b38-1821">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="24b38-1821">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="24b38-1822">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="24b38-1822">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="24b38-1823">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="24b38-1823">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="24b38-1824">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-1824">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="24b38-1825">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-1825">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="24b38-1826">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="24b38-1826">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="24b38-1827">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="24b38-1827">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="24b38-1828">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="24b38-1828">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="24b38-1829">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="24b38-1829">Az.RedisCache</span></span>
* <span data-ttu-id="24b38-1830">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="24b38-1830">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="24b38-1831">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="24b38-1831">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="24b38-1832">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="24b38-1832">Az.Resources</span></span>
* <span data-ttu-id="24b38-1833">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="24b38-1833">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="24b38-1834">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="24b38-1834">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="24b38-1835">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="24b38-1835">Az.Sql</span></span>
* <span data-ttu-id="24b38-1836">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="24b38-1836">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="24b38-1837">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="24b38-1837">Az.Websites</span></span>
* <span data-ttu-id="24b38-1838">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="24b38-1838">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="24b38-1839">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="24b38-1839">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="24b38-1840">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="24b38-1840">0.2.0 - September 2018</span></span>
 <span data-ttu-id="24b38-1841">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="24b38-1841">Initial Release</span></span>
