---
ms.openlocfilehash: 2db9810e20254373a487013de50d4297d4ec50d5
ms.sourcegitcommit: 8f59e11e5c991543964154d63648aa1e6ae22512
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/26/2019
ms.locfileid: "58475395"
---
## <a name="160---march-2019"></a><span data-ttu-id="9bcba-101">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="9bcba-101">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="9bcba-102">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="9bcba-102">Highlights since the last major release</span></span>
* <span data-ttu-id="9bcba-103">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="9bcba-103">General availability of `Az` module</span></span>
* <span data-ttu-id="9bcba-104">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="9bcba-104">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="9bcba-105">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="9bcba-105">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="9bcba-106">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="9bcba-106">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="9bcba-107">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="9bcba-107">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="9bcba-108">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="9bcba-108">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="9bcba-109">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="9bcba-109">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="9bcba-110">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="9bcba-110">Az.Automation</span></span>
* <span data-ttu-id="9bcba-111">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="9bcba-111">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="9bcba-112">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="9bcba-112">Dynamic grouping</span></span>
    * <span data-ttu-id="9bcba-113">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="9bcba-113">Pre-Post script</span></span>
    * <span data-ttu-id="9bcba-114">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="9bcba-114">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="9bcba-115">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="9bcba-115">Az.Compute</span></span>
