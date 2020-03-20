---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: f24e5ef66f9c49976c550c9847903bd0608c5123
ms.sourcegitcommit: f6fa6543be1e0f6330b1598f01528b2928cc426c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2020
ms.locfileid: "79111042"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="754b4-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="754b4-103">Azure PowerShell release notes</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="754b4-104">3.6.1 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="754b4-104">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="754b4-105">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-105">Az.Accounts</span></span>
* <span data-ttu-id="754b4-106">Abrir a página de inquérito do Azure PowerShell em "Send-Feedback" [#11020]</span><span class="sxs-lookup"><span data-stu-id="754b4-106">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="754b4-107">Apresentar o URL de inquérito do Azure PowerShell em "Resolve-Error" [#11021]</span><span class="sxs-lookup"><span data-stu-id="754b4-107">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="754b4-108">Adicionada versão de Az em UserAgent</span><span class="sxs-lookup"><span data-stu-id="754b4-108">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="754b4-109">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="754b4-109">Az.ApiManagement</span></span>
* <span data-ttu-id="754b4-110">Adicionado suporte para a obtenção e configuração do Domínio Personalizado no Ponto Final do DeveloperPortal [#11007]</span><span class="sxs-lookup"><span data-stu-id="754b4-110">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="754b4-111">"Export-AzApiManagementApi" Adicionado suporte para a transferência da definição da API no formato JSON [#9987]</span><span class="sxs-lookup"><span data-stu-id="754b4-111">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="754b4-112">"Import-AzApiManagementApi" Adicionado suporte para a importação da definição de OpenApi 3.0 a partir de documento JSON</span><span class="sxs-lookup"><span data-stu-id="754b4-112">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="754b4-113">"New-AzApiManagementIdentityProvider" e "Set-AzApiManagementIdentityProvider" Adicionado suporte para a configuração de "Inquilino de Início de Sessão" para Fornecedor de AAD B2C [#9784]</span><span class="sxs-lookup"><span data-stu-id="754b4-113">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="754b4-114">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="754b4-114">Az.DataLakeStore</span></span>
* <span data-ttu-id="754b4-115">Adicionada referência a System.Buffers explicitamente em csproj e psd1.</span><span class="sxs-lookup"><span data-stu-id="754b4-115">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="754b4-116">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="754b4-116">Az.IotHub</span></span>
* <span data-ttu-id="754b4-117">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="754b4-117">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="754b4-118">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="754b4-118">New Cmdlets are:</span></span>
    - <span data-ttu-id="754b4-119">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="754b4-119">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="754b4-120">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="754b4-120">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="754b4-121">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="754b4-121">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="754b4-122">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="754b4-122">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="754b4-123">Adicionado suporte para a gestão de módulos num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="754b4-123">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="754b4-124">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="754b4-124">New Cmdlets are:</span></span>
    - <span data-ttu-id="754b4-125">"Add-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="754b4-125">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="754b4-126">"Get-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="754b4-126">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="754b4-127">"Remove-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="754b4-127">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="754b4-128">"Set-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="754b4-128">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="754b4-129">Adicionado cmdlet para obter a cadeia de ligação de um dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="754b4-129">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="754b4-130">Adicionado cmdlet para obter a cadeia de ligação de um módulo num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="754b4-130">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="754b4-131">Adicionado suporte para obter/definir dispositivo principal de um dispositivo IoT.</span><span class="sxs-lookup"><span data-stu-id="754b4-131">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="754b4-132">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="754b4-132">New Cmdlets are:</span></span>
    - <span data-ttu-id="754b4-133">"Get-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="754b4-133">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="754b4-134">"Set-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="754b4-134">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="754b4-135">Adicionado suporte para gerir relações principal-subordinado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="754b4-135">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="754b4-136">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="754b4-136">Az.Monitor</span></span>
* <span data-ttu-id="754b4-137">Corrigido o valor de saída de "Get-AzMetricDefinition" [#9714]</span><span class="sxs-lookup"><span data-stu-id="754b4-137">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-138">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-138">Az.Network</span></span>
* <span data-ttu-id="754b4-139">Sdk Sql Management atualizado.</span><span class="sxs-lookup"><span data-stu-id="754b4-139">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="754b4-140">Corrigido um problema de diferença de nomes na classe PrivateLinkServiceConnectionState.</span><span class="sxs-lookup"><span data-stu-id="754b4-140">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="754b4-141">Mapeamento do campo ActionsRequired para ActionRequired.</span><span class="sxs-lookup"><span data-stu-id="754b4-141">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="754b4-142">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="754b4-142">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-143">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-143">Az.Resources</span></span>
* <span data-ttu-id="754b4-144">Correção para erro de referência nula em "Get-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="754b4-144">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="754b4-145">Comutadores "-Force" e "-PassThru" marcados como opcionais em "Remove-AzADGroup" [#10849]</span><span class="sxs-lookup"><span data-stu-id="754b4-145">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="754b4-146">Corrigido problema em que "MailNickname" não devolve "Remove-AzADGroup" [#11167]</span><span class="sxs-lookup"><span data-stu-id="754b4-146">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="754b4-147">Corrigido problema em que a operação de pipe "Remove-AzADGroup" não funciona [#11171]</span><span class="sxs-lookup"><span data-stu-id="754b4-147">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="754b4-148">Correção para erro de referência nula em GetAzureRoleAssignmentCommand</span><span class="sxs-lookup"><span data-stu-id="754b4-148">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="754b4-149">Adicionados atributos de alterações interruptivas para futuras alterações a cmdlets de política</span><span class="sxs-lookup"><span data-stu-id="754b4-149">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="754b4-150">"Get-AzResourceGroup" atualizado para realizar filtragem de etiqueta de grupo de recursos no lado do servidor</span><span class="sxs-lookup"><span data-stu-id="754b4-150">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="754b4-151">Cmdlets Tag alargados para accept -ResourceId</span><span class="sxs-lookup"><span data-stu-id="754b4-151">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="754b4-152">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="754b4-152">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="754b4-153">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="754b4-153">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="754b4-154">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="754b4-154">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="754b4-155">Adicionado cmdlet Tag novo</span><span class="sxs-lookup"><span data-stu-id="754b4-155">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="754b4-156">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="754b4-156">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="754b4-157">ScopedDeployment trazido de SDK 3.3.0</span><span class="sxs-lookup"><span data-stu-id="754b4-157">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-158">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-158">Az.Sql</span></span>
* <span data-ttu-id="754b4-159">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="754b4-159">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="754b4-160">Adicionado suporte para configuração de cópia de segurança de Retenção de Longo Prazo para Bases de Dados Geridas</span><span class="sxs-lookup"><span data-stu-id="754b4-160">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="754b4-161">Política Get/Set numa base de dados gerida</span><span class="sxs-lookup"><span data-stu-id="754b4-161">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="754b4-162">Obter cópia(s) de segurança LTR por base de dados gerida, por instância gerida ou por localização</span><span class="sxs-lookup"><span data-stu-id="754b4-162">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="754b4-163">Remover uma cópia de segurança LTR</span><span class="sxs-lookup"><span data-stu-id="754b4-163">Remove an LTR backup</span></span>
    - <span data-ttu-id="754b4-164">Restaurar uma cópia de segurança LTR para criar uma base de dados gerida nova</span><span class="sxs-lookup"><span data-stu-id="754b4-164">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="754b4-165">Adicionado MinimalTlsVersion a New-AzSqlServer e Set-AzSqlServer</span><span class="sxs-lookup"><span data-stu-id="754b4-165">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="754b4-166">Adicionado MinimalTlsVersion a New-AzSqlInstance e Set-AzSqlInstance</span><span class="sxs-lookup"><span data-stu-id="754b4-166">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="754b4-167">Versão de SDK SQL atualizada para Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-167">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-168">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-168">Az.Storage</span></span>
* <span data-ttu-id="754b4-169">AllowProtectedAppendWrite suportada em ImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="754b4-169">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="754b4-170">"Set-AzRmStorageContainerImmutabilityPolicy"</span><span class="sxs-lookup"><span data-stu-id="754b4-170">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="754b4-171">Adicionada uma mensagem de aviso de alteração interruptiva para alteração do tipo AzureStorageTable numa futura versão</span><span class="sxs-lookup"><span data-stu-id="754b4-171">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="754b4-172">"New-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="754b4-172">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="754b4-173">"Get-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="754b4-173">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="754b4-174">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-174">Az.Websites</span></span>
* <span data-ttu-id="754b4-175">Adicionado o parâmetro Tag para "New-AzAppServicePlan" e "Set-AzAppServicePlan"</span><span class="sxs-lookup"><span data-stu-id="754b4-175">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="754b4-176">Paragem da execução de cmdlet caso seja emitida uma exceção ao adicionar um domínio personalizado a um site</span><span class="sxs-lookup"><span data-stu-id="754b4-176">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="754b4-177">Adicionado suporte para a realização de operações para Serviços de Aplicações em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="754b4-177">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="754b4-178">Aplicada restrição de acesso a WebApp/Função em diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="754b4-178">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="754b4-179">Corrigido problema para definir os nomes de anfitrião personalizados para WebAppSlots</span><span class="sxs-lookup"><span data-stu-id="754b4-179">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="754b4-180">3.5.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="754b4-180">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="754b4-181">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="754b4-181">Highlights since the last major release</span></span>
* <span data-ttu-id="754b4-182">Telemetria do lado do cliente atualizada.</span><span class="sxs-lookup"><span data-stu-id="754b4-182">Updated client side telemetry.</span></span>
* <span data-ttu-id="754b4-183">O Az.IotHub adicionou cmdlets para suportar a gestão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="754b4-183">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="754b4-184">O Az.SqlVirtualMachine adicionou cmdlets ao Serviço de Escuta do Grupo de Disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="754b4-184">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="754b4-185">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-185">Az.Accounts</span></span>
* <span data-ttu-id="754b4-186">SubscriptionId, TenantId e tempo de execução adicionados aos dados de telemetria do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="754b4-186">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="754b4-187">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="754b4-187">Az.Automation</span></span>
* <span data-ttu-id="754b4-188">Foi corrigido o erro no Exemplo 1 na documentação de referência de "New-AzAutomationSoftwareUpdateConfiguration"</span><span class="sxs-lookup"><span data-stu-id="754b4-188">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="754b4-189">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="754b4-189">Az.CognitiveServices</span></span>
* <span data-ttu-id="754b4-190">SDK atualizado para a versão 7.0</span><span class="sxs-lookup"><span data-stu-id="754b4-190">Updated SDK to 7.0</span></span>
* <span data-ttu-id="754b4-191">Mensagem de erro melhorada quando o servidor responde ao corpo vazio</span><span class="sxs-lookup"><span data-stu-id="754b4-191">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-192">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-192">Az.Compute</span></span>
* <span data-ttu-id="754b4-193">Valor vazio permitido para ProximityPlacementGroupId durante a atualização</span><span class="sxs-lookup"><span data-stu-id="754b4-193">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="754b4-194">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="754b4-194">Az.FrontDoor</span></span>
* <span data-ttu-id="754b4-195">Cmdlet adicionado para obter definições de regras geridas que podem ser utilizadas na WAF</span><span class="sxs-lookup"><span data-stu-id="754b4-195">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="754b4-196">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="754b4-196">Az.IotHub</span></span>
* <span data-ttu-id="754b4-197">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="754b4-197">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="754b4-198">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="754b4-198">New Cmdlets are:</span></span>
    - <span data-ttu-id="754b4-199">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="754b4-199">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="754b4-200">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="754b4-200">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="754b4-201">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="754b4-201">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="754b4-202">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="754b4-202">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="754b4-203">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="754b4-203">Az.KeyVault</span></span>
* <span data-ttu-id="754b4-204">Texto duplicado fixo para Add-AzKeyVaultKey.md</span><span class="sxs-lookup"><span data-stu-id="754b4-204">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="754b4-205">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="754b4-205">Az.Monitor</span></span>
* <span data-ttu-id="754b4-206">Descrição fixa do cmdlet Get-AzLog.</span><span class="sxs-lookup"><span data-stu-id="754b4-206">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="754b4-207">Foi adicionado um novo parâmetro chamado ActionGroupId ao comando "New-AzMetricAlertRuleV2".</span><span class="sxs-lookup"><span data-stu-id="754b4-207">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="754b4-208">O utilizador pode fornecer ActionGroupId(string) ou ActionGorup(ActivityLogAlertActionGroup).</span><span class="sxs-lookup"><span data-stu-id="754b4-208">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-209">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-209">Az.Network</span></span>
* <span data-ttu-id="754b4-210">Foi adicionada uma nota de parâmetro adicional para o parâmetro "-EnableProxyProtocol" para o cmdlet "New-AzPrivateLinkService".</span><span class="sxs-lookup"><span data-stu-id="754b4-210">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="754b4-211">Exemplo de FilterData fixo em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="754b4-211">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="754b4-212">Exemplo de Captura de Pacotes adicionado para capturar todos os pacotes internos e externos em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="754b4-212">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="754b4-213">Política do Azure Firewall suportada em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="754b4-213">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="754b4-214">Não foram adicionados novos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="754b4-214">No new cmdlets are added.</span></span> <span data-ttu-id="754b4-215">Simplificação da restrição da política de firewall em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="754b4-215">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-216">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-216">Az.RecoveryServices</span></span>
* <span data-ttu-id="754b4-217">Suporte adicionado da funcionalidade Restaurar como ficheiros para Bases de Dados SQL.</span><span class="sxs-lookup"><span data-stu-id="754b4-217">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-218">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-218">Az.Resources</span></span>
* <span data-ttu-id="754b4-219">Cmdlets de implementação de modelos refatorizados</span><span class="sxs-lookup"><span data-stu-id="754b4-219">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="754b4-220">Foram adicionados novos cmdlets para gerir implementações no grupo de gestão: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="754b4-220">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="754b4-221">Foram adicionados novos cmdlets para gerir implementações no inquilino: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="754b4-221">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="754b4-222">Cmdlets \*-AzDeployment refatorizados para trabalhar especificamente no âmbito da subscrição</span><span class="sxs-lookup"><span data-stu-id="754b4-222">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="754b4-223">Foram criados aliases \*-AzSubscriptionDeployment para os cmdlets \*-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="754b4-223">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="754b4-224">"Update-AzADApplication" fixo quando o parâmetro "AvailableToOtherTenants" não está definido</span><span class="sxs-lookup"><span data-stu-id="754b4-224">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="754b4-225">ApplicationObjectWithoutCredentialParameterSet removido para evitar AmbiguousParameterSetException.</span><span class="sxs-lookup"><span data-stu-id="754b4-225">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="754b4-226">Ficheiros de ajuda regenerados</span><span class="sxs-lookup"><span data-stu-id="754b4-226">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-227">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-227">Az.Sql</span></span>
* <span data-ttu-id="754b4-228">Suporte adicionado para restauro para um ponto anterior no tempo entre subscrições nas Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="754b4-228">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="754b4-229">Suporte adicionado para alterar a geração de hardware das Instâncias Geridas de SQL existentes</span><span class="sxs-lookup"><span data-stu-id="754b4-229">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="754b4-230">Exemplos de ajuda "Update-AzSqlServerVulnerabilityAssessmentSetting" fixos: saída do parâmetro/propriedade - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="754b4-230">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="754b4-231">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="754b4-231">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="754b4-232">Cmdlets adicionados para o Serviço de Escuta do Grupo de Disponibilidade</span><span class="sxs-lookup"><span data-stu-id="754b4-232">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="754b4-233">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="754b4-233">Az.StorageSync</span></span>
* <span data-ttu-id="754b4-234">Conjuntos de carateres suportados atualizados em "Invoke-AzStorageSyncCompatibilityCheck".</span><span class="sxs-lookup"><span data-stu-id="754b4-234">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="754b4-235">3.4.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="754b4-235">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="754b4-236">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="754b4-236">Highlights since the last major release</span></span>
* <span data-ttu-id="754b4-237">Versão inicial Az.CosmosDB 0.1.0 lançada</span><span class="sxs-lookup"><span data-stu-id="754b4-237">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="754b4-238">Foi adicionado suporte para Az.Network ConnectionMonitor V2</span><span class="sxs-lookup"><span data-stu-id="754b4-238">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="754b4-239">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-239">Az.Accounts</span></span>
* <span data-ttu-id="754b4-240">Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível</span><span class="sxs-lookup"><span data-stu-id="754b4-240">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="754b4-241">Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5</span><span class="sxs-lookup"><span data-stu-id="754b4-241">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="754b4-242">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="754b4-242">Az.ApiManagement</span></span>
* <span data-ttu-id="754b4-243">**Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="754b4-243">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="754b4-244">**New-AzApiManagementProduct**\* e **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="754b4-244">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="754b4-245">Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472</span><span class="sxs-lookup"><span data-stu-id="754b4-245">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="754b4-246">**Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet</span><span class="sxs-lookup"><span data-stu-id="754b4-246">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-247">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-247">Az.Compute</span></span>
* <span data-ttu-id="754b4-248">Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.</span><span class="sxs-lookup"><span data-stu-id="754b4-248">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="754b4-249">Foi adicionado o cmdlet Update-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="754b4-249">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="754b4-250">Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="754b4-250">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="754b4-251">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-251">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="754b4-252">Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="754b4-252">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="754b4-253">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="754b4-253">Az.DataFactory</span></span>
* <span data-ttu-id="754b4-254">Atualização do SDK .NET do ADF para a versão 4.7.0</span><span class="sxs-lookup"><span data-stu-id="754b4-254">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="754b4-255">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="754b4-255">Az.DeploymentManager</span></span>
* <span data-ttu-id="754b4-256">Adiciona operações LIST para os recursos</span><span class="sxs-lookup"><span data-stu-id="754b4-256">Adds LIST operations for resources</span></span>
* <span data-ttu-id="754b4-257">Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="754b4-257">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="754b4-258">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="754b4-258">Az.HDInsight</span></span>
* <span data-ttu-id="754b4-259">Foi corrigido o erro do documento de New-AzHDInsightCluster.</span><span class="sxs-lookup"><span data-stu-id="754b4-259">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="754b4-260">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="754b4-260">Az.KeyVault</span></span>
* <span data-ttu-id="754b4-261">Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.</span><span class="sxs-lookup"><span data-stu-id="754b4-261">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-262">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-262">Az.Network</span></span>
* <span data-ttu-id="754b4-263">Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="754b4-263">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="754b4-264">Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão</span><span class="sxs-lookup"><span data-stu-id="754b4-264">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="754b4-265">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="754b4-265">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="754b4-266">Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="754b4-266">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="754b4-267">Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"</span><span class="sxs-lookup"><span data-stu-id="754b4-267">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="754b4-268">Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.</span><span class="sxs-lookup"><span data-stu-id="754b4-268">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="754b4-269">Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="754b4-269">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="754b4-270">Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="754b4-270">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="754b4-271">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="754b4-271">New cmdlets added:</span></span>
        - <span data-ttu-id="754b4-272">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="754b4-272">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="754b4-273">Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="754b4-273">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="754b4-274">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="754b4-274">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="754b4-275">Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2</span><span class="sxs-lookup"><span data-stu-id="754b4-275">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="754b4-276">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="754b4-276">Az.PolicyInsights</span></span>
* <span data-ttu-id="754b4-277">Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar</span><span class="sxs-lookup"><span data-stu-id="754b4-277">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="754b4-278">Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation</span><span class="sxs-lookup"><span data-stu-id="754b4-278">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="754b4-279">Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política</span><span class="sxs-lookup"><span data-stu-id="754b4-279">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="754b4-280">Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="754b4-280">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-281">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-281">Az.RecoveryServices</span></span>
* <span data-ttu-id="754b4-282">Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.</span><span class="sxs-lookup"><span data-stu-id="754b4-282">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="754b4-283">O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.</span><span class="sxs-lookup"><span data-stu-id="754b4-283">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-284">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-284">Az.Resources</span></span>
* <span data-ttu-id="754b4-285">-Scope foi tornado opcional nos cmdlets \*-AzPolicyAssignment com subscrição de contexto predefinida</span><span class="sxs-lookup"><span data-stu-id="754b4-285">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="754b4-286">Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves</span><span class="sxs-lookup"><span data-stu-id="754b4-286">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-287">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-287">Az.Sql</span></span>
<span data-ttu-id="754b4-288">Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.</span><span class="sxs-lookup"><span data-stu-id="754b4-288">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-289">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-289">Az.Storage</span></span>
* <span data-ttu-id="754b4-290">Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="754b4-290">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="754b4-291">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-291">New-AzStorageAccount</span></span>
* <span data-ttu-id="754b4-292">Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation</span><span class="sxs-lookup"><span data-stu-id="754b4-292">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="754b4-293">Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="754b4-293">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="754b4-294">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-294">Az.Websites</span></span>
* <span data-ttu-id="754b4-295">Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState</span><span class="sxs-lookup"><span data-stu-id="754b4-295">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="754b4-296">Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido</span><span class="sxs-lookup"><span data-stu-id="754b4-296">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="754b4-297">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="754b4-297">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="754b4-298">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-298">Az.Accounts</span></span>
* <span data-ttu-id="754b4-299">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="754b4-299">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="754b4-300">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="754b4-300">Az.Cdn</span></span>
* <span data-ttu-id="754b4-301">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="754b4-301">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-302">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-302">Az.Compute</span></span>
* <span data-ttu-id="754b4-303">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="754b4-303">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="754b4-304">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="754b4-304">Az.ContainerInstance</span></span>
* <span data-ttu-id="754b4-305">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="754b4-305">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="754b4-306">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="754b4-306">Az.DataBoxEdge</span></span>
* <span data-ttu-id="754b4-307">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="754b4-307">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="754b4-308">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="754b4-308">Get the Edge Storage Container</span></span>
* <span data-ttu-id="754b4-309">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="754b4-309">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="754b4-310">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="754b4-310">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="754b4-311">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="754b4-311">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="754b4-312">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="754b4-312">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="754b4-313">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="754b4-313">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="754b4-314">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="754b4-314">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="754b4-315">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="754b4-315">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="754b4-316">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="754b4-316">Get the Edge Storage Account</span></span>
* <span data-ttu-id="754b4-317">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="754b4-317">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="754b4-318">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="754b4-318">Create new Edge Storage Account</span></span>
* <span data-ttu-id="754b4-319">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="754b4-319">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="754b4-320">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="754b4-320">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="754b4-321">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="754b4-321">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="754b4-322">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="754b4-322">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="754b4-323">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="754b4-323">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="754b4-324">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="754b4-324">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="754b4-325">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="754b4-325">Az.DataFactory</span></span>
* <span data-ttu-id="754b4-326">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="754b4-326">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="754b4-327">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="754b4-327">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="754b4-328">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="754b4-328">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="754b4-329">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="754b4-329">Az.DevTestLabs</span></span>
* <span data-ttu-id="754b4-330">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="754b4-330">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="754b4-331">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="754b4-331">Az.EventHub</span></span>
* <span data-ttu-id="754b4-332">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="754b4-332">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="754b4-333">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="754b4-333">Az.HDInsight</span></span>
* <span data-ttu-id="754b4-334">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="754b4-334">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="754b4-335">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="754b4-335">Az.MachineLearning</span></span>
* <span data-ttu-id="754b4-336">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="754b4-336">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="754b4-337">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="754b4-337">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="754b4-338">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="754b4-338">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="754b4-339">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="754b4-339">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="754b4-340">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="754b4-340">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="754b4-341">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="754b4-341">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="754b4-342">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="754b4-342">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="754b4-343">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="754b4-343">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-344">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-344">Az.Network</span></span>
* <span data-ttu-id="754b4-345">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="754b4-345">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-346">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-346">Az.RecoveryServices</span></span>
* <span data-ttu-id="754b4-347">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-347">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="754b4-348">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-348">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="754b4-349">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-349">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="754b4-350">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-350">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-351">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-351">Az.Resources</span></span>
* <span data-ttu-id="754b4-352">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="754b4-352">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-353">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-353">Az.Sql</span></span>
* <span data-ttu-id="754b4-354">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="754b4-354">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="754b4-355">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="754b4-355">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="754b4-356">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="754b4-356">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="754b4-357">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="754b4-357">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-358">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-358">Az.Storage</span></span>
* <span data-ttu-id="754b4-359">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="754b4-359">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="754b4-360">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="754b4-360">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="754b4-361">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="754b4-361">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="754b4-362">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-362">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="754b4-363">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-363">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="754b4-364">Geral</span><span class="sxs-lookup"><span data-stu-id="754b4-364">General</span></span>
* <span data-ttu-id="754b4-365">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="754b4-365">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="754b4-366">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-366">Az.Accounts</span></span>
* <span data-ttu-id="754b4-367">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="754b4-367">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="754b4-368">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="754b4-368">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="754b4-369">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="754b4-369">Az.Batch</span></span>
* <span data-ttu-id="754b4-370">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="754b4-370">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="754b4-371">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="754b4-371">Az.DataFactory</span></span>
* <span data-ttu-id="754b4-372">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="754b4-372">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="754b4-373">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="754b4-373">Az.FrontDoor</span></span>
* <span data-ttu-id="754b4-374">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="754b4-374">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="754b4-375">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="754b4-375">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="754b4-376">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="754b4-376">Az.HealthcareApis</span></span>
* <span data-ttu-id="754b4-377">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="754b4-377">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="754b4-378">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="754b4-378">Az.KeyVault</span></span>
* <span data-ttu-id="754b4-379">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="754b4-379">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="754b4-380">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="754b4-380">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="754b4-381">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="754b4-381">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="754b4-382">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="754b4-382">Az.Monitor</span></span>
* <span data-ttu-id="754b4-383">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="754b4-383">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="754b4-384">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="754b4-384">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="754b4-385">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="754b4-385">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-386">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-386">Az.Network</span></span>
* <span data-ttu-id="754b4-387">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="754b4-387">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-388">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-388">Az.Resources</span></span>
* <span data-ttu-id="754b4-389">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="754b4-389">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="754b4-390">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="754b4-390">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-391">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-391">Az.Sql</span></span>
* <span data-ttu-id="754b4-392">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="754b4-392">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-393">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-393">Az.Storage</span></span>
* <span data-ttu-id="754b4-394">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="754b4-394">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="754b4-395">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="754b4-395">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="754b4-396">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="754b4-396">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="754b4-397">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="754b4-397">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="754b4-398">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="754b4-398">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="754b4-399">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="754b4-399">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="754b4-400">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="754b4-400">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="754b4-401">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="754b4-401">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="754b4-402">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="754b4-402">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="754b4-403">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="754b4-403">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="754b4-404">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="754b4-404">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="754b4-405">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="754b4-405">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="754b4-406">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="754b4-406">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="754b4-407">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-407">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="754b4-408">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="754b4-408">Highlights since the last major release</span></span>
* <span data-ttu-id="754b4-409">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="754b4-409">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="754b4-410">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="754b4-410">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-411">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-411">Az.Compute</span></span>
* <span data-ttu-id="754b4-412">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="754b4-412">VM Reapply feature</span></span>
    - <span data-ttu-id="754b4-413">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="754b4-413">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="754b4-414">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="754b4-414">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="754b4-415">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="754b4-415">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="754b4-416">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="754b4-416">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="754b4-417">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="754b4-417">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="754b4-418">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="754b4-418">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="754b4-419">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="754b4-419">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="754b4-420">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="754b4-420">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="754b4-421">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="754b4-421">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="754b4-422">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="754b4-422">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="754b4-423">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="754b4-423">Az.DataBoxEdge</span></span>
* <span data-ttu-id="754b4-424">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="754b4-424">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="754b4-425">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="754b4-425">Get the Order</span></span>
* <span data-ttu-id="754b4-426">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="754b4-426">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="754b4-427">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="754b4-427">Create new Order</span></span>
* <span data-ttu-id="754b4-428">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="754b4-428">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="754b4-429">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="754b4-429">Remove the Order</span></span>
* <span data-ttu-id="754b4-430">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="754b4-430">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="754b4-431">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="754b4-431">Now creates Local Share</span></span>
* <span data-ttu-id="754b4-432">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="754b4-432">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="754b4-433">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="754b4-433">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="754b4-434">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="754b4-434">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="754b4-435">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="754b4-435">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="754b4-436">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="754b4-436">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="754b4-437">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="754b4-437">Gets the information about Triggers</span></span>
* <span data-ttu-id="754b4-438">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="754b4-438">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="754b4-439">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="754b4-439">Create new Triggers</span></span>
* <span data-ttu-id="754b4-440">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="754b4-440">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="754b4-441">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="754b4-441">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="754b4-442">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="754b4-442">Az.DataFactory</span></span>
* <span data-ttu-id="754b4-443">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="754b4-443">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="754b4-444">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="754b4-444">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="754b4-445">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="754b4-445">Az.DataLakeStore</span></span>
* <span data-ttu-id="754b4-446">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="754b4-446">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="754b4-447">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="754b4-447">Az.EventHub</span></span>
* <span data-ttu-id="754b4-448">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="754b4-448">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="754b4-449">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="754b4-449">Az.FrontDoor</span></span>
* <span data-ttu-id="754b4-450">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="754b4-450">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="754b4-451">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="754b4-451">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="754b4-452">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="754b4-452">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="754b4-453">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="754b4-453">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-454">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-454">Az.Network</span></span>
* <span data-ttu-id="754b4-455">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="754b4-455">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="754b4-456">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="754b4-456">Az.PrivateDns</span></span>
* <span data-ttu-id="754b4-457">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="754b4-457">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-458">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-458">Az.RecoveryServices</span></span>
* <span data-ttu-id="754b4-459">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="754b4-459">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="754b4-460">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="754b4-460">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="754b4-461">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="754b4-461">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="754b4-462">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="754b4-462">Az.RedisCache</span></span>
* <span data-ttu-id="754b4-463">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="754b4-463">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="754b4-464">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="754b4-464">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="754b4-465">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="754b4-465">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-466">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-466">Az.Resources</span></span>
- <span data-ttu-id="754b4-467">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="754b4-467">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="754b4-468">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="754b4-468">Updated create policy definition help example</span></span>
- <span data-ttu-id="754b4-469">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="754b4-469">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="754b4-470">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="754b4-470">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="754b4-471">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="754b4-471">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-472">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-472">Az.Sql</span></span>
* <span data-ttu-id="754b4-473">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="754b4-473">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="754b4-474">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="754b4-474">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="754b4-475">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-475">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="754b4-476">Geral</span><span class="sxs-lookup"><span data-stu-id="754b4-476">General</span></span>
* <span data-ttu-id="754b4-477">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="754b4-477">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="754b4-478">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-478">Az.Accounts</span></span>
* <span data-ttu-id="754b4-479">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="754b4-479">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="754b4-480">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="754b4-480">Az.Advisor</span></span>
* <span data-ttu-id="754b4-481">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="754b4-481">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="754b4-482">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="754b4-482">Az.Batch</span></span>
* <span data-ttu-id="754b4-483">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="754b4-483">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="754b4-484">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="754b4-484">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="754b4-485">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="754b4-485">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="754b4-486">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="754b4-486">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="754b4-487">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="754b4-487">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="754b4-488">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="754b4-488">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="754b4-489">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="754b4-489">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="754b4-490">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="754b4-490">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="754b4-491">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="754b4-491">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="754b4-492">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="754b4-492">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="754b4-493">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="754b4-493">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="754b4-494">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="754b4-494">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="754b4-495">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="754b4-495">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="754b4-496">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="754b4-496">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="754b4-497">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="754b4-497">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="754b4-498">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="754b4-498">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="754b4-499">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="754b4-499">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="754b4-500">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="754b4-500">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="754b4-501">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="754b4-501">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="754b4-502">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="754b4-502">This operation is no longer supported.</span></span>
* <span data-ttu-id="754b4-503">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="754b4-503">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="754b4-504">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="754b4-504">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="754b4-505">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="754b4-505">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="754b4-506">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="754b4-506">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="754b4-507">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="754b4-507">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="754b4-508">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="754b4-508">New non-verified images are also now returned.</span></span> <span data-ttu-id="754b4-509">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="754b4-509">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="754b4-510">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="754b4-510">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="754b4-511">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="754b4-511">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="754b4-512">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="754b4-512">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="754b4-513">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="754b4-513">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="754b4-514">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="754b4-514">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="754b4-515">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="754b4-515">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="754b4-516">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="754b4-516">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="754b4-517">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="754b4-517">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="754b4-518">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="754b4-518">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="754b4-519">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="754b4-519">Az.Cdn</span></span>
* <span data-ttu-id="754b4-520">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="754b4-520">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="754b4-521">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="754b4-521">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-522">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-522">Az.Compute</span></span>
* <span data-ttu-id="754b4-523">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="754b4-523">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="754b4-524">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="754b4-524">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="754b4-525">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="754b4-525">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="754b4-526">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-526">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="754b4-527">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-527">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="754b4-528">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="754b4-528">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="754b4-529">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="754b4-529">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="754b4-530">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="754b4-530">Breaking changes</span></span>
    - <span data-ttu-id="754b4-531">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="754b4-531">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="754b4-532">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="754b4-532">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="754b4-533">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="754b4-533">Az.DataFactory</span></span>
* <span data-ttu-id="754b4-534">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="754b4-534">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="754b4-535">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="754b4-535">Az.DataLakeStore</span></span>
* <span data-ttu-id="754b4-536">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="754b4-536">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="754b4-537">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="754b4-537">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="754b4-538">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="754b4-538">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="754b4-539">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="754b4-539">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="754b4-540">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="754b4-540">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="754b4-541">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="754b4-541">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="754b4-542">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="754b4-542">Az.FrontDoor</span></span>
* <span data-ttu-id="754b4-543">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="754b4-543">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="754b4-544">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="754b4-544">Az.HDInsight</span></span>
* <span data-ttu-id="754b4-545">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="754b4-545">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="754b4-546">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="754b4-546">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="754b4-547">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="754b4-547">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="754b4-548">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="754b4-548">Removed five cmdlets:</span></span>
    - <span data-ttu-id="754b4-549">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="754b4-549">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="754b4-550">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="754b4-550">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="754b4-551">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="754b4-551">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="754b4-552">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="754b4-552">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="754b4-553">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="754b4-553">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="754b4-554">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="754b4-554">Added three cmdlets:</span></span>
    - <span data-ttu-id="754b4-555">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="754b4-555">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="754b4-556">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="754b4-556">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="754b4-557">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="754b4-557">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="754b4-558">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="754b4-558">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="754b4-559">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="754b4-559">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="754b4-560">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="754b4-560">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="754b4-561">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="754b4-561">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="754b4-562">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="754b4-562">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="754b4-563">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="754b4-563">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="754b4-564">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="754b4-564">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="754b4-565">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="754b4-565">Added some scenario test cases.</span></span>
* <span data-ttu-id="754b4-566">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="754b4-566">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="754b4-567">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="754b4-567">Az.IotHub</span></span>
* <span data-ttu-id="754b4-568">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="754b4-568">Breaking changes:</span></span>
    - <span data-ttu-id="754b4-569">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="754b4-569">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="754b4-570">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="754b4-570">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="754b4-571">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="754b4-571">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="754b4-572">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="754b4-572">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="754b4-573">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="754b4-573">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="754b4-574">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="754b4-574">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="754b4-575">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="754b4-575">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="754b4-576">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="754b4-576">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="754b4-577">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="754b4-577">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="754b4-578">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="754b4-578">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="754b4-579">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="754b4-579">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="754b4-580">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="754b4-580">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-581">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-581">Az.RecoveryServices</span></span>
* <span data-ttu-id="754b4-582">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-582">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="754b4-583">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-583">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="754b4-584">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-584">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="754b4-585">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-585">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="754b4-586">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-586">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="754b4-587">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-587">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="754b4-588">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-588">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="754b4-589">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-589">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="754b4-590">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="754b4-590">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-591">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-591">Az.Resources</span></span>
* <span data-ttu-id="754b4-592">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="754b4-592">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-593">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-593">Az.Network</span></span>
* <span data-ttu-id="754b4-594">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="754b4-594">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="754b4-595">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="754b4-595">Updated cmdlet:</span></span>
        - <span data-ttu-id="754b4-596">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-596">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="754b4-597">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-597">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="754b4-598">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-598">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="754b4-599">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-599">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="754b4-600">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-600">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="754b4-601">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="754b4-601">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="754b4-602">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="754b4-602">New cmdlet:</span></span>
        - <span data-ttu-id="754b4-603">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="754b4-603">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="754b4-604">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="754b4-604">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="754b4-605">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="754b4-605">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="754b4-606">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-606">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="754b4-607">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="754b4-607">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="754b4-608">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="754b4-608">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="754b4-609">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="754b4-609">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="754b4-610">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="754b4-610">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="754b4-611">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="754b4-611">New cmdlets added:</span></span>
        - <span data-ttu-id="754b4-612">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="754b4-612">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="754b4-613">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="754b4-613">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="754b4-614">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="754b4-614">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="754b4-615">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="754b4-615">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="754b4-616">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="754b4-616">Set-AzVirtualHub</span></span>
* <span data-ttu-id="754b4-617">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="754b4-617">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="754b4-618">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="754b4-618">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="754b4-619">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="754b4-619">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="754b4-620">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="754b4-620">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="754b4-621">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="754b4-621">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="754b4-622">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="754b4-622">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="754b4-623">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-623">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="754b4-624">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="754b4-624">New cmdlets added:</span></span>
        - <span data-ttu-id="754b4-625">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-625">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="754b4-626">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="754b4-626">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="754b4-627">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="754b4-627">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="754b4-628">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="754b4-628">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="754b4-629">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="754b4-629">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="754b4-630">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="754b4-630">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="754b4-631">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="754b4-631">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="754b4-632">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="754b4-632">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="754b4-633">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="754b4-633">New cmdlets added:</span></span>
        - <span data-ttu-id="754b4-634">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="754b4-634">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="754b4-635">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="754b4-635">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="754b4-636">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="754b4-636">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="754b4-637">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="754b4-637">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="754b4-638">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="754b4-638">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="754b4-639">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="754b4-639">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="754b4-640">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="754b4-640">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="754b4-641">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="754b4-641">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="754b4-642">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="754b4-642">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="754b4-643">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="754b4-643">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="754b4-644">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="754b4-644">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="754b4-645">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="754b4-645">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="754b4-646">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="754b4-646">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="754b4-647">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="754b4-647">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="754b4-648">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="754b4-648">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="754b4-649">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="754b4-649">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="754b4-650">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="754b4-650">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="754b4-651">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="754b4-651">New cmdlets added:</span></span>
        - <span data-ttu-id="754b4-652">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="754b4-652">New-AzIpGroup</span></span>
        - <span data-ttu-id="754b4-653">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="754b4-653">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="754b4-654">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="754b4-654">Get-AzIpGroup</span></span>
        - <span data-ttu-id="754b4-655">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="754b4-655">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="754b4-656">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="754b4-656">Az.ServiceFabric</span></span>
* <span data-ttu-id="754b4-657">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="754b4-657">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-658">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-658">Az.Sql</span></span>
* <span data-ttu-id="754b4-659">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="754b4-659">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="754b4-660">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="754b4-660">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="754b4-661">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="754b4-661">Removed deprecated aliases:</span></span>
* <span data-ttu-id="754b4-662">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="754b4-662">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="754b4-663">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="754b4-663">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="754b4-664">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="754b4-664">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="754b4-665">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="754b4-665">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="754b4-666">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="754b4-666">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="754b4-667">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="754b4-667">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-668">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-668">Az.Storage</span></span>
* <span data-ttu-id="754b4-669">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="754b4-669">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="754b4-670">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-670">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="754b4-671">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-671">Set-AzStorageAccount</span></span>
* <span data-ttu-id="754b4-672">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="754b4-672">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="754b4-673">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="754b4-673">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="754b4-674">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="754b4-674">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="754b4-675">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-675">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="754b4-676">Geral</span><span class="sxs-lookup"><span data-stu-id="754b4-676">General</span></span>
* <span data-ttu-id="754b4-677">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="754b4-677">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="754b4-678">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-678">Az.Accounts</span></span>
* <span data-ttu-id="754b4-679">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="754b4-679">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="754b4-680">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="754b4-680">Az.ApiManagement</span></span>
* <span data-ttu-id="754b4-681">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="754b4-681">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="754b4-682">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="754b4-682">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="754b4-683">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="754b4-683">Az.Automation</span></span>
* <span data-ttu-id="754b4-684">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="754b4-684">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="754b4-685">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="754b4-685">Az.Batch</span></span>
* <span data-ttu-id="754b4-686">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="754b4-686">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-687">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-687">Az.Compute</span></span>
* <span data-ttu-id="754b4-688">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="754b4-688">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="754b4-689">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="754b4-689">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="754b4-690">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="754b4-690">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="754b4-691">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="754b4-691">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="754b4-692">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="754b4-692">Az.DataFactory</span></span>
* <span data-ttu-id="754b4-693">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="754b4-693">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="754b4-694">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="754b4-694">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="754b4-695">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="754b4-695">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="754b4-696">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="754b4-696">Az.DataLakeStore</span></span>
* <span data-ttu-id="754b4-697">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="754b4-697">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="754b4-698">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="754b4-698">Az.HealthcareApis</span></span>
* <span data-ttu-id="754b4-699">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="754b4-699">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="754b4-700">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="754b4-700">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="754b4-701">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="754b4-701">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="754b4-702">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="754b4-702">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="754b4-703">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="754b4-703">Az.IotHub</span></span>
* <span data-ttu-id="754b4-704">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="754b4-704">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="754b4-705">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="754b4-705">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="754b4-706">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="754b4-706">Az.Monitor</span></span>
* <span data-ttu-id="754b4-707">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="754b4-707">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="754b4-708">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="754b4-708">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="754b4-709">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="754b4-709">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="754b4-710">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="754b4-710">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-711">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-711">Az.Network</span></span>
* <span data-ttu-id="754b4-712">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="754b4-712">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="754b4-713">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="754b4-713">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="754b4-714">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="754b4-714">New cmdlets added:</span></span>
        - <span data-ttu-id="754b4-715">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="754b4-715">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="754b4-716">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-716">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="754b4-717">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="754b4-717">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="754b4-718">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="754b4-718">Updated cmdlets:</span></span>
        - <span data-ttu-id="754b4-719">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-719">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="754b4-720">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-720">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="754b4-721">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-721">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="754b4-722">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="754b4-722">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="754b4-723">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="754b4-723">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="754b4-724">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="754b4-724">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="754b4-725">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="754b4-725">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="754b4-726">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="754b4-726">Az.RedisCache</span></span>
* <span data-ttu-id="754b4-727">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="754b4-727">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-728">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-728">Az.Sql</span></span>
* <span data-ttu-id="754b4-729">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="754b4-729">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-730">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-730">Az.Storage</span></span>
* <span data-ttu-id="754b4-731">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="754b4-731">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="754b4-732">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="754b4-732">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="754b4-733">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="754b4-733">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="754b4-734">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="754b4-734">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="754b4-735">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-735">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="754b4-736">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="754b4-736">Az.StorageSync</span></span>
* <span data-ttu-id="754b4-737">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="754b4-737">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="754b4-738">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-738">Az.Websites</span></span>
* <span data-ttu-id="754b4-739">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="754b4-739">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="754b4-740">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-740">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="754b4-741">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="754b4-741">Az.ApiManagement</span></span>
* <span data-ttu-id="754b4-742">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="754b4-742">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="754b4-743">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="754b4-743">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="754b4-744">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="754b4-744">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="754b4-745">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="754b4-745">Az.Automation</span></span>
* <span data-ttu-id="754b4-746">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="754b4-746">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="754b4-747">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="754b4-747">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="754b4-748">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="754b4-748">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-749">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-749">Az.Compute</span></span>
* <span data-ttu-id="754b4-750">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-750">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="754b4-751">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-751">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="754b4-752">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="754b4-752">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="754b4-753">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="754b4-753">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="754b4-754">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="754b4-754">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="754b4-755">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="754b4-755">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="754b4-756">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="754b4-756">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="754b4-757">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="754b4-757">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="754b4-758">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="754b4-758">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="754b4-759">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="754b4-759">Az.DataFactory</span></span>
* <span data-ttu-id="754b4-760">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="754b4-760">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="754b4-761">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="754b4-761">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="754b4-762">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="754b4-762">Az.HDInsight</span></span>
* <span data-ttu-id="754b4-763">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="754b4-763">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="754b4-764">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="754b4-764">Az.IotHub</span></span>
* <span data-ttu-id="754b4-765">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="754b4-765">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="754b4-766">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="754b4-766">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="754b4-767">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="754b4-767">New cmdlets are:</span></span>
    - <span data-ttu-id="754b4-768">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="754b4-768">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="754b4-769">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="754b4-769">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="754b4-770">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="754b4-770">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="754b4-771">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="754b4-771">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="754b4-772">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="754b4-772">Az.Monitor</span></span>
* <span data-ttu-id="754b4-773">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="754b4-773">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="754b4-774">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="754b4-774">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="754b4-775">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="754b4-775">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="754b4-776">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="754b4-776">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="754b4-777">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="754b4-777">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="754b4-778">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="754b4-778">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="754b4-779">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="754b4-779">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="754b4-780">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="754b4-780">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="754b4-781">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="754b4-781">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="754b4-782">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="754b4-782">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="754b4-783">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="754b4-783">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="754b4-784">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="754b4-784">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="754b4-785">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="754b4-785">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="754b4-786">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="754b4-786">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="754b4-787">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="754b4-787">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="754b4-788">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="754b4-788">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="754b4-789">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="754b4-789">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="754b4-790">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="754b4-790">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="754b4-791">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="754b4-791">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="754b4-792">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="754b4-792">Overall improved help files</span></span>
* <span data-ttu-id="754b4-793">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="754b4-793">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-794">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-794">Az.Network</span></span>
* <span data-ttu-id="754b4-795">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="754b4-795">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="754b4-796">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="754b4-796">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="754b4-797">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="754b4-797">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="754b4-798">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="754b4-798">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="754b4-799">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="754b4-799">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="754b4-800">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="754b4-800">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="754b4-801">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="754b4-801">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="754b4-802">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="754b4-802">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="754b4-803">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="754b4-803">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="754b4-804">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="754b4-804">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="754b4-805">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="754b4-805">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="754b4-806">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="754b4-806">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="754b4-807">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="754b4-807">New cmdlets</span></span>
        - <span data-ttu-id="754b4-808">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="754b4-808">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="754b4-809">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-809">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="754b4-810">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="754b4-810">Updated cmdlet:</span></span>
        - <span data-ttu-id="754b4-811">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="754b4-811">New-VpnSite</span></span>
        - <span data-ttu-id="754b4-812">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="754b4-812">Update-VpnSite</span></span>
        - <span data-ttu-id="754b4-813">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-813">New-VpnConnection</span></span>
        - <span data-ttu-id="754b4-814">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-814">Update-VpnConnection</span></span>
* <span data-ttu-id="754b4-815">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="754b4-815">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-816">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-816">Az.RecoveryServices</span></span>
* <span data-ttu-id="754b4-817">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="754b4-817">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="754b4-818">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="754b4-818">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-819">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-819">Az.Resources</span></span>
* <span data-ttu-id="754b4-820">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="754b4-820">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="754b4-821">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="754b4-821">Az.ServiceFabric</span></span>
* <span data-ttu-id="754b4-822">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="754b4-822">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="754b4-823">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="754b4-823">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="754b4-824">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="754b4-824">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="754b4-825">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="754b4-825">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="754b4-826">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="754b4-826">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="754b4-827">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="754b4-827">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="754b4-828">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="754b4-828">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="754b4-829">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="754b4-829">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="754b4-830">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="754b4-830">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="754b4-831">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="754b4-831">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="754b4-832">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="754b4-832">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="754b4-833">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="754b4-833">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="754b4-834">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="754b4-834">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="754b4-835">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="754b4-835">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="754b4-836">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="754b4-836">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="754b4-837">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="754b4-837">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="754b4-838">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="754b4-838">Az.SignalR</span></span>
* <span data-ttu-id="754b4-839">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="754b4-839">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-840">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-840">Az.Sql</span></span>
* <span data-ttu-id="754b4-841">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="754b4-841">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="754b4-842">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="754b4-842">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="754b4-843">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="754b4-843">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="754b4-844">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="754b4-844">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="754b4-845">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="754b4-845">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-846">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-846">Az.Storage</span></span>
* <span data-ttu-id="754b4-847">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="754b4-847">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="754b4-848">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="754b4-848">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="754b4-849">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="754b4-849">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="754b4-850">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="754b4-850">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="754b4-851">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="754b4-851">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="754b4-852">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="754b4-852">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="754b4-853">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="754b4-853">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="754b4-854">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="754b4-854">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="754b4-855">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="754b4-855">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="754b4-856">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="754b4-856">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="754b4-857">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="754b4-857">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="754b4-858">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-858">Az.Websites</span></span>
* <span data-ttu-id="754b4-859">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="754b4-859">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="754b4-860">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="754b4-860">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="754b4-861">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="754b4-861">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="754b4-862">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-862">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="754b4-863">Geral</span><span class="sxs-lookup"><span data-stu-id="754b4-863">General</span></span>
* <span data-ttu-id="754b4-864">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="754b4-864">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="754b4-865">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-865">Az.Accounts</span></span>
* <span data-ttu-id="754b4-866">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="754b4-866">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="754b4-867">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="754b4-867">Az.Aks</span></span>
* <span data-ttu-id="754b4-868">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="754b4-868">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="754b4-869">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="754b4-869">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="754b4-870">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="754b4-870">Az.ApiManagement</span></span>
* <span data-ttu-id="754b4-871">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="754b4-871">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="754b4-872">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="754b4-872">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="754b4-873">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="754b4-873">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="754b4-874">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="754b4-874">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="754b4-875">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="754b4-875">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="754b4-876">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="754b4-876">Az.Batch</span></span>
* <span data-ttu-id="754b4-877">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="754b4-877">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="754b4-878">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="754b4-878">Az.Cdn</span></span>
* <span data-ttu-id="754b4-879">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="754b4-879">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-880">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-880">Az.Compute</span></span>
* <span data-ttu-id="754b4-881">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-881">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="754b4-882">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="754b4-882">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="754b4-883">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="754b4-883">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="754b4-884">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="754b4-884">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="754b4-885">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="754b4-885">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="754b4-886">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="754b4-886">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="754b4-887">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="754b4-887">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="754b4-888">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="754b4-888">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="754b4-889">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="754b4-889">Az.DataFactory</span></span>
* <span data-ttu-id="754b4-890">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="754b4-890">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="754b4-891">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="754b4-891">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="754b4-892">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="754b4-892">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="754b4-893">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="754b4-893">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="754b4-894">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="754b4-894">Az.DataLakeStore</span></span>
* <span data-ttu-id="754b4-895">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="754b4-895">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="754b4-896">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="754b4-896">Az.EventHub</span></span>
* <span data-ttu-id="754b4-897">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="754b4-897">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="754b4-898">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="754b4-898">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="754b4-899">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="754b4-899">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="754b4-900">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="754b4-900">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="754b4-901">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="754b4-901">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="754b4-902">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="754b4-902">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="754b4-903">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="754b4-903">Az.Monitor</span></span>
* <span data-ttu-id="754b4-904">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="754b4-904">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-905">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-905">Az.Network</span></span>
* <span data-ttu-id="754b4-906">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="754b4-906">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="754b4-907">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="754b4-907">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="754b4-908">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="754b4-908">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="754b4-909">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="754b4-909">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="754b4-910">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="754b4-910">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="754b4-911">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="754b4-911">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="754b4-912">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="754b4-912">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="754b4-913">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="754b4-913">Az.OperationalInsights</span></span>
* <span data-ttu-id="754b4-914">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="754b4-914">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="754b4-915">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="754b4-915">Added example</span></span>
    - <span data-ttu-id="754b4-916">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="754b4-916">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="754b4-917">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="754b4-917">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="754b4-918">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="754b4-918">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-919">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-919">Az.RecoveryServices</span></span>
* <span data-ttu-id="754b4-920">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="754b4-920">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-921">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-921">Az.Resources</span></span>
* <span data-ttu-id="754b4-922">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="754b4-922">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="754b4-923">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="754b4-923">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="754b4-924">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="754b4-924">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="754b4-925">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="754b4-925">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="754b4-926">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="754b4-926">Az.ServiceBus</span></span>
* <span data-ttu-id="754b4-927">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="754b4-927">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="754b4-928">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="754b4-928">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="754b4-929">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="754b4-929">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="754b4-930">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="754b4-930">Az.ServiceFabric</span></span>
* <span data-ttu-id="754b4-931">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="754b4-931">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="754b4-932">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="754b4-932">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="754b4-933">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="754b4-933">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="754b4-934">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="754b4-934">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="754b4-935">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="754b4-935">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="754b4-936">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="754b4-936">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-937">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-937">Az.Sql</span></span>
* <span data-ttu-id="754b4-938">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="754b4-938">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-939">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-939">Az.Storage</span></span>
* <span data-ttu-id="754b4-940">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="754b4-940">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="754b4-941">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="754b4-941">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="754b4-942">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="754b4-942">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="754b4-943">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="754b4-943">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="754b4-944">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="754b4-944">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="754b4-945">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="754b4-945">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="754b4-946">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-946">Az.Websites</span></span>
* <span data-ttu-id="754b4-947">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="754b4-947">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="754b4-948">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-948">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="754b4-949">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-949">Az.Accounts</span></span>
* <span data-ttu-id="754b4-950">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="754b4-950">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="754b4-951">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="754b4-951">Az.ApplicationInsights</span></span>
* <span data-ttu-id="754b4-952">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="754b4-952">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="754b4-953">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="754b4-953">Az.Automation</span></span>
* <span data-ttu-id="754b4-954">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="754b4-954">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="754b4-955">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="754b4-955">Az.CognitiveServices</span></span>
* <span data-ttu-id="754b4-956">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="754b4-956">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-957">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-957">Az.Compute</span></span>
* <span data-ttu-id="754b4-958">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="754b4-958">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="754b4-959">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="754b4-959">Az.ContainerRegistry</span></span>
* <span data-ttu-id="754b4-960">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="754b4-960">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="754b4-961">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="754b4-961">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="754b4-962">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="754b4-962">Az.DataFactory</span></span>
* <span data-ttu-id="754b4-963">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="754b4-963">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="754b4-964">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="754b4-964">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="754b4-965">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="754b4-965">Az.EventHub</span></span>
* <span data-ttu-id="754b4-966">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="754b4-966">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="754b4-967">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="754b4-967">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="754b4-968">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="754b4-968">Az.KeyVault</span></span>
* <span data-ttu-id="754b4-969">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="754b4-969">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="754b4-970">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="754b4-970">Az.LogicApp</span></span>
* <span data-ttu-id="754b4-971">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="754b4-971">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="754b4-972">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="754b4-972">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="754b4-973">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="754b4-973">Az.ManagedServices</span></span>
* <span data-ttu-id="754b4-974">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="754b4-974">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-975">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-975">Az.Network</span></span>
* <span data-ttu-id="754b4-976">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="754b4-976">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="754b4-977">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="754b4-977">New cmdlets</span></span>
        - <span data-ttu-id="754b4-978">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="754b4-978">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="754b4-979">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="754b4-979">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="754b4-980">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-980">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="754b4-981">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-981">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="754b4-982">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-982">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="754b4-983">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-983">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="754b4-984">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="754b4-984">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="754b4-985">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="754b4-985">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="754b4-986">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="754b4-986">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="754b4-987">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-987">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="754b4-988">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="754b4-988">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="754b4-989">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="754b4-989">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="754b4-990">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="754b4-990">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="754b4-991">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="754b4-991">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="754b4-992">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="754b4-992">Updated cmdlets</span></span>
        - <span data-ttu-id="754b4-993">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-993">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="754b4-994">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-994">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="754b4-995">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-995">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="754b4-996">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-996">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="754b4-997">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="754b4-997">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="754b4-998">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="754b4-998">Updated cmdlet:</span></span>
        - <span data-ttu-id="754b4-999">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-999">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="754b4-1000">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-1000">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="754b4-1001">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-1001">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="754b4-1002">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="754b4-1002">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="754b4-1003">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="754b4-1003">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="754b4-1004">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="754b4-1004">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="754b4-1005">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="754b4-1005">Az.OperationalInsights</span></span>
* <span data-ttu-id="754b4-1006">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="754b4-1006">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="754b4-1007">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="754b4-1007">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-1008">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1008">Az.RecoveryServices</span></span>
* <span data-ttu-id="754b4-1009">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="754b4-1009">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="754b4-1010">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="754b4-1010">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="754b4-1011">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="754b4-1011">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="754b4-1012">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="754b4-1012">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="754b4-1013">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="754b4-1013">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="754b4-1014">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="754b4-1014">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="754b4-1015">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="754b4-1015">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="754b4-1016">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="754b4-1016">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="754b4-1017">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="754b4-1017">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="754b4-1018">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="754b4-1018">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-1019">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-1019">Az.Resources</span></span>
- <span data-ttu-id="754b4-1020">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="754b4-1020">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="754b4-1021">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="754b4-1021">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="754b4-1022">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="754b4-1022">Az.ServiceBus</span></span>
* <span data-ttu-id="754b4-1023">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="754b4-1023">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="754b4-1024">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="754b4-1024">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-1025">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1025">Az.Sql</span></span>
* <span data-ttu-id="754b4-1026">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="754b4-1026">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="754b4-1027">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="754b4-1027">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="754b4-1028">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="754b4-1028">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-1029">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-1029">Az.Storage</span></span>
* <span data-ttu-id="754b4-1030">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="754b4-1030">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="754b4-1031">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="754b4-1031">Az.StorageSync</span></span>
* <span data-ttu-id="754b4-1032">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="754b4-1032">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="754b4-1033">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="754b4-1033">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="754b4-1034">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-1034">Az.Websites</span></span>
* <span data-ttu-id="754b4-1035">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="754b4-1035">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="754b4-1036">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="754b4-1036">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="754b4-1037">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="754b4-1037">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="754b4-1038">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-1038">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="754b4-1039">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-1039">Az.Accounts</span></span>
* <span data-ttu-id="754b4-1040">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="754b4-1040">Add support for profile cmdlets</span></span>
* <span data-ttu-id="754b4-1041">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="754b4-1041">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="754b4-1042">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="754b4-1042">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="754b4-1043">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="754b4-1043">Az.Advisor</span></span>
* <span data-ttu-id="754b4-1044">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="754b4-1044">GA release of Az.Advisor</span></span>
* <span data-ttu-id="754b4-1045">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="754b4-1045">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="754b4-1046">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="754b4-1046">Az.ApiManagement</span></span>
* <span data-ttu-id="754b4-1047">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="754b4-1047">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="754b4-1048">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="754b4-1048">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="754b4-1049">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="754b4-1049">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="754b4-1050">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="754b4-1050">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="754b4-1051">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="754b4-1051">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="754b4-1052">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="754b4-1052">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="754b4-1053">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="754b4-1053">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="754b4-1054">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="754b4-1054">Az.Automation</span></span>
* <span data-ttu-id="754b4-1055">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="754b4-1055">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-1056">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-1056">Az.Compute</span></span>
* <span data-ttu-id="754b4-1057">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-1057">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="754b4-1058">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="754b4-1058">Az.DataFactory</span></span>
* <span data-ttu-id="754b4-1059">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="754b4-1059">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="754b4-1060">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="754b4-1060">Az.EventGrid</span></span>
* <span data-ttu-id="754b4-1061">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="754b4-1061">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="754b4-1062">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="754b4-1062">Az.IotHub</span></span>
* <span data-ttu-id="754b4-1063">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="754b4-1063">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-1064">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1064">Az.Network</span></span>
* <span data-ttu-id="754b4-1065">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="754b4-1065">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="754b4-1066">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="754b4-1066">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="754b4-1067">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="754b4-1067">Az.PolicyInsights</span></span>
* <span data-ttu-id="754b4-1068">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="754b4-1068">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="754b4-1069">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="754b4-1069">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="754b4-1070">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="754b4-1070">Az.OperationalInsights</span></span>
* <span data-ttu-id="754b4-1071">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="754b4-1071">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-1072">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1072">Az.RecoveryServices</span></span>
* <span data-ttu-id="754b4-1073">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="754b4-1073">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-1074">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-1074">Az.Resources</span></span>
    - <span data-ttu-id="754b4-1075">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="754b4-1075">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="754b4-1076">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="754b4-1076">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="754b4-1077">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="754b4-1077">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="754b4-1078">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="754b4-1078">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="754b4-1079">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="754b4-1079">Az.ServiceBus</span></span>
* <span data-ttu-id="754b4-1080">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="754b4-1080">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-1081">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1081">Az.Sql</span></span>
* <span data-ttu-id="754b4-1082">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="754b4-1082">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="754b4-1083">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="754b4-1083">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="754b4-1084">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="754b4-1084">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="754b4-1085">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="754b4-1085">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="754b4-1086">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="754b4-1086">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="754b4-1087">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="754b4-1087">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="754b4-1088">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="754b4-1088">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="754b4-1089">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="754b4-1089">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="754b4-1090">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="754b4-1090">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-1091">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-1091">Az.Storage</span></span>
* <span data-ttu-id="754b4-1092">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="754b4-1092">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="754b4-1093">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="754b4-1093">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="754b4-1094">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="754b4-1094">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="754b4-1095">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="754b4-1095">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="754b4-1096">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="754b4-1096">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="754b4-1097">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-1097">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="754b4-1098">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-1098">Set-AzStorageAccount</span></span>
* <span data-ttu-id="754b4-1099">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="754b4-1099">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="754b4-1100">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="754b4-1100">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="754b4-1101">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="754b4-1101">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="754b4-1102">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="754b4-1102">Az.StorageSync</span></span>
* <span data-ttu-id="754b4-1103">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="754b4-1103">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="754b4-1104">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-1104">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="754b4-1105">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-1105">Az.Accounts</span></span>
* <span data-ttu-id="754b4-1106">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="754b4-1106">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="754b4-1107">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="754b4-1107">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="754b4-1108">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="754b4-1108">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="754b4-1109">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="754b4-1109">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="754b4-1110">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="754b4-1110">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-1111">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-1111">Az.Compute</span></span>
* <span data-ttu-id="754b4-1112">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="754b4-1112">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="754b4-1113">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="754b4-1113">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="754b4-1114">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="754b4-1114">Az.Dns</span></span>
* <span data-ttu-id="754b4-1115">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="754b4-1115">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="754b4-1116">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="754b4-1116">Az.EventGrid</span></span>
* <span data-ttu-id="754b4-1117">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="754b4-1117">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="754b4-1118">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="754b4-1118">New cmdlets:</span></span>
    - <span data-ttu-id="754b4-1119">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="754b4-1119">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="754b4-1120">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="754b4-1120">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="754b4-1121">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="754b4-1121">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="754b4-1122">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-1122">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="754b4-1123">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="754b4-1123">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="754b4-1124">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="754b4-1124">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="754b4-1125">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="754b4-1125">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="754b4-1126">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="754b4-1126">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="754b4-1127">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="754b4-1127">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="754b4-1128">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="754b4-1128">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="754b4-1129">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="754b4-1129">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="754b4-1130">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="754b4-1130">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="754b4-1131">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="754b4-1131">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="754b4-1132">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="754b4-1132">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="754b4-1133">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="754b4-1133">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="754b4-1134">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="754b4-1134">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="754b4-1135">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="754b4-1135">Updated cmdlets:</span></span>
    - <span data-ttu-id="754b4-1136">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="754b4-1136">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="754b4-1137">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="754b4-1137">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="754b4-1138">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="754b4-1138">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="754b4-1139">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="754b4-1139">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="754b4-1140">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="754b4-1140">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="754b4-1141">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="754b4-1141">Event subscription expiration date,</span></span>
            - <span data-ttu-id="754b4-1142">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="754b4-1142">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="754b4-1143">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="754b4-1143">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="754b4-1144">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="754b4-1144">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="754b4-1145">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="754b4-1145">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="754b4-1146">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="754b4-1146">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="754b4-1147">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="754b4-1147">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="754b4-1148">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="754b4-1148">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="754b4-1149">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="754b4-1149">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="754b4-1150">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="754b4-1150">Az.FrontDoor</span></span>
* <span data-ttu-id="754b4-1151">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="754b4-1151">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="754b4-1152">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="754b4-1152">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="754b4-1153">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="754b4-1153">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="754b4-1154">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="754b4-1154">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-1155">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1155">Az.Network</span></span>
* <span data-ttu-id="754b4-1156">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="754b4-1156">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="754b4-1157">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="754b4-1157">New cmdlets</span></span>
        - <span data-ttu-id="754b4-1158">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="754b4-1158">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="754b4-1159">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="754b4-1159">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="754b4-1160">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="754b4-1160">New cmdlets</span></span>
        - <span data-ttu-id="754b4-1161">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="754b4-1161">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="754b4-1162">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="754b4-1162">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="754b4-1163">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="754b4-1163">New cmdlets</span></span>
        - <span data-ttu-id="754b4-1164">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="754b4-1164">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="754b4-1165">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="754b4-1165">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="754b4-1166">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="754b4-1166">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="754b4-1167">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-1167">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="754b4-1168">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-1168">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="754b4-1169">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="754b4-1169">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="754b4-1170">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="754b4-1170">New cmdlets</span></span>
        - <span data-ttu-id="754b4-1171">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="754b4-1171">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="754b4-1172">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="754b4-1172">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="754b4-1173">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="754b4-1173">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="754b4-1174">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-1174">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="754b4-1175">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="754b4-1175">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="754b4-1176">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="754b4-1176">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="754b4-1177">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="754b4-1177">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="754b4-1178">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="754b4-1178">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="754b4-1179">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="754b4-1179">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="754b4-1180">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="754b4-1180">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="754b4-1181">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="754b4-1181">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="754b4-1182">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="754b4-1182">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="754b4-1183">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="754b4-1183">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="754b4-1184">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="754b4-1184">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="754b4-1185">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="754b4-1185">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="754b4-1186">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="754b4-1186">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="754b4-1187">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="754b4-1187">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="754b4-1188">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="754b4-1188">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="754b4-1189">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="754b4-1189">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="754b4-1190">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="754b4-1190">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="754b4-1191">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="754b4-1191">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="754b4-1192">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="754b4-1192">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="754b4-1193">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="754b4-1193">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="754b4-1194">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="754b4-1194">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="754b4-1195">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="754b4-1195">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="754b4-1196">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="754b4-1196">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="754b4-1197">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="754b4-1197">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="754b4-1198">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="754b4-1198">Az.OperationalInsights</span></span>
* <span data-ttu-id="754b4-1199">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="754b4-1199">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-1200">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-1200">Az.Resources</span></span>
* <span data-ttu-id="754b4-1201">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="754b4-1201">Support for additional Template Export options</span></span>
    - <span data-ttu-id="754b4-1202">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="754b4-1202">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="754b4-1203">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="754b4-1203">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="754b4-1204">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="754b4-1204">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="754b4-1205">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="754b4-1205">Az.ServiceFabric</span></span>
* <span data-ttu-id="754b4-1206">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="754b4-1206">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-1207">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1207">Az.Sql</span></span>
* <span data-ttu-id="754b4-1208">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="754b4-1208">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="754b4-1209">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="754b4-1209">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="754b4-1210">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="754b4-1210">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="754b4-1211">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="754b4-1211">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="754b4-1212">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="754b4-1212">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="754b4-1213">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="754b4-1213">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="754b4-1214">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="754b4-1214">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="754b4-1215">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="754b4-1215">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-1216">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-1216">Az.Storage</span></span>
* <span data-ttu-id="754b4-1217">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="754b4-1217">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="754b4-1218">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-1218">New-AzStorageAccount</span></span>
* <span data-ttu-id="754b4-1219">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="754b4-1219">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="754b4-1220">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="754b4-1220">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="754b4-1221">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-1221">Az.Websites</span></span>
* <span data-ttu-id="754b4-1222">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="754b4-1222">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="754b4-1223">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="754b4-1223">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="754b4-1224">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-1224">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="754b4-1225">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="754b4-1225">Az.Cdn</span></span>
* <span data-ttu-id="754b4-1226">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="754b4-1226">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-1227">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-1227">Az.Compute</span></span>
* <span data-ttu-id="754b4-1228">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="754b4-1228">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="754b4-1229">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="754b4-1229">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="754b4-1230">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="754b4-1230">Az.EventHub</span></span>
* <span data-ttu-id="754b4-1231">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="754b4-1231">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="754b4-1232">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="754b4-1232">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-1233">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1233">Az.Network</span></span>
* <span data-ttu-id="754b4-1234">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="754b4-1234">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="754b4-1235">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="754b4-1235">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="754b4-1236">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="754b4-1236">Az.PolicyInsights</span></span>
* <span data-ttu-id="754b4-1237">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="754b4-1237">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-1238">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1238">Az.RecoveryServices</span></span>
* <span data-ttu-id="754b4-1239">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="754b4-1239">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="754b4-1240">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="754b4-1240">Az.ServiceBus</span></span>
* <span data-ttu-id="754b4-1241">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="754b4-1241">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="754b4-1242">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="754b4-1242">Az.ServiceFabric</span></span>
* <span data-ttu-id="754b4-1243">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="754b4-1243">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="754b4-1244">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="754b4-1244">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-1245">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1245">Az.Sql</span></span>
* <span data-ttu-id="754b4-1246">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="754b4-1246">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="754b4-1247">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="754b4-1247">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="754b4-1248">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="754b4-1248">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="754b4-1249">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="754b4-1249">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="754b4-1250">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-1250">Az.Websites</span></span>
* <span data-ttu-id="754b4-1251">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="754b4-1251">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="754b4-1252">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-1252">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="754b4-1253">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="754b4-1253">Az.ApiManagement</span></span>
* <span data-ttu-id="754b4-1254">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="754b4-1254">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="754b4-1255">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="754b4-1255">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="754b4-1256">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="754b4-1256">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="754b4-1257">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="754b4-1257">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="754b4-1258">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="754b4-1258">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="754b4-1259">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="754b4-1259">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="754b4-1260">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="754b4-1260">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="754b4-1261">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="754b4-1261">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="754b4-1262">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="754b4-1262">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="754b4-1263">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="754b4-1263">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="754b4-1264">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="754b4-1264">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="754b4-1265">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="754b4-1265">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="754b4-1266">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="754b4-1266">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="754b4-1267">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="754b4-1267">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="754b4-1268">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="754b4-1268">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="754b4-1269">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="754b4-1269">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="754b4-1270">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="754b4-1270">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="754b4-1271">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="754b4-1271">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="754b4-1272">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="754b4-1272">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="754b4-1273">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="754b4-1273">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="754b4-1274">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="754b4-1274">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="754b4-1275">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="754b4-1275">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="754b4-1276">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="754b4-1276">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="754b4-1277">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="754b4-1277">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="754b4-1278">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="754b4-1278">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="754b4-1279">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="754b4-1279">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="754b4-1280">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="754b4-1280">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="754b4-1281">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="754b4-1281">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="754b4-1282">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="754b4-1282">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="754b4-1283">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="754b4-1283">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="754b4-1284">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="754b4-1284">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="754b4-1285">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="754b4-1285">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="754b4-1286">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="754b4-1286">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="754b4-1287">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="754b4-1287">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="754b4-1288">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="754b4-1288">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="754b4-1289">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="754b4-1289">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="754b4-1290">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="754b4-1290">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="754b4-1291">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="754b4-1291">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="754b4-1292">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="754b4-1292">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="754b4-1293">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="754b4-1293">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="754b4-1294">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="754b4-1294">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="754b4-1295">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="754b4-1295">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="754b4-1296">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="754b4-1296">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="754b4-1297">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="754b4-1297">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="754b4-1298">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="754b4-1298">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="754b4-1299">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="754b4-1299">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="754b4-1300">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="754b4-1300">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="754b4-1301">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="754b4-1301">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="754b4-1302">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="754b4-1302">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="754b4-1303">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="754b4-1303">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="754b4-1304">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="754b4-1304">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="754b4-1305">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="754b4-1305">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="754b4-1306">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="754b4-1306">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="754b4-1307">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="754b4-1307">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="754b4-1308">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="754b4-1308">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="754b4-1309">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="754b4-1309">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="754b4-1310">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="754b4-1310">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="754b4-1311">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="754b4-1311">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="754b4-1312">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="754b4-1312">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="754b4-1313">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="754b4-1313">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="754b4-1314">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="754b4-1314">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="754b4-1315">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="754b4-1315">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="754b4-1316">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="754b4-1316">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="754b4-1317">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="754b4-1317">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="754b4-1318">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="754b4-1318">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="754b4-1319">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="754b4-1319">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="754b4-1320">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="754b4-1320">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="754b4-1321">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="754b4-1321">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="754b4-1322">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="754b4-1322">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="754b4-1323">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="754b4-1323">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="754b4-1324">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="754b4-1324">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="754b4-1325">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="754b4-1325">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="754b4-1326">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="754b4-1326">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="754b4-1327">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="754b4-1327">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="754b4-1328">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="754b4-1328">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="754b4-1329">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="754b4-1329">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="754b4-1330">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="754b4-1330">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="754b4-1331">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="754b4-1331">Az.Automation</span></span>
* <span data-ttu-id="754b4-1332">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="754b4-1332">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="754b4-1333">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="754b4-1333">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="754b4-1334">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="754b4-1334">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="754b4-1335">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="754b4-1335">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="754b4-1336">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="754b4-1336">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="754b4-1337">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="754b4-1337">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="754b4-1338">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="754b4-1338">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-1339">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-1339">Az.Compute</span></span>
* <span data-ttu-id="754b4-1340">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="754b4-1340">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="754b4-1341">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="754b4-1341">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="754b4-1342">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="754b4-1342">Az.DataLakeStore</span></span>
* <span data-ttu-id="754b4-1343">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="754b4-1343">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="754b4-1344">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="754b4-1344">Az.Monitor</span></span>
* <span data-ttu-id="754b4-1345">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="754b4-1345">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-1346">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1346">Az.Network</span></span>
* <span data-ttu-id="754b4-1347">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="754b4-1347">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="754b4-1348">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="754b4-1348">Updated cmdlet:</span></span>
        - <span data-ttu-id="754b4-1349">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="754b4-1349">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="754b4-1350">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="754b4-1350">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-1351">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-1351">Az.Resources</span></span>
* <span data-ttu-id="754b4-1352">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="754b4-1352">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-1353">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1353">Az.Sql</span></span>
* <span data-ttu-id="754b4-1354">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="754b4-1354">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="754b4-1355">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-1355">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="754b4-1356">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-1356">Az.Accounts</span></span>
* <span data-ttu-id="754b4-1357">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="754b4-1357">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="754b4-1358">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1358">Az.CognitiveServices</span></span>
* <span data-ttu-id="754b4-1359">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="754b4-1359">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="754b4-1360">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="754b4-1360">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-1361">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-1361">Az.Compute</span></span>
* <span data-ttu-id="754b4-1362">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="754b4-1362">Proximity placement group feature.</span></span>
    - <span data-ttu-id="754b4-1363">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="754b4-1363">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="754b4-1364">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-1364">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="754b4-1365">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="754b4-1365">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="754b4-1366">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="754b4-1366">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="754b4-1367">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="754b4-1367">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="754b4-1368">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="754b4-1368">Breaking changes</span></span>
    - <span data-ttu-id="754b4-1369">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="754b4-1369">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="754b4-1370">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="754b4-1370">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="754b4-1371">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="754b4-1371">Az.DeploymentManager</span></span>
* <span data-ttu-id="754b4-1372">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="754b4-1372">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="754b4-1373">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="754b4-1373">Az.Dns</span></span>
* <span data-ttu-id="754b4-1374">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="754b4-1374">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="754b4-1375">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="754b4-1375">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="754b4-1376">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="754b4-1376">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="754b4-1377">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="754b4-1377">Az.FrontDoor</span></span>
* <span data-ttu-id="754b4-1378">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="754b4-1378">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="754b4-1379">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="754b4-1379">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="754b4-1380">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="754b4-1380">Az.HDInsight</span></span>
* <span data-ttu-id="754b4-1381">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="754b4-1381">Removed two cmdlets:</span></span>
    - <span data-ttu-id="754b4-1382">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="754b4-1382">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="754b4-1383">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="754b4-1383">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="754b4-1384">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="754b4-1384">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="754b4-1385">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="754b4-1385">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="754b4-1386">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="754b4-1386">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="754b4-1387">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="754b4-1387">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="754b4-1388">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="754b4-1388">Az.Monitor</span></span>
* <span data-ttu-id="754b4-1389">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="754b4-1389">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="754b4-1390">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="754b4-1390">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="754b4-1391">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="754b4-1391">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="754b4-1392">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="754b4-1392">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="754b4-1393">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="754b4-1393">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="754b4-1394">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="754b4-1394">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="754b4-1395">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="754b4-1395">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="754b4-1396">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="754b4-1396">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="754b4-1397">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="754b4-1397">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="754b4-1398">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="754b4-1398">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="754b4-1399">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="754b4-1399">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="754b4-1400">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="754b4-1400">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="754b4-1401">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="754b4-1401">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="754b4-1402">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="754b4-1402">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-1403">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1403">Az.Network</span></span>
* <span data-ttu-id="754b4-1404">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="754b4-1404">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="754b4-1405">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="754b4-1405">New cmdlets</span></span>
        - <span data-ttu-id="754b4-1406">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="754b4-1406">New-AzNatGateway</span></span>
        - <span data-ttu-id="754b4-1407">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="754b4-1407">Get-AzNatGateway</span></span>
        - <span data-ttu-id="754b4-1408">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="754b4-1408">Set-AzNatGateway</span></span>
        - <span data-ttu-id="754b4-1409">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="754b4-1409">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="754b4-1410">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="754b4-1410">Updated cmdlets</span></span>
        - <span data-ttu-id="754b4-1411">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="754b4-1411">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="754b4-1412">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="754b4-1412">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="754b4-1413">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="754b4-1413">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="754b4-1414">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="754b4-1414">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="754b4-1415">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="754b4-1415">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="754b4-1416">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="754b4-1416">Az.PolicyInsights</span></span>
* <span data-ttu-id="754b4-1417">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="754b4-1417">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="754b4-1418">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="754b4-1418">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="754b4-1419">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="754b4-1419">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-1420">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1420">Az.RecoveryServices</span></span>
* <span data-ttu-id="754b4-1421">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="754b4-1421">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="754b4-1422">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="754b4-1422">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="754b4-1423">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="754b4-1423">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="754b4-1424">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-1424">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="754b4-1425">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="754b4-1425">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="754b4-1426">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="754b4-1426">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="754b4-1427">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="754b4-1427">Az.Relay</span></span>
* <span data-ttu-id="754b4-1428">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="754b4-1428">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="754b4-1429">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="754b4-1429">Az.ServiceBus</span></span>
* <span data-ttu-id="754b4-1430">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="754b4-1430">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-1431">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-1431">Az.Storage</span></span>
* <span data-ttu-id="754b4-1432">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="754b4-1432">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="754b4-1433">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="754b4-1433">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="754b4-1434">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="754b4-1434">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="754b4-1435">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-1435">New-AzStorageAccount</span></span>
* <span data-ttu-id="754b4-1436">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="754b4-1436">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="754b4-1437">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-1437">New-AzStorageAccount</span></span>
    - <span data-ttu-id="754b4-1438">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-1438">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="754b4-1439">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-1439">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="754b4-1440">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-1440">Az.Websites</span></span>
* <span data-ttu-id="754b4-1441">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="754b4-1441">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="754b4-1442">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="754b4-1442">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="754b4-1443">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-1443">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="754b4-1444">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="754b4-1444">Highlights since the last major release</span></span>
* <span data-ttu-id="754b4-1445">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="754b4-1445">General availability of `Az` module</span></span>
* <span data-ttu-id="754b4-1446">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="754b4-1446">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="754b4-1447">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="754b4-1447">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="754b4-1448">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1448">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="754b4-1449">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="754b4-1449">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="754b4-1450">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="754b4-1450">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="754b4-1451">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="754b4-1451">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="754b4-1452">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-1452">Az.Accounts</span></span>
* <span data-ttu-id="754b4-1453">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="754b4-1453">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="754b4-1454">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="754b4-1454">Az.Batch</span></span>
* <span data-ttu-id="754b4-1455">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1455">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="754b4-1456">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="754b4-1456">Az.Cdn</span></span>
* <span data-ttu-id="754b4-1457">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1457">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="754b4-1458">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1458">Az.CognitiveServices</span></span>
* <span data-ttu-id="754b4-1459">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1459">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-1460">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-1460">Az.Compute</span></span>
* <span data-ttu-id="754b4-1461">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="754b4-1461">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="754b4-1462">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1462">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="754b4-1463">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="754b4-1463">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="754b4-1464">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="754b4-1464">Az.DataFactory</span></span>
* <span data-ttu-id="754b4-1465">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="754b4-1465">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="754b4-1466">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="754b4-1466">Az.DataLakeStore</span></span>
* <span data-ttu-id="754b4-1467">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1467">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="754b4-1468">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="754b4-1468">Az.EventGrid</span></span>
* <span data-ttu-id="754b4-1469">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="754b4-1469">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="754b4-1470">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="754b4-1470">Az.EventHub</span></span>
* <span data-ttu-id="754b4-1471">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="754b4-1471">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="754b4-1472">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="754b4-1472">Az.HDInsight</span></span>
* <span data-ttu-id="754b4-1473">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1473">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="754b4-1474">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="754b4-1474">Az.IotHub</span></span>
* <span data-ttu-id="754b4-1475">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1475">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="754b4-1476">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="754b4-1476">Az.KeyVault</span></span>
* <span data-ttu-id="754b4-1477">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1477">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="754b4-1478">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="754b4-1478">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="754b4-1479">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="754b4-1479">Az.MachineLearning</span></span>
* <span data-ttu-id="754b4-1480">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1480">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="754b4-1481">Az.Media</span><span class="sxs-lookup"><span data-stu-id="754b4-1481">Az.Media</span></span>
* <span data-ttu-id="754b4-1482">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1482">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="754b4-1483">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="754b4-1483">Az.Monitor</span></span>
  * <span data-ttu-id="754b4-1484">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="754b4-1484">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="754b4-1485">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="754b4-1485">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="754b4-1486">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="754b4-1486">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="754b4-1487">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="754b4-1487">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="754b4-1488">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="754b4-1488">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="754b4-1489">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="754b4-1489">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="754b4-1490">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="754b4-1490">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-1491">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1491">Az.Network</span></span>
* <span data-ttu-id="754b4-1492">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1492">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="754b4-1493">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="754b4-1493">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="754b4-1494">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="754b4-1494">Az.NotificationHubs</span></span>
* <span data-ttu-id="754b4-1495">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1495">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="754b4-1496">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="754b4-1496">Az.OperationalInsights</span></span>
* <span data-ttu-id="754b4-1497">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1497">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="754b4-1498">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="754b4-1498">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="754b4-1499">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1499">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-1500">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1500">Az.RecoveryServices</span></span>
* <span data-ttu-id="754b4-1501">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1501">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="754b4-1502">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="754b4-1502">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="754b4-1503">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="754b4-1503">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="754b4-1504">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="754b4-1504">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="754b4-1505">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="754b4-1505">Az.RedisCache</span></span>
* <span data-ttu-id="754b4-1506">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1506">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-1507">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-1507">Az.Resources</span></span>
* <span data-ttu-id="754b4-1508">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="754b4-1508">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-1509">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1509">Az.Sql</span></span>
* <span data-ttu-id="754b4-1510">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="754b4-1510">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="754b4-1511">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1511">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="754b4-1512">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="754b4-1512">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="754b4-1513">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="754b4-1513">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="754b4-1514">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="754b4-1514">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="754b4-1515">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="754b4-1515">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="754b4-1516">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="754b4-1516">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="754b4-1517">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-1517">Az.Websites</span></span>
* <span data-ttu-id="754b4-1518">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="754b4-1518">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="754b4-1519">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="754b4-1519">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="754b4-1520">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="754b4-1520">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="754b4-1521">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="754b4-1521">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="754b4-1522">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-1522">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="754b4-1523">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="754b4-1523">Highlights since the last major release</span></span>
* <span data-ttu-id="754b4-1524">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="754b4-1524">General availability of `Az` module</span></span>
* <span data-ttu-id="754b4-1525">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="754b4-1525">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="754b4-1526">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="754b4-1526">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="754b4-1527">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1527">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="754b4-1528">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="754b4-1528">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="754b4-1529">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="754b4-1529">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="754b4-1530">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="754b4-1530">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="754b4-1531">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-1531">Az.Accounts</span></span>
* <span data-ttu-id="754b4-1532">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="754b4-1532">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="754b4-1533">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1533">Az.AnalysisServices</span></span>
* <span data-ttu-id="754b4-1534">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="754b4-1534">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="754b4-1535">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="754b4-1535">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="754b4-1536">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="754b4-1536">Az.Automation</span></span>
* <span data-ttu-id="754b4-1537">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="754b4-1537">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="754b4-1538">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="754b4-1538">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="754b4-1539">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="754b4-1539">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-1540">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-1540">Az.Compute</span></span>
* <span data-ttu-id="754b4-1541">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-1541">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="754b4-1542">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="754b4-1542">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="754b4-1543">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="754b4-1543">Az.ContainerInstance</span></span>
* <span data-ttu-id="754b4-1544">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="754b4-1544">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="754b4-1545">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="754b4-1545">Az.DataFactory</span></span>
* <span data-ttu-id="754b4-1546">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="754b4-1546">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="754b4-1547">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="754b4-1547">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-1548">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-1548">Az.Resources</span></span>
* <span data-ttu-id="754b4-1549">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="754b4-1549">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="754b4-1550">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="754b4-1550">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="754b4-1551">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="754b4-1551">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="754b4-1552">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="754b4-1552">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="754b4-1553">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="754b4-1553">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="754b4-1554">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="754b4-1554">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-1555">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1555">Az.Sql</span></span>
* <span data-ttu-id="754b4-1556">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="754b4-1556">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-1557">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-1557">Az.Storage</span></span>
* <span data-ttu-id="754b4-1558">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="754b4-1558">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="754b4-1559">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="754b4-1559">New-AzStorageContext</span></span>
* <span data-ttu-id="754b4-1560">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="754b4-1560">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="754b4-1561">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="754b4-1561">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="754b4-1562">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="754b4-1562">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="754b4-1563">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="754b4-1563">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="754b4-1564">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="754b4-1564">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="754b4-1565">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="754b4-1565">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="754b4-1566">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="754b4-1566">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="754b4-1567">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="754b4-1567">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="754b4-1568">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="754b4-1568">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="754b4-1569">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="754b4-1569">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="754b4-1570">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-1570">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="754b4-1571">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="754b4-1571">Highlights since the last major release</span></span>
* <span data-ttu-id="754b4-1572">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="754b4-1572">General availability of `Az` module</span></span>
* <span data-ttu-id="754b4-1573">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="754b4-1573">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="754b4-1574">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="754b4-1574">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="754b4-1575">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1575">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="754b4-1576">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="754b4-1576">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="754b4-1577">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="754b4-1577">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="754b4-1578">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="754b4-1578">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="754b4-1579">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="754b4-1579">Az.Automation</span></span>
* <span data-ttu-id="754b4-1580">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="754b4-1580">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="754b4-1581">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="754b4-1581">Dynamic grouping</span></span>
    * <span data-ttu-id="754b4-1582">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="754b4-1582">Pre-Post script</span></span>
    * <span data-ttu-id="754b4-1583">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="754b4-1583">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-1584">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-1584">Az.Compute</span></span>
* <span data-ttu-id="754b4-1585">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="754b4-1585">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="754b4-1586">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="754b4-1586">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="754b4-1587">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="754b4-1587">Az.KeyVault</span></span>
* <span data-ttu-id="754b4-1588">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="754b4-1588">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-1589">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1589">Az.Network</span></span>
* <span data-ttu-id="754b4-1590">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="754b4-1590">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="754b4-1591">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="754b4-1591">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-1592">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1592">Az.RecoveryServices</span></span>
* <span data-ttu-id="754b4-1593">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="754b4-1593">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="754b4-1594">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="754b4-1594">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-1595">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-1595">Az.Resources</span></span>
* <span data-ttu-id="754b4-1596">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="754b4-1596">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="754b4-1597">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="754b4-1597">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-1598">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1598">Az.Sql</span></span>
* <span data-ttu-id="754b4-1599">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="754b4-1599">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-1600">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-1600">Az.Storage</span></span>
* <span data-ttu-id="754b4-1601">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="754b4-1601">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="754b4-1602">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="754b4-1602">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="754b4-1603">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="754b4-1603">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="754b4-1604">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="754b4-1604">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="754b4-1605">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="754b4-1605">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="754b4-1606">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="754b4-1606">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="754b4-1607">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="754b4-1607">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="754b4-1608">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-1608">Az.Websites</span></span>
* <span data-ttu-id="754b4-1609">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="754b4-1609">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="754b4-1610">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-1610">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="754b4-1611">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-1611">Az.Accounts</span></span>
* <span data-ttu-id="754b4-1612">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="754b4-1612">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="754b4-1613">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-1613">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="754b4-1614">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="754b4-1614">Az.Automation</span></span>
* <span data-ttu-id="754b4-1615">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="754b4-1615">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="754b4-1616">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="754b4-1616">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="754b4-1617">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="754b4-1617">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="754b4-1618">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="754b4-1618">Az.Cdn</span></span>
* <span data-ttu-id="754b4-1619">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="754b4-1619">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-1620">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-1620">Az.Compute</span></span>
* <span data-ttu-id="754b4-1621">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="754b4-1621">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="754b4-1622">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="754b4-1622">Az.DataFactory</span></span>
* <span data-ttu-id="754b4-1623">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="754b4-1623">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="754b4-1624">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="754b4-1624">Az.LogicApp</span></span>
* <span data-ttu-id="754b4-1625">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="754b4-1625">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-1626">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1626">Az.Network</span></span>
* <span data-ttu-id="754b4-1627">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1627">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-1628">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1628">Az.RecoveryServices</span></span>
* <span data-ttu-id="754b4-1629">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="754b4-1629">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="754b4-1630">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="754b4-1630">SDK Update</span></span>
* <span data-ttu-id="754b4-1631">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="754b4-1631">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="754b4-1632">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="754b4-1632">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-1633">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-1633">Az.Resources</span></span>
* <span data-ttu-id="754b4-1634">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="754b4-1634">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="754b4-1635">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="754b4-1635">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="754b4-1636">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="754b4-1636">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="754b4-1637">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="754b4-1637">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="754b4-1638">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="754b4-1638">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="754b4-1639">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="754b4-1639">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-1640">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1640">Az.Sql</span></span>
* <span data-ttu-id="754b4-1641">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="754b4-1641">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="754b4-1642">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="754b4-1642">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-1643">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-1643">Az.Storage</span></span>
* <span data-ttu-id="754b4-1644">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-1644">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="754b4-1645">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-1645">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="754b4-1646">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1646">Az.AnalysisServices</span></span>
* <span data-ttu-id="754b4-1647">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="754b4-1647">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="754b4-1648">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="754b4-1648">Az.Automation</span></span>
* <span data-ttu-id="754b4-1649">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="754b4-1649">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="754b4-1650">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="754b4-1650">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="754b4-1651">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="754b4-1651">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="754b4-1652">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1652">Az.CognitiveServices</span></span>
* <span data-ttu-id="754b4-1653">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="754b4-1653">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-1654">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-1654">Az.Compute</span></span>
* <span data-ttu-id="754b4-1655">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="754b4-1655">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="754b4-1656">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="754b4-1656">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="754b4-1657">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="754b4-1657">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="754b4-1658">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="754b4-1658">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="754b4-1659">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="754b4-1659">Az.DataLakeStore</span></span>
* <span data-ttu-id="754b4-1660">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="754b4-1660">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="754b4-1661">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="754b4-1661">Az.EventHub</span></span>
* <span data-ttu-id="754b4-1662">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="754b4-1662">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="754b4-1663">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="754b4-1663">Az.KeyVault</span></span>
* <span data-ttu-id="754b4-1664">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="754b4-1664">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="754b4-1665">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="754b4-1665">Az.LogicApp</span></span>
* <span data-ttu-id="754b4-1666">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="754b4-1666">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="754b4-1667">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="754b4-1667">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="754b4-1668">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="754b4-1668">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="754b4-1669">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="754b4-1669">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="754b4-1670">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="754b4-1670">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="754b4-1671">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="754b4-1671">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="754b4-1672">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="754b4-1672">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="754b4-1673">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="754b4-1673">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="754b4-1674">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="754b4-1674">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="754b4-1675">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="754b4-1675">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="754b4-1676">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="754b4-1676">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="754b4-1677">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="754b4-1677">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="754b4-1678">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="754b4-1678">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="754b4-1679">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="754b4-1679">Az.Monitor</span></span>
* <span data-ttu-id="754b4-1680">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="754b4-1680">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-1681">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1681">Az.Network</span></span>
* <span data-ttu-id="754b4-1682">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="754b4-1682">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="754b4-1683">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="754b4-1683">Az.OperationalInsights</span></span>
* <span data-ttu-id="754b4-1684">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="754b4-1684">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="754b4-1685">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="754b4-1685">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="754b4-1686">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="754b4-1686">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-1687">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-1687">Az.Resources</span></span>
* <span data-ttu-id="754b4-1688">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="754b4-1688">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="754b4-1689">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="754b4-1689">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="754b4-1690">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="754b4-1690">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="754b4-1691">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="754b4-1691">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-1692">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1692">Az.Sql</span></span>
* <span data-ttu-id="754b4-1693">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="754b4-1693">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="754b4-1694">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="754b4-1694">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="754b4-1695">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-1695">Az.Websites</span></span>
* <span data-ttu-id="754b4-1696">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="754b4-1696">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="754b4-1697">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-1697">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="754b4-1698">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-1698">Az.Accounts</span></span>
* <span data-ttu-id="754b4-1699">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="754b4-1699">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="754b4-1700">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1700">Az.AnalysisServices</span></span>
<span data-ttu-id="754b4-1701">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="754b4-1701">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-1702">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-1702">Az.Compute</span></span>
* <span data-ttu-id="754b4-1703">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="754b4-1703">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="754b4-1704">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="754b4-1704">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="754b4-1705">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="754b4-1705">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-1706">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1706">Az.RecoveryServices</span></span>
<span data-ttu-id="754b4-1707">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="754b4-1707">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-1708">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-1708">Az.Resources</span></span>
* <span data-ttu-id="754b4-1709">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="754b4-1709">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="754b4-1710">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="754b4-1710">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="754b4-1711">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="754b4-1711">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="754b4-1712">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="754b4-1712">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-1713">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1713">Az.Sql</span></span>
* <span data-ttu-id="754b4-1714">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="754b4-1714">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="754b4-1715">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="754b4-1715">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="754b4-1716">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="754b4-1716">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="754b4-1717">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-1717">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="754b4-1718">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-1718">Az.Accounts</span></span>
* <span data-ttu-id="754b4-1719">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="754b4-1719">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="754b4-1720">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1720">Az.AnalysisServices</span></span>
* <span data-ttu-id="754b4-1721">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="754b4-1721">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-1722">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1722">Az.RecoveryServices</span></span>
* <span data-ttu-id="754b4-1723">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="754b4-1723">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="754b4-1724">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-1724">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="754b4-1725">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-1725">Az.Accounts</span></span>
* <span data-ttu-id="754b4-1726">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="754b4-1726">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="754b4-1727">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="754b4-1727">Update incorrect online help URLs</span></span>
* <span data-ttu-id="754b4-1728">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="754b4-1728">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="754b4-1729">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="754b4-1729">Az.Aks</span></span>
* <span data-ttu-id="754b4-1730">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="754b4-1730">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="754b4-1731">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="754b4-1731">Az.Automation</span></span>
* <span data-ttu-id="754b4-1732">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="754b4-1732">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="754b4-1733">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="754b4-1733">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="754b4-1734">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="754b4-1734">Az.Cdn</span></span>
* <span data-ttu-id="754b4-1735">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="754b4-1735">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-1736">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-1736">Az.Compute</span></span>
* <span data-ttu-id="754b4-1737">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="754b4-1737">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="754b4-1738">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="754b4-1738">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="754b4-1739">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="754b4-1739">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="754b4-1740">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="754b4-1740">Az.ContainerRegistry</span></span>
* <span data-ttu-id="754b4-1741">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="754b4-1741">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="754b4-1742">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="754b4-1742">Az.DataFactory</span></span>
* <span data-ttu-id="754b4-1743">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="754b4-1743">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="754b4-1744">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="754b4-1744">Az.DataLakeStore</span></span>
* <span data-ttu-id="754b4-1745">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="754b4-1745">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="754b4-1746">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="754b4-1746">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="754b4-1747">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="754b4-1747">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="754b4-1748">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="754b4-1748">Az.IotHub</span></span>
* <span data-ttu-id="754b4-1749">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="754b4-1749">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="754b4-1750">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="754b4-1750">Az.KeyVault</span></span>
* <span data-ttu-id="754b4-1751">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="754b4-1751">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-1752">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1752">Az.Network</span></span>
* <span data-ttu-id="754b4-1753">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="754b4-1753">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-1754">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-1754">Az.Resources</span></span>
* <span data-ttu-id="754b4-1755">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="754b4-1755">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="754b4-1756">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="754b4-1756">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="754b4-1757">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="754b4-1757">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="754b4-1758">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="754b4-1758">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="754b4-1759">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="754b4-1759">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="754b4-1760">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="754b4-1760">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="754b4-1761">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="754b4-1761">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="754b4-1762">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="754b4-1762">Az.ServiceFabric</span></span>
* <span data-ttu-id="754b4-1763">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="754b4-1763">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="754b4-1764">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="754b4-1764">Fix some error messages.</span></span>
* <span data-ttu-id="754b4-1765">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="754b4-1765">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="754b4-1766">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="754b4-1766">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="754b4-1767">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="754b4-1767">Az.SignalR</span></span>
* <span data-ttu-id="754b4-1768">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="754b4-1768">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-1769">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1769">Az.Sql</span></span>
* <span data-ttu-id="754b4-1770">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="754b4-1770">Update incorrect online help URLs</span></span>
* <span data-ttu-id="754b4-1771">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="754b4-1771">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="754b4-1772">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="754b4-1772">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="754b4-1773">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="754b4-1773">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-1774">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-1774">Az.Storage</span></span>
* <span data-ttu-id="754b4-1775">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="754b4-1775">Update incorrect online help URLs</span></span>
* <span data-ttu-id="754b4-1776">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="754b4-1776">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="754b4-1777">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="754b4-1777">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="754b4-1778">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="754b4-1778">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="754b4-1779">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="754b4-1779">Az.TrafficManager</span></span>
* <span data-ttu-id="754b4-1780">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="754b4-1780">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="754b4-1781">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-1781">Az.Websites</span></span>
* <span data-ttu-id="754b4-1782">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="754b4-1782">Update incorrect online help URLs</span></span>
* <span data-ttu-id="754b4-1783">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="754b4-1783">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="754b4-1784">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="754b4-1784">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="754b4-1785">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="754b4-1785">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="754b4-1786">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-1786">Az.Accounts</span></span>
* <span data-ttu-id="754b4-1787">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="754b4-1787">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-1788">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-1788">Az.Compute</span></span>
* <span data-ttu-id="754b4-1789">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="754b4-1789">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="754b4-1790">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="754b4-1790">Updated the description of ID in help files</span></span>
* <span data-ttu-id="754b4-1791">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-1791">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="754b4-1792">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="754b4-1792">Az.DataLakeStore</span></span>
* <span data-ttu-id="754b4-1793">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="754b4-1793">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="754b4-1794">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="754b4-1794">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="754b4-1795">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="754b4-1795">Az.EventGrid</span></span>
* <span data-ttu-id="754b4-1796">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="754b4-1796">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="754b4-1797">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="754b4-1797">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="754b4-1798">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="754b4-1798">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="754b4-1799">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="754b4-1799">Event Time-To-Live,</span></span>
        - <span data-ttu-id="754b4-1800">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="754b4-1800">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="754b4-1801">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="754b4-1801">Dead letter endpoint.</span></span>
    - <span data-ttu-id="754b4-1802">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="754b4-1802">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="754b4-1803">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="754b4-1803">Event Time-To-Live,</span></span>
        - <span data-ttu-id="754b4-1804">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="754b4-1804">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="754b4-1805">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="754b4-1805">Dead letter endpoint.</span></span>
* <span data-ttu-id="754b4-1806">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="754b4-1806">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="754b4-1807">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="754b4-1807">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="754b4-1808">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="754b4-1808">Az.IotHub</span></span>
* <span data-ttu-id="754b4-1809">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="754b4-1809">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="754b4-1810">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="754b4-1810">Az.LogicApp</span></span>
* <span data-ttu-id="754b4-1811">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="754b4-1811">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-1812">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-1812">Az.Resources</span></span>
* <span data-ttu-id="754b4-1813">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="754b4-1813">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="754b4-1814">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="754b4-1814">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="754b4-1815">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="754b4-1815">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="754b4-1816">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="754b4-1816">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="754b4-1817">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="754b4-1817">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="754b4-1818">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="754b4-1818">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="754b4-1819">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="754b4-1819">Az.SignalR</span></span>
* <span data-ttu-id="754b4-1820">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-1820">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-1821">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1821">Az.Sql</span></span>
* <span data-ttu-id="754b4-1822">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="754b4-1822">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="754b4-1823">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-1823">Az.Storage</span></span>
* <span data-ttu-id="754b4-1824">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="754b4-1824">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="754b4-1825">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="754b4-1825">New-AzStorageContext</span></span>
* <span data-ttu-id="754b4-1826">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="754b4-1826">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="754b4-1827">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="754b4-1827">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="754b4-1828">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-1828">Az.Websites</span></span>
* <span data-ttu-id="754b4-1829">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="754b4-1829">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="754b4-1830">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-1830">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="754b4-1831">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="754b4-1831">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="754b4-1832">Geral</span><span class="sxs-lookup"><span data-stu-id="754b4-1832">General</span></span>

- <span data-ttu-id="754b4-1833">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="754b4-1833">General Availability of Az Module</span></span>
- <span data-ttu-id="754b4-1834">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="754b4-1834">Online help for each module</span></span>
- <span data-ttu-id="754b4-1835">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="754b4-1835">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="754b4-1836">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="754b4-1836">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="754b4-1837">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-1837">Az.Accounts</span></span>
- <span data-ttu-id="754b4-1838">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="754b4-1838">Changed from Az.Profile</span></span>
- <span data-ttu-id="754b4-1839">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="754b4-1839">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="754b4-1840">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="754b4-1840">Az.ApiManagement</span></span>
- <span data-ttu-id="754b4-1841">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="754b4-1841">Fixes for #7002</span></span>
- <span data-ttu-id="754b4-1842">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="754b4-1842">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="754b4-1843">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="754b4-1843">Az.Batch</span></span>
- <span data-ttu-id="754b4-1844">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="754b4-1844">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="754b4-1845">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="754b4-1845">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="754b4-1846">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="754b4-1846">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="754b4-1847">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="754b4-1847">Az.Billing</span></span>
- <span data-ttu-id="754b4-1848">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="754b4-1848">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="754b4-1849">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1849">Az.CognitivServices</span></span>
- <span data-ttu-id="754b4-1850">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-1850">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="754b4-1851">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="754b4-1851">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="754b4-1852">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="754b4-1852">Az.ContainerInstance</span></span>
- <span data-ttu-id="754b4-1853">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="754b4-1853">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="754b4-1854">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="754b4-1854">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="754b4-1855">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="754b4-1855">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="754b4-1856">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="754b4-1856">Az.DataLakeStore</span></span>
- <span data-ttu-id="754b4-1857">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="754b4-1857">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="754b4-1858">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="754b4-1858">Az.Monitor</span></span>
- <span data-ttu-id="754b4-1859">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="754b4-1859">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="754b4-1860">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="754b4-1860">Az.KeyVault</span></span>
- <span data-ttu-id="754b4-1861">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="754b4-1861">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="754b4-1862">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="754b4-1862">Az.MachineLearning</span></span>
- <span data-ttu-id="754b4-1863">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="754b4-1863">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="754b4-1864">Az.Media</span><span class="sxs-lookup"><span data-stu-id="754b4-1864">Az.Media</span></span>
- <span data-ttu-id="754b4-1865">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="754b4-1865">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="754b4-1866">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1866">Az.Network</span></span>
<span data-ttu-id="754b4-1867">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="754b4-1867">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="754b4-1868">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="754b4-1868">New cmdlets added:</span></span>
        - <span data-ttu-id="754b4-1869">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="754b4-1869">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="754b4-1870">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="754b4-1870">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="754b4-1871">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="754b4-1871">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="754b4-1872">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="754b4-1872">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="754b4-1873">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="754b4-1873">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="754b4-1874">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="754b4-1874">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="754b4-1875">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="754b4-1875">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="754b4-1876">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="754b4-1876">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="754b4-1877">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="754b4-1877">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="754b4-1878">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="754b4-1878">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="754b4-1879">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="754b4-1879">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="754b4-1880">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="754b4-1880">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="754b4-1881">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-1881">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="754b4-1882">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-1882">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="754b4-1883">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="754b4-1883">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="754b4-1884">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="754b4-1884">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="754b4-1885">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="754b4-1885">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="754b4-1886">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="754b4-1886">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="754b4-1887">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="754b4-1887">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="754b4-1888">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="754b4-1888">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="754b4-1889">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="754b4-1889">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="754b4-1890">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="754b4-1890">Az.OperationalInsights</span></span>
- <span data-ttu-id="754b4-1891">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="754b4-1891">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="754b4-1892">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="754b4-1892">Az.Profile</span></span>
- <span data-ttu-id="754b4-1893">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="754b4-1893">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-1894">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1894">Az.RecoveryServices</span></span>
- <span data-ttu-id="754b4-1895">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="754b4-1895">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="754b4-1896">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-1896">Az.Resources</span></span>
- <span data-ttu-id="754b4-1897">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="754b4-1897">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="754b4-1898">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="754b4-1898">Az.ServiceFabric</span></span>
- <span data-ttu-id="754b4-1899">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="754b4-1899">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="754b4-1900">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="754b4-1900">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="754b4-1901">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="754b4-1901">Az.SIgnalR</span></span>
- <span data-ttu-id="754b4-1902">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="754b4-1902">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="754b4-1903">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1903">Az.Sql</span></span>
- <span data-ttu-id="754b4-1904">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="754b4-1904">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="754b4-1905">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="754b4-1905">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="754b4-1906">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="754b4-1906">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="754b4-1907">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-1907">Az.Storage</span></span>
- <span data-ttu-id="754b4-1908">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="754b4-1908">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="754b4-1909">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-1909">Az.Websites</span></span>
- <span data-ttu-id="754b4-1910">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="754b4-1910">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="754b4-1911">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="754b4-1911">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="754b4-1912">Geral</span><span class="sxs-lookup"><span data-stu-id="754b4-1912">General</span></span>

* <span data-ttu-id="754b4-1913">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="754b4-1913">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="754b4-1914">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-1914">Az.Compute</span></span>

* <span data-ttu-id="754b4-1915">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="754b4-1915">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="754b4-1916">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="754b4-1916">Az.DataLakeStore</span></span>

* <span data-ttu-id="754b4-1917">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="754b4-1917">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="754b4-1918">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="754b4-1918">Az.FrontDoor</span></span>

* <span data-ttu-id="754b4-1919">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="754b4-1919">Fixed some broken links</span></span>
    - <span data-ttu-id="754b4-1920">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="754b4-1920">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="754b4-1921">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="754b4-1921">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="754b4-1922">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="754b4-1922">Az.RecoveryServices</span></span>

* <span data-ttu-id="754b4-1923">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-1923">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="754b4-1924">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="754b4-1924">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="754b4-1925">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-1925">Az.Resources</span></span>

* <span data-ttu-id="754b4-1926">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="754b4-1926">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="754b4-1927">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="754b4-1927">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="754b4-1928">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1928">Az.Sql</span></span>

* <span data-ttu-id="754b4-1929">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="754b4-1929">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="754b4-1930">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="754b4-1930">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="754b4-1931">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="754b4-1931">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="754b4-1932">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-1932">Az.Storage</span></span>

* <span data-ttu-id="754b4-1933">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="754b4-1933">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="754b4-1934">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="754b4-1934">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="754b4-1935">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="754b4-1935">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="754b4-1936">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="754b4-1936">Support Static Website configuration</span></span>
    - <span data-ttu-id="754b4-1937">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="754b4-1937">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="754b4-1938">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="754b4-1938">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="754b4-1939">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-1939">Az.Websites</span></span>

* <span data-ttu-id="754b4-1940">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="754b4-1940">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="754b4-1941">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="754b4-1941">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="754b4-1942">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-1942">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="754b4-1943">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="754b4-1943">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="754b4-1944">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="754b4-1944">Az.ApiManagement</span></span>
* <span data-ttu-id="754b4-1945">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="754b4-1945">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="754b4-1946">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="754b4-1946">Az.Automation</span></span>
* <span data-ttu-id="754b4-1947">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="754b4-1947">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="754b4-1948">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="754b4-1948">Added Update Management cmdlets</span></span>
* <span data-ttu-id="754b4-1949">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="754b4-1949">Added Source Control cmdlets</span></span>
* <span data-ttu-id="754b4-1950">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="754b4-1950">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="754b4-1951">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="754b4-1951">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="754b4-1952">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-1952">Az.Compute</span></span>
* <span data-ttu-id="754b4-1953">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="754b4-1953">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="754b4-1954">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="754b4-1954">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="754b4-1955">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="754b4-1955">Az.ContainerInstance</span></span>
* <span data-ttu-id="754b4-1956">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="754b4-1956">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="754b4-1957">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="754b4-1957">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="754b4-1958">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="754b4-1958">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="754b4-1959">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-1959">Az.Network</span></span>
* <span data-ttu-id="754b4-1960">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="754b4-1960">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="754b4-1961">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="754b4-1961">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="754b4-1962">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="754b4-1962">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="754b4-1963">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="754b4-1963">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="754b4-1964">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="754b4-1964">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="754b4-1965">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="754b4-1965">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="754b4-1966">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="754b4-1966">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="754b4-1967">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="754b4-1967">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="754b4-1968">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="754b4-1968">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="754b4-1969">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="754b4-1969">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="754b4-1970">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="754b4-1970">Az.Relay</span></span>
* <span data-ttu-id="754b4-1971">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="754b4-1971">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="754b4-1972">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-1972">Az.Resources</span></span>
* <span data-ttu-id="754b4-1973">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="754b4-1973">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="754b4-1974">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="754b4-1974">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="754b4-1975">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="754b4-1975">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="754b4-1976">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="754b4-1976">Az.ServiceFabric</span></span>
* <span data-ttu-id="754b4-1977">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="754b4-1977">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="754b4-1978">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-1978">Az.Sql</span></span>
* <span data-ttu-id="754b4-1979">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="754b4-1979">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="754b4-1980">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="754b4-1980">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="754b4-1981">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="754b4-1981">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="754b4-1982">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="754b4-1982">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="754b4-1983">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="754b4-1983">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="754b4-1984">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="754b4-1984">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="754b4-1985">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="754b4-1985">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="754b4-1986">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="754b4-1986">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="754b4-1987">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="754b4-1987">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="754b4-1988">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="754b4-1988">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="754b4-1989">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="754b4-1989">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="754b4-1990">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="754b4-1990">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="754b4-1991">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="754b4-1991">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="754b4-1992">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="754b4-1992">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="754b4-1993">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="754b4-1993">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="754b4-1994">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="754b4-1994">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="754b4-1995">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="754b4-1995">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="754b4-1996">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="754b4-1996">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="754b4-1997">Geral</span><span class="sxs-lookup"><span data-stu-id="754b4-1997">General</span></span>
* <span data-ttu-id="754b4-1998">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="754b4-1998">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="754b4-1999">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="754b4-1999">Az.Profile</span></span>
* <span data-ttu-id="754b4-2000">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="754b4-2000">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="754b4-2001">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="754b4-2001">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="754b4-2002">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="754b4-2002">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="754b4-2003">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="754b4-2003">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="754b4-2004">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="754b4-2004">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="754b4-2005">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="754b4-2005">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="754b4-2006">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="754b4-2006">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="754b4-2007">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="754b4-2007">Az.CognitiveServices</span></span>
* <span data-ttu-id="754b4-2008">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="754b4-2008">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-2009">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-2009">Az.Compute</span></span>
* <span data-ttu-id="754b4-2010">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="754b4-2010">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="754b4-2011">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="754b4-2011">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="754b4-2012">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="754b4-2012">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="754b4-2013">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="754b4-2013">Az.DataLakeStore</span></span>
* <span data-ttu-id="754b4-2014">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="754b4-2014">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="754b4-2015">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="754b4-2015">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="754b4-2016">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="754b4-2016">Az.Insights</span></span>
* <span data-ttu-id="754b4-2017">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="754b4-2017">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="754b4-2018">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="754b4-2018">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="754b4-2019">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="754b4-2019">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="754b4-2020">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="754b4-2020">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-2021">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-2021">Az.Network</span></span>
* <span data-ttu-id="754b4-2022">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="754b4-2022">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="754b4-2023">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="754b4-2023">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="754b4-2024">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="754b4-2024">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="754b4-2025">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="754b4-2025">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="754b4-2026">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="754b4-2026">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="754b4-2027">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="754b4-2027">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="754b4-2028">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="754b4-2028">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="754b4-2029">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="754b4-2029">Az.PolicyInsights</span></span>
* <span data-ttu-id="754b4-2030">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="754b4-2030">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-2031">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-2031">Az.Resources</span></span>
* <span data-ttu-id="754b4-2032">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="754b4-2032">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="754b4-2033">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="754b4-2033">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="754b4-2034">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="754b4-2034">Az.ServiceBus</span></span>
* <span data-ttu-id="754b4-2035">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="754b4-2035">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="754b4-2036">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="754b4-2036">Az.ServiceFabric</span></span>
* <span data-ttu-id="754b4-2037">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="754b4-2037">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="754b4-2038">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="754b4-2038">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="754b4-2039">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="754b4-2039">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="754b4-2040">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="754b4-2040">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="754b4-2041">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="754b4-2041">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="754b4-2042">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="754b4-2042">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="754b4-2043">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="754b4-2043">Az.Profile</span></span>
* <span data-ttu-id="754b4-2044">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="754b4-2044">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="754b4-2045">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="754b4-2045">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-2046">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-2046">Az.Compute</span></span>
* <span data-ttu-id="754b4-2047">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="754b4-2047">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="754b4-2048">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="754b4-2048">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="754b4-2049">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="754b4-2049">Az.DataLakeStore</span></span>
* <span data-ttu-id="754b4-2050">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="754b4-2050">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="754b4-2051">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-2051">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="754b4-2052">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="754b4-2052">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="754b4-2053">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="754b4-2053">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="754b4-2054">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="754b4-2054">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-2055">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-2055">Az.Network</span></span>
* <span data-ttu-id="754b4-2056">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="754b4-2056">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="754b4-2057">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="754b4-2057">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-2058">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-2058">Az.Resources</span></span>
* <span data-ttu-id="754b4-2059">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="754b4-2059">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="754b4-2060">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="754b4-2060">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="754b4-2061">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="754b4-2061">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="754b4-2062">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="754b4-2062">Azure.Storage</span></span>
* <span data-ttu-id="754b4-2063">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="754b4-2063">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="754b4-2064">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="754b4-2064">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="754b4-2065">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="754b4-2065">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="754b4-2066">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="754b4-2066">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="754b4-2067">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="754b4-2067">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="754b4-2068">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="754b4-2068">Az.CognitiveServices</span></span>
* <span data-ttu-id="754b4-2069">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="754b4-2069">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="754b4-2070">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="754b4-2070">Az.Compute</span></span>
* <span data-ttu-id="754b4-2071">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="754b4-2071">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="754b4-2072">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="754b4-2072">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="754b4-2073">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="754b4-2073">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="754b4-2074">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="754b4-2074">Az.DataFactoryV2</span></span>
* <span data-ttu-id="754b4-2075">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="754b4-2075">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="754b4-2076">Az.Network</span><span class="sxs-lookup"><span data-stu-id="754b4-2076">Az.Network</span></span>
* <span data-ttu-id="754b4-2077">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="754b4-2077">Added NetworkProfile functionality.</span></span> <span data-ttu-id="754b4-2078">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="754b4-2078">new cmdlets added</span></span>
    - <span data-ttu-id="754b4-2079">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="754b4-2079">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="754b4-2080">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="754b4-2080">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="754b4-2081">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="754b4-2081">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="754b4-2082">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="754b4-2082">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="754b4-2083">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-2083">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="754b4-2084">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-2084">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="754b4-2085">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="754b4-2085">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="754b4-2086">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="754b4-2086">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="754b4-2087">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="754b4-2087">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="754b4-2088">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="754b4-2088">Az.RedisCache</span></span>
* <span data-ttu-id="754b4-2089">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="754b4-2089">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="754b4-2090">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="754b4-2090">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="754b4-2091">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="754b4-2091">Az.Resources</span></span>
* <span data-ttu-id="754b4-2092">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="754b4-2092">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="754b4-2093">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="754b4-2093">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="754b4-2094">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="754b4-2094">Az.Sql</span></span>
* <span data-ttu-id="754b4-2095">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="754b4-2095">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="754b4-2096">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="754b4-2096">Az.Websites</span></span>
* <span data-ttu-id="754b4-2097">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="754b4-2097">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="754b4-2098">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="754b4-2098">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="754b4-2099">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="754b4-2099">0.2.0 - September 2018</span></span>
 <span data-ttu-id="754b4-2100">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="754b4-2100">Initial Release</span></span>
