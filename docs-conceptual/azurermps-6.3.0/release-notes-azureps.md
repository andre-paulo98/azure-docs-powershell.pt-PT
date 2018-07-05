---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: 3811e28dda69d194d23934943fb47d562f869fc4
ms.sourcegitcommit: 5a5b6dd216d5f805204244146cf6f88ad2f34fb4
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/19/2018
ms.locfileid: "36237818"
---
# <a name="release-notes"></a><span data-ttu-id="300cd-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="300cd-103">Release notes</span></span>

<span data-ttu-id="300cd-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="300cd-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="630---june-2018"></a><span data-ttu-id="300cd-105">6.3.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="300cd-105">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="300cd-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="300cd-106">AzureRM.Profile</span></span>
* <span data-ttu-id="300cd-107">Mensagens de erro atualizado para Enable-AzureRmContextAutoSave</span><span class="sxs-lookup"><span data-stu-id="300cd-107">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="300cd-108">Criar um contexto para cada subscrição ao executar "Connect-AzureRmAccount" sem contexto anterior</span><span class="sxs-lookup"><span data-stu-id="300cd-108">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="300cd-109">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="300cd-109">Azure.Storage</span></span>
* <span data-ttu-id="300cd-110">Outras informações adicionadas sobre o parâmetro -Permissions nos ficheiros de ajuda.</span><span class="sxs-lookup"><span data-stu-id="300cd-110">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="300cd-111">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="300cd-111">AzureRM.Compute</span></span>
* <span data-ttu-id="300cd-112">O "Get-AzureRmVmDiskEncryptionStatus" corrige um problema observado para VMs sem discos de dados</span><span class="sxs-lookup"><span data-stu-id="300cd-112">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="300cd-113">Atualizar versão da biblioteca de cliente de Computação para corrigir os seguintes cmdlets</span><span class="sxs-lookup"><span data-stu-id="300cd-113">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="300cd-114">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="300cd-114">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="300cd-115">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="300cd-115">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="300cd-116">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="300cd-116">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="300cd-117">Os seguintes cmdlets foram corrigidos para mostrar o "ID da operação" e o "estado da operação" corretamente:</span><span class="sxs-lookup"><span data-stu-id="300cd-117">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="300cd-118">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="300cd-118">Start-AzureRmVM</span></span>
    - <span data-ttu-id="300cd-119">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="300cd-119">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="300cd-120">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="300cd-120">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="300cd-121">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="300cd-121">Set-AzureRmVM</span></span>
    - <span data-ttu-id="300cd-122">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="300cd-122">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="300cd-123">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="300cd-123">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="300cd-124">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="300cd-124">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="300cd-125">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="300cd-125">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="300cd-126">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="300cd-126">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="300cd-127">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="300cd-127">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="300cd-128">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="300cd-128">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="300cd-129">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="300cd-129">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="300cd-130">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="300cd-130">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="300cd-131">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="300cd-131">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="300cd-132">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="300cd-132">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="300cd-133">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="300cd-133">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="300cd-134">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="300cd-134">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="300cd-135">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="300cd-135">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="300cd-136">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="300cd-136">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="300cd-137">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="300cd-137">AzureRM.EventGrid</span></span>