* <span data-ttu-id="9bcba-116">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="9bcba-116">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="9bcba-117">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="9bcba-117">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="9bcba-118">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9bcba-118">Az.KeyVault</span></span>
* <span data-ttu-id="9bcba-119">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="9bcba-119">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="9bcba-120">Az.Network</span><span class="sxs-lookup"><span data-stu-id="9bcba-120">Az.Network</span></span>
* <span data-ttu-id="9bcba-121">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="9bcba-121">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="9bcba-122">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="9bcba-122">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="9bcba-123">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="9bcba-123">Az.RecoveryServices</span></span>
* <span data-ttu-id="9bcba-124">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="9bcba-124">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="9bcba-125">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="9bcba-125">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="9bcba-126">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="9bcba-126">Az.Resources</span></span>
* <span data-ttu-id="9bcba-127">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="9bcba-127">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="9bcba-128">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="9bcba-128">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="9bcba-129">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="9bcba-129">Az.Sql</span></span>
* <span data-ttu-id="9bcba-130">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="9bcba-130">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="9bcba-131">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="9bcba-131">Az.Storage</span></span>
* <span data-ttu-id="9bcba-132">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="9bcba-132">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="9bcba-133">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="9bcba-133">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="9bcba-134">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="9bcba-134">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="9bcba-135">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="9bcba-135">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="9bcba-136">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="9bcba-136">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="9bcba-137">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="9bcba-137">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="9bcba-138">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="9bcba-138">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="9bcba-139">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="9bcba-139">Az.Websites</span></span>
* <span data-ttu-id="9bcba-140">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="9bcba-140">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="9bcba-141">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="9bcba-141">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="9bcba-142">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="9bcba-142">Az.Accounts</span></span>
* <span data-ttu-id="9bcba-143">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="9bcba-143">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="9bcba-144">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="9bcba-144">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="9bcba-145">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="9bcba-145">Az.Automation</span></span>
* <span data-ttu-id="9bcba-146">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="9bcba-146">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="9bcba-147">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="9bcba-147">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="9bcba-148">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="9bcba-148">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="9bcba-149">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="9bcba-149">Az.Cdn</span></span>
* <span data-ttu-id="9bcba-150">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="9bcba-150">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="9bcba-151">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="9bcba-151">Az.Compute</span></span>
* <span data-ttu-id="9bcba-152">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="9bcba-152">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="9bcba-153">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="9bcba-153">Az.DataFactory</span></span>
* <span data-ttu-id="9bcba-154">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="9bcba-154">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="9bcba-155">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="9bcba-155">Az.LogicApp</span></span>
* <span data-ttu-id="9bcba-156">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="9bcba-156">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="9bcba-157">Az.Network</span><span class="sxs-lookup"><span data-stu-id="9bcba-157">Az.Network</span></span>
* <span data-ttu-id="9bcba-158">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="9bcba-158">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="9bcba-159">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="9bcba-159">Az.RecoveryServices</span></span>
* <span data-ttu-id="9bcba-160">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="9bcba-160">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="9bcba-161">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="9bcba-161">SDK Update</span></span>
* <span data-ttu-id="9bcba-162">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="9bcba-162">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="9bcba-163">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="9bcba-163">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="9bcba-164">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="9bcba-164">Az.Resources</span></span>
* <span data-ttu-id="9bcba-165">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="9bcba-165">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="9bcba-166">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="9bcba-166">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="9bcba-167">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="9bcba-167">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="9bcba-168">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="9bcba-168">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="9bcba-169">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="9bcba-169">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="9bcba-170">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="9bcba-170">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="9bcba-171">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="9bcba-171">Az.Sql</span></span>
* <span data-ttu-id="9bcba-172">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="9bcba-172">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="9bcba-173">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="9bcba-173">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="9bcba-174">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="9bcba-174">Az.Storage</span></span>
* <span data-ttu-id="9bcba-175">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="9bcba-175">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="9bcba-176">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="9bcba-176">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="9bcba-177">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9bcba-177">Az.AnalysisServices</span></span>
* <span data-ttu-id="9bcba-178">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="9bcba-178">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="9bcba-179">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="9bcba-179">Az.Automation</span></span>
* <span data-ttu-id="9bcba-180">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="9bcba-180">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="9bcba-181">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="9bcba-181">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="9bcba-182">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="9bcba-182">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="9bcba-183">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="9bcba-183">Az.CognitiveServices</span></span>
* <span data-ttu-id="9bcba-184">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="9bcba-184">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="9bcba-185">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="9bcba-185">Az.Compute</span></span>
* <span data-ttu-id="9bcba-186">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="9bcba-186">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="9bcba-187">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="9bcba-187">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="9bcba-188">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="9bcba-188">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="9bcba-189">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="9bcba-189">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="9bcba-190">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9bcba-190">Az.DataLakeStore</span></span>
* <span data-ttu-id="9bcba-191">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="9bcba-191">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="9bcba-192">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="9bcba-192">Az.EventHub</span></span>
* <span data-ttu-id="9bcba-193">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="9bcba-193">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="9bcba-194">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9bcba-194">Az.KeyVault</span></span>
* <span data-ttu-id="9bcba-195">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="9bcba-195">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="9bcba-196">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="9bcba-196">Az.LogicApp</span></span>
* <span data-ttu-id="9bcba-197">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="9bcba-197">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="9bcba-198">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="9bcba-198">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="9bcba-199">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="9bcba-199">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="9bcba-200">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="9bcba-200">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="9bcba-201">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="9bcba-201">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="9bcba-202">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="9bcba-202">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="9bcba-203">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="9bcba-203">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="9bcba-204">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="9bcba-204">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="9bcba-205">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="9bcba-205">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="9bcba-206">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="9bcba-206">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="9bcba-207">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="9bcba-207">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="9bcba-208">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="9bcba-208">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="9bcba-209">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="9bcba-209">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="9bcba-210">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="9bcba-210">Az.Monitor</span></span>
* <span data-ttu-id="9bcba-211">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="9bcba-211">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="9bcba-212">Az.Network</span><span class="sxs-lookup"><span data-stu-id="9bcba-212">Az.Network</span></span>
* <span data-ttu-id="9bcba-213">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="9bcba-213">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="9bcba-214">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="9bcba-214">Az.OperationalInsights</span></span>
* <span data-ttu-id="9bcba-215">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="9bcba-215">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="9bcba-216">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="9bcba-216">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="9bcba-217">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="9bcba-217">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="9bcba-218">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="9bcba-218">Az.Resources</span></span>
* <span data-ttu-id="9bcba-219">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="9bcba-219">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="9bcba-220">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="9bcba-220">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="9bcba-221">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="9bcba-221">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="9bcba-222">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="9bcba-222">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="9bcba-223">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="9bcba-223">Az.Sql</span></span>
* <span data-ttu-id="9bcba-224">Suporte adicionado para a camada Hiperescala da BD SQL</span><span class="sxs-lookup"><span data-stu-id="9bcba-224">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="9bcba-225">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="9bcba-225">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="9bcba-226">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="9bcba-226">Az.Websites</span></span>
* <span data-ttu-id="9bcba-227">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="9bcba-227">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="9bcba-228">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="9bcba-228">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="9bcba-229">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="9bcba-229">Az.Accounts</span></span>
* <span data-ttu-id="9bcba-230">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="9bcba-230">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="9bcba-231">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9bcba-231">Az.AnalysisServices</span></span>
<span data-ttu-id="9bcba-232">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="9bcba-232">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="9bcba-233">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="9bcba-233">Az.Compute</span></span>
* <span data-ttu-id="9bcba-234">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="9bcba-234">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="9bcba-235">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="9bcba-235">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="9bcba-236">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="9bcba-236">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="9bcba-237">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="9bcba-237">Az.RecoveryServices</span></span>
<span data-ttu-id="9bcba-238">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="9bcba-238">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="9bcba-239">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="9bcba-239">Az.Resources</span></span>
* <span data-ttu-id="9bcba-240">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="9bcba-240">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="9bcba-241">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="9bcba-241">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="9bcba-242">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="9bcba-242">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="9bcba-243">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="9bcba-243">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="9bcba-244">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="9bcba-244">Az.Sql</span></span>
* <span data-ttu-id="9bcba-245">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="9bcba-245">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="9bcba-246">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="9bcba-246">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="9bcba-247">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="9bcba-247">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="9bcba-248">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="9bcba-248">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="9bcba-249">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="9bcba-249">Az.Accounts</span></span>
* <span data-ttu-id="9bcba-250">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="9bcba-250">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="9bcba-251">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9bcba-251">Az.AnalysisServices</span></span>
* <span data-ttu-id="9bcba-252">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="9bcba-252">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="9bcba-253">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="9bcba-253">Az.RecoveryServices</span></span>
* <span data-ttu-id="9bcba-254">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="9bcba-254">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="9bcba-255">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="9bcba-255">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="9bcba-256">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="9bcba-256">Az.Accounts</span></span>
* <span data-ttu-id="9bcba-257">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="9bcba-257">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="9bcba-258">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="9bcba-258">Update incorrect online help URLs</span></span>
* <span data-ttu-id="9bcba-259">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="9bcba-259">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="9bcba-260">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="9bcba-260">Az.Aks</span></span>
* <span data-ttu-id="9bcba-261">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="9bcba-261">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="9bcba-262">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="9bcba-262">Az.Automation</span></span>
* <span data-ttu-id="9bcba-263">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="9bcba-263">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="9bcba-264">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="9bcba-264">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="9bcba-265">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="9bcba-265">Az.Cdn</span></span>
* <span data-ttu-id="9bcba-266">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="9bcba-266">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="9bcba-267">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="9bcba-267">Az.Compute</span></span>
* <span data-ttu-id="9bcba-268">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="9bcba-268">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="9bcba-269">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="9bcba-269">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="9bcba-270">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="9bcba-270">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="9bcba-271">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="9bcba-271">Az.ContainerRegistry</span></span>
* <span data-ttu-id="9bcba-272">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="9bcba-272">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="9bcba-273">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="9bcba-273">Az.DataFactory</span></span>
* <span data-ttu-id="9bcba-274">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="9bcba-274">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="9bcba-275">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9bcba-275">Az.DataLakeStore</span></span>
* <span data-ttu-id="9bcba-276">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="9bcba-276">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="9bcba-277">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="9bcba-277">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="9bcba-278">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="9bcba-278">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="9bcba-279">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="9bcba-279">Az.IotHub</span></span>
* <span data-ttu-id="9bcba-280">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="9bcba-280">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="9bcba-281">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9bcba-281">Az.KeyVault</span></span>
* <span data-ttu-id="9bcba-282">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="9bcba-282">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="9bcba-283">Az.Network</span><span class="sxs-lookup"><span data-stu-id="9bcba-283">Az.Network</span></span>
* <span data-ttu-id="9bcba-284">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="9bcba-284">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="9bcba-285">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="9bcba-285">Az.Resources</span></span>
* <span data-ttu-id="9bcba-286">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="9bcba-286">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="9bcba-287">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="9bcba-287">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="9bcba-288">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="9bcba-288">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="9bcba-289">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="9bcba-289">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="9bcba-290">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="9bcba-290">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="9bcba-291">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="9bcba-291">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="9bcba-292">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="9bcba-292">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="9bcba-293">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9bcba-293">Az.ServiceFabric</span></span>
* <span data-ttu-id="9bcba-294">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="9bcba-294">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="9bcba-295">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="9bcba-295">Fix some error messages.</span></span>
* <span data-ttu-id="9bcba-296">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="9bcba-296">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="9bcba-297">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="9bcba-297">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="9bcba-298">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="9bcba-298">Az.SignalR</span></span>
* <span data-ttu-id="9bcba-299">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="9bcba-299">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="9bcba-300">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="9bcba-300">Az.Sql</span></span>
* <span data-ttu-id="9bcba-301">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="9bcba-301">Update incorrect online help URLs</span></span>
* <span data-ttu-id="9bcba-302">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="9bcba-302">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="9bcba-303">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="9bcba-303">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="9bcba-304">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="9bcba-304">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="9bcba-305">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="9bcba-305">Az.Storage</span></span>
* <span data-ttu-id="9bcba-306">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="9bcba-306">Update incorrect online help URLs</span></span>
* <span data-ttu-id="9bcba-307">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="9bcba-307">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="9bcba-308">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="9bcba-308">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="9bcba-309">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="9bcba-309">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="9bcba-310">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9bcba-310">Az.TrafficManager</span></span>
* <span data-ttu-id="9bcba-311">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="9bcba-311">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="9bcba-312">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="9bcba-312">Az.Websites</span></span>
* <span data-ttu-id="9bcba-313">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="9bcba-313">Update incorrect online help URLs</span></span>
* <span data-ttu-id="9bcba-314">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="9bcba-314">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="9bcba-315">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="9bcba-315">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="9bcba-316">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="9bcba-316">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="9bcba-317">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="9bcba-317">Az.Accounts</span></span>
* <span data-ttu-id="9bcba-318">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="9bcba-318">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="9bcba-319">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="9bcba-319">Az.Compute</span></span>
* <span data-ttu-id="9bcba-320">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="9bcba-320">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="9bcba-321">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="9bcba-321">Updated the description of ID in help files</span></span>
* <span data-ttu-id="9bcba-322">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="9bcba-322">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="9bcba-323">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9bcba-323">Az.DataLakeStore</span></span>
* <span data-ttu-id="9bcba-324">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="9bcba-324">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="9bcba-325">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="9bcba-325">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="9bcba-326">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="9bcba-326">Az.EventGrid</span></span>
* <span data-ttu-id="9bcba-327">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="9bcba-327">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="9bcba-328">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="9bcba-328">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="9bcba-329">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="9bcba-329">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="9bcba-330">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="9bcba-330">Event Time-To-Live,</span></span>
        - <span data-ttu-id="9bcba-331">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="9bcba-331">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="9bcba-332">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="9bcba-332">Dead letter endpoint.</span></span>
    - <span data-ttu-id="9bcba-333">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="9bcba-333">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="9bcba-334">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="9bcba-334">Event Time-To-Live,</span></span>
        - <span data-ttu-id="9bcba-335">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="9bcba-335">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="9bcba-336">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="9bcba-336">Dead letter endpoint.</span></span>