* <span data-ttu-id="300cd-138">Remova as condições de validação ValidateNotNullOrEmpty para SubjectBeginsWith/SubjectEndsWith no cmdlet Update-AzureRmEventGridSubscription para permitir a alteração destes parâmetros para cadeia vazia, se for preciso.</span><span class="sxs-lookup"><span data-stu-id="300cd-138">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="300cd-139">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="300cd-139">AzureRM.KeyVault</span></span>
* <span data-ttu-id="300cd-140">Corrigir problema quando não forem devolvidas Etiquetas quando o Get-AzureRmKeyVault-Tag for executado</span><span class="sxs-lookup"><span data-stu-id="300cd-140">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="300cd-141">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="300cd-141">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="300cd-142">Lançamento público de cmdlets de informações de Política</span><span class="sxs-lookup"><span data-stu-id="300cd-142">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="300cd-143">Utilizar versão da API 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="300cd-143">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="300cd-144">Adicione PolicyDefinitionReferenceId aos resultados do Get-AzureRmPolicyStateSummary</span><span class="sxs-lookup"><span data-stu-id="300cd-144">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="300cd-145">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="300cd-145">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="300cd-146">Parâmetro -Vault adicionado aos cmdlets RecoveryServices.Backup.</span><span class="sxs-lookup"><span data-stu-id="300cd-146">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="300cd-147">Quando for passado, isto irá substituir o cmdlet Set-AzureRmRecoveryServicesContext.</span><span class="sxs-lookup"><span data-stu-id="300cd-147">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="300cd-148">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="300cd-148">AzureRM.Sql</span></span>
* <span data-ttu-id="300cd-149">Exemplo atualizado no ficheiro de ajuda de Get-AzureRmSqlDatabaseExpanded</span><span class="sxs-lookup"><span data-stu-id="300cd-149">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="300cd-150">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="300cd-150">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="300cd-151">Ficheiro de ajuda atualizado para Add-AzureRmTrafficManagerEndpointConfig</span><span class="sxs-lookup"><span data-stu-id="300cd-151">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="300cd-152">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="300cd-152">AzureRM.Websites</span></span>
* <span data-ttu-id="300cd-153">"Set-AzureRmWebApp" está atualizado para não substituir o AppSettings ao utilizar o -AssignIdentity</span><span class="sxs-lookup"><span data-stu-id="300cd-153">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="300cd-154">"New-AzureRmWebAppSlot" está atualizado para honrar o AppServicePlan como um parâmetro opcional</span><span class="sxs-lookup"><span data-stu-id="300cd-154">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="300cd-155">6.2.1 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="300cd-155">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="300cd-156">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="300cd-156">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="300cd-157">Modelo do PSWorkspace atualizado para permitir que a Rede utilize o tipo como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="300cd-157">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="300cd-158">6.2.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="300cd-158">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="300cd-159">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="300cd-159">AzureRM.Profile</span></span>
* <span data-ttu-id="300cd-160">Corrija o problema onde a versão 10.0.3 de Newtonsoft.Json não foi carregada na importação do módulo</span><span class="sxs-lookup"><span data-stu-id="300cd-160">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="300cd-161">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="300cd-161">AzureRM.Compute</span></span>
* <span data-ttu-id="300cd-162">Funcionalidade Atualização da VM VMSS</span><span class="sxs-lookup"><span data-stu-id="300cd-162">VMSS VM Update feature</span></span>
    - <span data-ttu-id="300cd-163">Cmdlets "Update-AzureRmVmssVM" e "New-AzureRmVMDataDisk" adicionados</span><span class="sxs-lookup"><span data-stu-id="300cd-163">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="300cd-164">Adicione o parâmetro VirtualMachineScaleSetVM ao cmdlet "Add-AzureRmVMDataDisk" para suportar a adição de um disco de dados à VM Vmss.</span><span class="sxs-lookup"><span data-stu-id="300cd-164">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="300cd-165">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="300cd-165">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="300cd-166">O SDK de .Net do ADF foi atualizado para a versão 0.8.0-preview que contém as seguintes alterações:</span><span class="sxs-lookup"><span data-stu-id="300cd-166">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="300cd-167">Foi adicionada a operação de Configuração de fábrica do repositório</span><span class="sxs-lookup"><span data-stu-id="300cd-167">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="300cd-168">QuickBooks LinkedService atualizado para expor as propriedades consumerKey e consumerSecret</span><span class="sxs-lookup"><span data-stu-id="300cd-168">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="300cd-169">Vários tipos de modelos Atualizados de SecretBase para Object</span><span class="sxs-lookup"><span data-stu-id="300cd-169">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="300cd-170">Acionador de Eventos de Blob adicionado</span><span class="sxs-lookup"><span data-stu-id="300cd-170">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="300cd-171">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="300cd-171">AzureRM.KeyVault</span></span>