* <span data-ttu-id="9bcba-337">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="9bcba-337">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="9bcba-338">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="9bcba-338">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="9bcba-339">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="9bcba-339">Az.IotHub</span></span>
* <span data-ttu-id="9bcba-340">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="9bcba-340">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="9bcba-341">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="9bcba-341">Az.LogicApp</span></span>
* <span data-ttu-id="9bcba-342">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="9bcba-342">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="9bcba-343">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="9bcba-343">Az.Resources</span></span>
* <span data-ttu-id="9bcba-344">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="9bcba-344">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="9bcba-345">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="9bcba-345">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="9bcba-346">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9bcba-346">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="9bcba-347">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="9bcba-347">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="9bcba-348">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="9bcba-348">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="9bcba-349">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="9bcba-349">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="9bcba-350">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="9bcba-350">Az.SignalR</span></span>
* <span data-ttu-id="9bcba-351">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="9bcba-351">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="9bcba-352">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="9bcba-352">Az.Sql</span></span>
* <span data-ttu-id="9bcba-353">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="9bcba-353">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="9bcba-354">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="9bcba-354">Az.Storage</span></span>
* <span data-ttu-id="9bcba-355">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="9bcba-355">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="9bcba-356">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="9bcba-356">New-AzStorageContext</span></span>
* <span data-ttu-id="9bcba-357">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="9bcba-357">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="9bcba-358">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="9bcba-358">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="9bcba-359">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="9bcba-359">Az.Websites</span></span>
* <span data-ttu-id="9bcba-360">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="9bcba-360">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="9bcba-361">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="9bcba-361">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="9bcba-362">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="9bcba-362">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="9bcba-363">Geral</span><span class="sxs-lookup"><span data-stu-id="9bcba-363">General</span></span>

- <span data-ttu-id="9bcba-364">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="9bcba-364">General Availability of Az Module</span></span>
- <span data-ttu-id="9bcba-365">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="9bcba-365">Online help for each module</span></span>
- <span data-ttu-id="9bcba-366">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="9bcba-366">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="9bcba-367">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="9bcba-367">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="9bcba-368">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="9bcba-368">Az.Accounts</span></span>
- <span data-ttu-id="9bcba-369">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="9bcba-369">Changed from Az.Profile</span></span>
- <span data-ttu-id="9bcba-370">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="9bcba-370">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="9bcba-371">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="9bcba-371">Az.ApiManagement</span></span>
- <span data-ttu-id="9bcba-372">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="9bcba-372">Fixes for #7002</span></span>
- <span data-ttu-id="9bcba-373">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="9bcba-373">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="9bcba-374">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="9bcba-374">Az.Batch</span></span>
- <span data-ttu-id="9bcba-375">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="9bcba-375">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="9bcba-376">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="9bcba-376">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="9bcba-377">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="9bcba-377">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="9bcba-378">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="9bcba-378">Az.Billing</span></span>
- <span data-ttu-id="9bcba-379">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="9bcba-379">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="9bcba-380">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="9bcba-380">Az.CognitivServices</span></span>
- <span data-ttu-id="9bcba-381">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="9bcba-381">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="9bcba-382">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="9bcba-382">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="9bcba-383">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="9bcba-383">Az.ContainerInstance</span></span>
- <span data-ttu-id="9bcba-384">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="9bcba-384">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="9bcba-385">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="9bcba-385">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="9bcba-386">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="9bcba-386">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="9bcba-387">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9bcba-387">Az.DataLakeStore</span></span>
- <span data-ttu-id="9bcba-388">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="9bcba-388">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="9bcba-389">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="9bcba-389">Az.Monitor</span></span>
- <span data-ttu-id="9bcba-390">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="9bcba-390">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="9bcba-391">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9bcba-391">Az.KeyVault</span></span>
- <span data-ttu-id="9bcba-392">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="9bcba-392">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="9bcba-393">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="9bcba-393">Az.MachineLearning</span></span>
- <span data-ttu-id="9bcba-394">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="9bcba-394">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="9bcba-395">Az.Media</span><span class="sxs-lookup"><span data-stu-id="9bcba-395">Az.Media</span></span>
- <span data-ttu-id="9bcba-396">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="9bcba-396">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="9bcba-397">Az.Network</span><span class="sxs-lookup"><span data-stu-id="9bcba-397">Az.Network</span></span>
<span data-ttu-id="9bcba-398">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="9bcba-398">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="9bcba-399">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="9bcba-399">New cmdlets added:</span></span>
        - <span data-ttu-id="9bcba-400">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="9bcba-400">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="9bcba-401">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="9bcba-401">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="9bcba-402">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="9bcba-402">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="9bcba-403">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="9bcba-403">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="9bcba-404">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="9bcba-404">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="9bcba-405">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="9bcba-405">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="9bcba-406">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="9bcba-406">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="9bcba-407">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="9bcba-407">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="9bcba-408">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="9bcba-408">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="9bcba-409">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="9bcba-409">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="9bcba-410">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="9bcba-410">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="9bcba-411">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="9bcba-411">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="9bcba-412">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="9bcba-412">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="9bcba-413">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="9bcba-413">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="9bcba-414">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="9bcba-414">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="9bcba-415">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="9bcba-415">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="9bcba-416">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="9bcba-416">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="9bcba-417">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="9bcba-417">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="9bcba-418">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="9bcba-418">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="9bcba-419">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="9bcba-419">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="9bcba-420">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="9bcba-420">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="9bcba-421">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="9bcba-421">Az.OperationalInsights</span></span>