* <span data-ttu-id="300cd-172">Documentação de atualização com resultado de exemplo</span><span class="sxs-lookup"><span data-stu-id="300cd-172">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="300cd-173">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="300cd-173">AzureRM.Network</span></span>
* <span data-ttu-id="300cd-174">Ativar parâmetros da Análise de Tráfego em cmdlets do Observador de Rede</span><span class="sxs-lookup"><span data-stu-id="300cd-174">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="300cd-175">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="300cd-175">AzureRM.Resources</span></span>
* <span data-ttu-id="300cd-176">Corrija o problema com a propriedade "Propriedades" do(s) objeto(s) "PSResource" devolvidos por "Get-AzureRmResource"</span><span class="sxs-lookup"><span data-stu-id="300cd-176">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="300cd-177">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="300cd-177">AzureRM.Scheduler</span></span>
* <span data-ttu-id="300cd-178">Corrija o problema com a atualização ServiceBusQueueJob sem definir novos valores de Autenticação</span><span class="sxs-lookup"><span data-stu-id="300cd-178">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="300cd-179">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="300cd-179">AzureRM.Sql</span></span>
* <span data-ttu-id="300cd-180">Cmdlets seguintes atualizados com parâmetro opcional LicenseType</span><span class="sxs-lookup"><span data-stu-id="300cd-180">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="300cd-181">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="300cd-181">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="300cd-182">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="300cd-182">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="300cd-183">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="300cd-183">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="300cd-184">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="300cd-184">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="300cd-185">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="300cd-185">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="300cd-186">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="300cd-186">AzureRM.Websites</span></span>
* <span data-ttu-id="300cd-187">"New-AzureRMWebApp" está atualizado para utilizar algoritmos comuns da biblioteca Estratégia.</span><span class="sxs-lookup"><span data-stu-id="300cd-187">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="300cd-188">6.1.0 - Maio de 2018</span><span class="sxs-lookup"><span data-stu-id="300cd-188">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="300cd-189">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="300cd-189">AzureRM.Profile</span></span>
* <span data-ttu-id="300cd-190">Correção do problema em que a execução de "Clear-AzureRmContext" mantinha um contexto vazio com o nome do contexto predefinido anterior, o que impedia o utilizador de criar um novo contexto com o nome antigo</span><span class="sxs-lookup"><span data-stu-id="300cd-190">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="300cd-191">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="300cd-191">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="300cd-192">Permitir operações de associação/desassociação do Gateway no AS.</span><span class="sxs-lookup"><span data-stu-id="300cd-192">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="300cd-193">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="300cd-193">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="300cd-194">Foi adicionado suporte para ApiVersions, ApiReleases e ApiRevisions</span><span class="sxs-lookup"><span data-stu-id="300cd-194">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="300cd-195">Foi adicionado suporte para o Back-end do ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="300cd-195">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="300cd-196">Foi adicionado suporte para o Logger do Application Insights</span><span class="sxs-lookup"><span data-stu-id="300cd-196">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="300cd-197">Foi adicionado suporte para reconhecer o SKU "Básico" como um SKU válido do serviço Gestão de API</span><span class="sxs-lookup"><span data-stu-id="300cd-197">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="300cd-198">Foi adicionado suporte para instalar Certificados emitidos por AC privadas como Raiz ou AC</span><span class="sxs-lookup"><span data-stu-id="300cd-198">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="300cd-199">Foi adicionado suporte para aceitar Certificados SSL personalizados através do KeyVault e de vários nomes de anfitrião de proxy</span><span class="sxs-lookup"><span data-stu-id="300cd-199">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="300cd-200">Foi adicionado suporte para a identidade MSI</span><span class="sxs-lookup"><span data-stu-id="300cd-200">Added support for MSI identity</span></span>
* <span data-ttu-id="300cd-201">Foi adicionado suporte para aceitar políticas através de Url. NOTA: Os cmdlets seguintes serão preteridos numa versão futura</span><span class="sxs-lookup"><span data-stu-id="300cd-201">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="300cd-202">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="300cd-202">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="300cd-203">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="300cd-203">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="300cd-204">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="300cd-204">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="300cd-205">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="300cd-205">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="300cd-206">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="300cd-206">AzureRM.Batch</span></span>
* <span data-ttu-id="300cd-207">Lançamento do novo cmdlet Get-AzureBatchPoolNodeCounts</span><span class="sxs-lookup"><span data-stu-id="300cd-207">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="300cd-208">Lançamento do novo cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span><span class="sxs-lookup"><span data-stu-id="300cd-208">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="300cd-209">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="300cd-209">AzureRM.Consumption</span></span>
* <span data-ttu-id="300cd-210">Adição dos novos parâmetros Expand, ResourceGroup, InstanceName, InstanceId, Tags e Top no Cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="300cd-210">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="300cd-211">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="300cd-211">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="300cd-212">Correção do exemplo de Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="300cd-212">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="300cd-213">Correção da exceção do parâmetro nulo do caso Recursivo em Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="300cd-213">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="300cd-214">Correção dos ficheiros de ajuda de Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="300cd-214">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="300cd-215">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="300cd-215">AzureRM.Network</span></span>
* <span data-ttu-id="300cd-216">Aumento da versão do SDK de Rede de 18.0.0-preview para 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="300cd-216">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="300cd-217">Foi adicionado um cmdlet para criar a configuração de protocolo</span><span class="sxs-lookup"><span data-stu-id="300cd-217">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="300cd-218">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="300cd-218">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="300cd-219">Foi adicionado um cmdlet para adicionar uma nova ligação de circuito a um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="300cd-219">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="300cd-220">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="300cd-220">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="300cd-221">Foi adicionado um cmdlet para remover uma ligação de circuito de um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="300cd-221">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="300cd-222">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="300cd-222">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="300cd-223">Foi adicionado um cmdlet para obter uma ligação de circuito</span><span class="sxs-lookup"><span data-stu-id="300cd-223">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="300cd-224">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="300cd-224">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="300cd-225">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="300cd-225">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="300cd-226">Correção da utilização da autenticação de servidor com certificados gerados (Problema #5998)</span><span class="sxs-lookup"><span data-stu-id="300cd-226">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="300cd-227">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="300cd-227">AzureRM.Sql</span></span>
* <span data-ttu-id="300cd-228">Atualização dos cmdlets de Auditoria para permitir a remoção de AuditActions ou AuditActionGroups</span><span class="sxs-lookup"><span data-stu-id="300cd-228">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="300cd-229">Correção do problema de Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy ao definir uma nova política de retenção flexível em que o comando falhava com "Configurar a política de retenção de longo-prazo com o cofre e a política do serviço de recuperação do Azure já não é suportado.</span><span class="sxs-lookup"><span data-stu-id="300cd-229">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="300cd-230">Submeta um pedido com a nova política de retenção flexível".</span><span class="sxs-lookup"><span data-stu-id="300cd-230">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="300cd-231">Atualize todos os cmdlets relacionados com as Bases de Dados SQL do Azure/Criação de Conjuntos Elásticos/Atualização para utilizar a nova API de Base de Dados, que suporta a propriedade SKU para propriedades relacionadas com dimensionamento e escalão.</span><span class="sxs-lookup"><span data-stu-id="300cd-231">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="300cd-232">Os cmdlets atualizados, incluindo:</span><span class="sxs-lookup"><span data-stu-id="300cd-232">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="300cd-233">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="300cd-233">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="300cd-234">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="300cd-234">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="300cd-235">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="300cd-235">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="300cd-236">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="300cd-236">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="300cd-237">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="300cd-237">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="300cd-238">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="300cd-238">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="300cd-239">Atualize os parâmetros de "Get-AzureRmTrafficManagerProfile" para que o parâmetro -ResourceGroupName seja necessário ao utilizar o parâmetro -Name.</span><span class="sxs-lookup"><span data-stu-id="300cd-239">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>