- <span data-ttu-id="9bcba-422">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="9bcba-422">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="9bcba-423">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="9bcba-423">Az.Profile</span></span>
- <span data-ttu-id="9bcba-424">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="9bcba-424">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="9bcba-425">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="9bcba-425">Az.RecoveryServices</span></span>
- <span data-ttu-id="9bcba-426">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="9bcba-426">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="9bcba-427">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="9bcba-427">Az.Resources</span></span>
- <span data-ttu-id="9bcba-428">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="9bcba-428">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="9bcba-429">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9bcba-429">Az.ServiceFabric</span></span>
- <span data-ttu-id="9bcba-430">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="9bcba-430">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="9bcba-431">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="9bcba-431">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="9bcba-432">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="9bcba-432">Az.SIgnalR</span></span>
- <span data-ttu-id="9bcba-433">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="9bcba-433">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="9bcba-434">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="9bcba-434">Az.Sql</span></span>
- <span data-ttu-id="9bcba-435">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="9bcba-435">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="9bcba-436">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="9bcba-436">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="9bcba-437">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="9bcba-437">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="9bcba-438">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="9bcba-438">Az.Storage</span></span>
- <span data-ttu-id="9bcba-439">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="9bcba-439">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="9bcba-440">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="9bcba-440">Az.Websites</span></span>
- <span data-ttu-id="9bcba-441">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="9bcba-441">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="9bcba-442">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="9bcba-442">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="9bcba-443">Geral</span><span class="sxs-lookup"><span data-stu-id="9bcba-443">General</span></span>

* <span data-ttu-id="9bcba-444">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="9bcba-444">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="9bcba-445">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="9bcba-445">Az.Compute</span></span>

* <span data-ttu-id="9bcba-446">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="9bcba-446">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="9bcba-447">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9bcba-447">Az.DataLakeStore</span></span>

* <span data-ttu-id="9bcba-448">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="9bcba-448">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="9bcba-449">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="9bcba-449">Az.FrontDoor</span></span>

* <span data-ttu-id="9bcba-450">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="9bcba-450">Fixed some broken links</span></span>
    - <span data-ttu-id="9bcba-451">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="9bcba-451">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="9bcba-452">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="9bcba-452">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="9bcba-453">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="9bcba-453">Az.RecoveryServices</span></span>

* <span data-ttu-id="9bcba-454">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="9bcba-454">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="9bcba-455">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="9bcba-455">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="9bcba-456">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="9bcba-456">Az.Resources</span></span>

* <span data-ttu-id="9bcba-457">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="9bcba-457">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="9bcba-458">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="9bcba-458">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="9bcba-459">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="9bcba-459">Az.Sql</span></span>

* <span data-ttu-id="9bcba-460">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="9bcba-460">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="9bcba-461">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="9bcba-461">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="9bcba-462">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="9bcba-462">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="9bcba-463">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="9bcba-463">Az.Storage</span></span>

* <span data-ttu-id="9bcba-464">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="9bcba-464">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="9bcba-465">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="9bcba-465">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="9bcba-466">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="9bcba-466">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="9bcba-467">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="9bcba-467">Support Static Website configuration</span></span>
    - <span data-ttu-id="9bcba-468">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="9bcba-468">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="9bcba-469">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="9bcba-469">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="9bcba-470">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="9bcba-470">Az.Websites</span></span>

* <span data-ttu-id="9bcba-471">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="9bcba-471">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="9bcba-472">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="9bcba-472">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="9bcba-473">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="9bcba-473">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="9bcba-474">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="9bcba-474">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="9bcba-475">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="9bcba-475">Az.ApiManagement</span></span>
* <span data-ttu-id="9bcba-476">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="9bcba-476">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="9bcba-477">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="9bcba-477">Az.Automation</span></span>
* <span data-ttu-id="9bcba-478">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="9bcba-478">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="9bcba-479">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="9bcba-479">Added Update Management cmdlets</span></span>
* <span data-ttu-id="9bcba-480">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="9bcba-480">Added Source Control cmdlets</span></span>
* <span data-ttu-id="9bcba-481">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="9bcba-481">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="9bcba-482">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="9bcba-482">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="9bcba-483">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="9bcba-483">Az.Compute</span></span>
* <span data-ttu-id="9bcba-484">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="9bcba-484">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="9bcba-485">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="9bcba-485">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="9bcba-486">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="9bcba-486">Az.ContainerInstance</span></span>
* <span data-ttu-id="9bcba-487">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="9bcba-487">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="9bcba-488">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="9bcba-488">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="9bcba-489">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="9bcba-489">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="9bcba-490">Az.Network</span><span class="sxs-lookup"><span data-stu-id="9bcba-490">Az.Network</span></span>
* <span data-ttu-id="9bcba-491">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="9bcba-491">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="9bcba-492">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="9bcba-492">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="9bcba-493">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="9bcba-493">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="9bcba-494">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="9bcba-494">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="9bcba-495">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="9bcba-495">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="9bcba-496">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="9bcba-496">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="9bcba-497">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="9bcba-497">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="9bcba-498">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="9bcba-498">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="9bcba-499">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="9bcba-499">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="9bcba-500">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="9bcba-500">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="9bcba-501">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="9bcba-501">Az.Relay</span></span>
* <span data-ttu-id="9bcba-502">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="9bcba-502">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="9bcba-503">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="9bcba-503">Az.Resources</span></span>
* <span data-ttu-id="9bcba-504">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="9bcba-504">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="9bcba-505">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="9bcba-505">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="9bcba-506">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="9bcba-506">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="9bcba-507">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9bcba-507">Az.ServiceFabric</span></span>
* <span data-ttu-id="9bcba-508">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="9bcba-508">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="9bcba-509">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="9bcba-509">Az.Sql</span></span>
* <span data-ttu-id="9bcba-510">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="9bcba-510">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="9bcba-511">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="9bcba-511">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="9bcba-512">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="9bcba-512">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="9bcba-513">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="9bcba-513">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="9bcba-514">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="9bcba-514">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="9bcba-515">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="9bcba-515">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="9bcba-516">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="9bcba-516">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="9bcba-517">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="9bcba-517">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="9bcba-518">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="9bcba-518">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="9bcba-519">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="9bcba-519">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="9bcba-520">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="9bcba-520">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="9bcba-521">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="9bcba-521">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="9bcba-522">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="9bcba-522">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="9bcba-523">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="9bcba-523">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="9bcba-524">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="9bcba-524">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="9bcba-525">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="9bcba-525">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="9bcba-526">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="9bcba-526">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="9bcba-527">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="9bcba-527">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="9bcba-528">Geral</span><span class="sxs-lookup"><span data-stu-id="9bcba-528">General</span></span>
* <span data-ttu-id="9bcba-529">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="9bcba-529">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="9bcba-530">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="9bcba-530">Az.Profile</span></span>
* <span data-ttu-id="9bcba-531">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="9bcba-531">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="9bcba-532">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="9bcba-532">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="9bcba-533">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="9bcba-533">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="9bcba-534">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="9bcba-534">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="9bcba-535">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="9bcba-535">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="9bcba-536">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="9bcba-536">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="9bcba-537">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="9bcba-537">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="9bcba-538">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="9bcba-538">Az.CognitiveServices</span></span>
* <span data-ttu-id="9bcba-539">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="9bcba-539">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="9bcba-540">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="9bcba-540">Az.Compute</span></span>
* <span data-ttu-id="9bcba-541">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="9bcba-541">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="9bcba-542">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="9bcba-542">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="9bcba-543">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="9bcba-543">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="9bcba-544">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9bcba-544">Az.DataLakeStore</span></span>
* <span data-ttu-id="9bcba-545">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="9bcba-545">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="9bcba-546">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="9bcba-546">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="9bcba-547">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="9bcba-547">Az.Insights</span></span>
* <span data-ttu-id="9bcba-548">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="9bcba-548">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="9bcba-549">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="9bcba-549">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="9bcba-550">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="9bcba-550">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="9bcba-551">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="9bcba-551">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="9bcba-552">Az.Network</span><span class="sxs-lookup"><span data-stu-id="9bcba-552">Az.Network</span></span>
* <span data-ttu-id="9bcba-553">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="9bcba-553">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="9bcba-554">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="9bcba-554">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="9bcba-555">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="9bcba-555">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="9bcba-556">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="9bcba-556">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="9bcba-557">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="9bcba-557">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="9bcba-558">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="9bcba-558">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="9bcba-559">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="9bcba-559">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="9bcba-560">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="9bcba-560">Az.PolicyInsights</span></span>
* <span data-ttu-id="9bcba-561">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="9bcba-561">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="9bcba-562">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="9bcba-562">Az.Resources</span></span>
* <span data-ttu-id="9bcba-563">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="9bcba-563">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="9bcba-564">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="9bcba-564">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="9bcba-565">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9bcba-565">Az.ServiceBus</span></span>
* <span data-ttu-id="9bcba-566">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="9bcba-566">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="9bcba-567">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9bcba-567">Az.ServiceFabric</span></span>
* <span data-ttu-id="9bcba-568">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="9bcba-568">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="9bcba-569">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="9bcba-569">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="9bcba-570">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="9bcba-570">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="9bcba-571">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="9bcba-571">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="9bcba-572">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="9bcba-572">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="9bcba-573">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="9bcba-573">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="9bcba-574">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="9bcba-574">Az.Profile</span></span>
* <span data-ttu-id="9bcba-575">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="9bcba-575">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="9bcba-576">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="9bcba-576">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="9bcba-577">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="9bcba-577">Az.Compute</span></span>
* <span data-ttu-id="9bcba-578">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="9bcba-578">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="9bcba-579">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="9bcba-579">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="9bcba-580">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9bcba-580">Az.DataLakeStore</span></span>
* <span data-ttu-id="9bcba-581">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="9bcba-581">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="9bcba-582">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="9bcba-582">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="9bcba-583">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="9bcba-583">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="9bcba-584">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="9bcba-584">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="9bcba-585">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="9bcba-585">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="9bcba-586">Az.Network</span><span class="sxs-lookup"><span data-stu-id="9bcba-586">Az.Network</span></span>
* <span data-ttu-id="9bcba-587">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="9bcba-587">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="9bcba-588">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="9bcba-588">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="9bcba-589">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="9bcba-589">Az.Resources</span></span>
* <span data-ttu-id="9bcba-590">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="9bcba-590">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="9bcba-591">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="9bcba-591">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="9bcba-592">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="9bcba-592">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="9bcba-593">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9bcba-593">Azure.Storage</span></span>
* <span data-ttu-id="9bcba-594">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="9bcba-594">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="9bcba-595">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="9bcba-595">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="9bcba-596">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="9bcba-596">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="9bcba-597">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="9bcba-597">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="9bcba-598">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="9bcba-598">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="9bcba-599">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="9bcba-599">Az.CognitiveServices</span></span>
* <span data-ttu-id="9bcba-600">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="9bcba-600">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="9bcba-601">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="9bcba-601">Az.Compute</span></span>
* <span data-ttu-id="9bcba-602">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="9bcba-602">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="9bcba-603">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="9bcba-603">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="9bcba-604">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="9bcba-604">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="9bcba-605">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="9bcba-605">Az.DataFactoryV2</span></span>
* <span data-ttu-id="9bcba-606">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="9bcba-606">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="9bcba-607">Az.Network</span><span class="sxs-lookup"><span data-stu-id="9bcba-607">Az.Network</span></span>
* <span data-ttu-id="9bcba-608">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="9bcba-608">Added NetworkProfile functionality.</span></span> <span data-ttu-id="9bcba-609">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="9bcba-609">new cmdlets added</span></span>
    - <span data-ttu-id="9bcba-610">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9bcba-610">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="9bcba-611">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9bcba-611">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="9bcba-612">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9bcba-612">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="9bcba-613">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9bcba-613">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="9bcba-614">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="9bcba-614">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="9bcba-615">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="9bcba-615">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="9bcba-616">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="9bcba-616">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="9bcba-617">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="9bcba-617">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="9bcba-618">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="9bcba-618">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="9bcba-619">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="9bcba-619">Az.RedisCache</span></span>
* <span data-ttu-id="9bcba-620">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="9bcba-620">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="9bcba-621">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="9bcba-621">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="9bcba-622">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="9bcba-622">Az.Resources</span></span>
* <span data-ttu-id="9bcba-623">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9bcba-623">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="9bcba-624">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="9bcba-624">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="9bcba-625">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="9bcba-625">Az.Sql</span></span>
* <span data-ttu-id="9bcba-626">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="9bcba-626">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="9bcba-627">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="9bcba-627">Az.Websites</span></span>
* <span data-ttu-id="9bcba-628">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="9bcba-628">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="9bcba-629">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="9bcba-629">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="9bcba-630">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="9bcba-630">0.2.0 - September 2018</span></span>
 <span data-ttu-id="9bcba-631">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="9bcba-631">Initial Release</span></span>