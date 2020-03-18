---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/09/2020
ms.openlocfilehash: 4c7ea19a225d63307ecf4a6fe5ebfa14ccd78d7e
ms.sourcegitcommit: f6fa6543be1e0f6330b1598f01528b2928cc426c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2020
ms.locfileid: "79036166"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="7f563-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="7f563-103">Azure PowerShell release notes</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="7f563-104">3.6.1 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="7f563-104">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="7f563-105">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-105">Az.Accounts</span></span>
* <span data-ttu-id="7f563-106">Abrir a página de inquérito do Azure PowerShell em "Send-Feedback" [#11020]</span><span class="sxs-lookup"><span data-stu-id="7f563-106">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="7f563-107">Apresentar o URL de inquérito do Azure PowerShell em "Resolve-Error" [#11021]</span><span class="sxs-lookup"><span data-stu-id="7f563-107">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="7f563-108">Adicionada versão de Az em UserAgent</span><span class="sxs-lookup"><span data-stu-id="7f563-108">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="7f563-109">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7f563-109">Az.ApiManagement</span></span>
* <span data-ttu-id="7f563-110">Adicionado suporte para a obtenção e configuração do Domínio Personalizado no Ponto Final do DeveloperPortal [#11007]</span><span class="sxs-lookup"><span data-stu-id="7f563-110">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="7f563-111">"Export-AzApiManagementApi" Adicionado suporte para a transferência da definição da API no formato JSON [#9987]</span><span class="sxs-lookup"><span data-stu-id="7f563-111">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="7f563-112">"Import-AzApiManagementApi" Adicionado suporte para a importação da definição de OpenApi 3.0 a partir de documento JSON</span><span class="sxs-lookup"><span data-stu-id="7f563-112">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="7f563-113">"New-AzApiManagementIdentityProvider" e "Set-AzApiManagementIdentityProvider" Adicionado suporte para a configuração de "Inquilino de Início de Sessão" para Fornecedor de AAD B2C [#9784]</span><span class="sxs-lookup"><span data-stu-id="7f563-113">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="7f563-114">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f563-114">Az.DataLakeStore</span></span>
* <span data-ttu-id="7f563-115">Adicionada referência a System.Buffers explicitamente em csproj e psd1.</span><span class="sxs-lookup"><span data-stu-id="7f563-115">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="7f563-116">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="7f563-116">Az.IotHub</span></span>
* <span data-ttu-id="7f563-117">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="7f563-117">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="7f563-118">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="7f563-118">New Cmdlets are:</span></span>
    - <span data-ttu-id="7f563-119">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="7f563-119">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="7f563-120">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="7f563-120">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="7f563-121">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="7f563-121">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="7f563-122">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="7f563-122">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="7f563-123">Adicionado suporte para a gestão de módulos num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="7f563-123">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="7f563-124">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="7f563-124">New Cmdlets are:</span></span>
    - <span data-ttu-id="7f563-125">"Add-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="7f563-125">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="7f563-126">"Get-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="7f563-126">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="7f563-127">"Remove-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="7f563-127">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="7f563-128">"Set-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="7f563-128">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="7f563-129">Adicionado cmdlet para obter a cadeia de ligação de um dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="7f563-129">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="7f563-130">Adicionado cmdlet para obter a cadeia de ligação de um módulo num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="7f563-130">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="7f563-131">Adicionado suporte para obter/definir dispositivo principal de um dispositivo IoT.</span><span class="sxs-lookup"><span data-stu-id="7f563-131">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="7f563-132">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="7f563-132">New Cmdlets are:</span></span>
    - <span data-ttu-id="7f563-133">"Get-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="7f563-133">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="7f563-134">"Set-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="7f563-134">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="7f563-135">Adicionado suporte para gerir relações principal-subordinado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7f563-135">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="7f563-136">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="7f563-136">Az.Monitor</span></span>
* <span data-ttu-id="7f563-137">Corrigido o valor de saída de "Get-AzMetricDefinition" [#9714]</span><span class="sxs-lookup"><span data-stu-id="7f563-137">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-138">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-138">Az.Network</span></span>
* <span data-ttu-id="7f563-139">Sdk Sql Management atualizado.</span><span class="sxs-lookup"><span data-stu-id="7f563-139">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="7f563-140">Corrigido um problema de diferença de nomes na classe PrivateLinkServiceConnectionState.</span><span class="sxs-lookup"><span data-stu-id="7f563-140">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="7f563-141">Mapeamento do campo ActionsRequired para ActionRequired.</span><span class="sxs-lookup"><span data-stu-id="7f563-141">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="7f563-142">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="7f563-142">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-143">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-143">Az.Resources</span></span>
* <span data-ttu-id="7f563-144">Correção para erro de referência nula em "Get-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="7f563-144">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="7f563-145">Comutadores "-Force" e "-PassThru" marcados como opcionais em "Remove-AzADGroup" [#10849]</span><span class="sxs-lookup"><span data-stu-id="7f563-145">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="7f563-146">Corrigido problema em que "MailNickname" não devolve "Remove-AzADGroup" [#11167]</span><span class="sxs-lookup"><span data-stu-id="7f563-146">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="7f563-147">Corrigido problema em que a operação de pipe "Remove-AzADGroup" não funciona [#11171]</span><span class="sxs-lookup"><span data-stu-id="7f563-147">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="7f563-148">Correção para erro de referência nula em GetAzureRoleAssignmentCommand</span><span class="sxs-lookup"><span data-stu-id="7f563-148">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="7f563-149">Adicionados atributos de alterações interruptivas para futuras alterações a cmdlets de política</span><span class="sxs-lookup"><span data-stu-id="7f563-149">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="7f563-150">"Get-AzResourceGroup" atualizado para realizar filtragem de etiqueta de grupo de recursos no lado do servidor</span><span class="sxs-lookup"><span data-stu-id="7f563-150">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="7f563-151">Cmdlets Tag alargados para accept -ResourceId</span><span class="sxs-lookup"><span data-stu-id="7f563-151">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="7f563-152">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="7f563-152">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="7f563-153">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="7f563-153">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="7f563-154">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="7f563-154">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="7f563-155">Adicionado cmdlet Tag novo</span><span class="sxs-lookup"><span data-stu-id="7f563-155">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="7f563-156">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="7f563-156">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="7f563-157">ScopedDeployment trazido de SDK 3.3.0</span><span class="sxs-lookup"><span data-stu-id="7f563-157">Brought ScopedDeployment from SDK 3.3.0</span></span> 

#### <a name="azsql"></a><span data-ttu-id="7f563-158">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-158">Az.Sql</span></span>
* <span data-ttu-id="7f563-159">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="7f563-159">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="7f563-160">Adicionado suporte para configuração de cópia de segurança de Retenção de Longo Prazo para Bases de Dados Geridas</span><span class="sxs-lookup"><span data-stu-id="7f563-160">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="7f563-161">Política Get/Set numa base de dados gerida</span><span class="sxs-lookup"><span data-stu-id="7f563-161">Get/Set LTR policy on a managed database</span></span> 
    - <span data-ttu-id="7f563-162">Obter cópia(s) de segurança LTR por base de dados gerida, por instância gerida ou por localização</span><span class="sxs-lookup"><span data-stu-id="7f563-162">Get LTR backup(s) by managed database, managed instance, or by location</span></span> 
    - <span data-ttu-id="7f563-163">Remover uma cópia de segurança LTR</span><span class="sxs-lookup"><span data-stu-id="7f563-163">Remove an LTR backup</span></span> 
    - <span data-ttu-id="7f563-164">Restaurar uma cópia de segurança LTR para criar uma base de dados gerida nova</span><span class="sxs-lookup"><span data-stu-id="7f563-164">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="7f563-165">Adicionado MinimalTlsVersion a New-AzSqlServer e Set-AzSqlServer</span><span class="sxs-lookup"><span data-stu-id="7f563-165">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="7f563-166">Adicionado MinimalTlsVersion a New-AzSqlInstance e Set-AzSqlInstance</span><span class="sxs-lookup"><span data-stu-id="7f563-166">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="7f563-167">Versão de SDK SQL atualizada para Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-167">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-168">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-168">Az.Storage</span></span>
* <span data-ttu-id="7f563-169">AllowProtectedAppendWrite suportada em ImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="7f563-169">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="7f563-170">"Set-AzRmStorageContainerImmutabilityPolicy"</span><span class="sxs-lookup"><span data-stu-id="7f563-170">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="7f563-171">Adicionada uma mensagem de aviso de alteração interruptiva para alteração do tipo AzureStorageTable numa futura versão</span><span class="sxs-lookup"><span data-stu-id="7f563-171">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="7f563-172">"New-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="7f563-172">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="7f563-173">"Get-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="7f563-173">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f563-174">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-174">Az.Websites</span></span>
* <span data-ttu-id="7f563-175">Adicionado o parâmetro Tag para "New-AzAppServicePlan" e "Set-AzAppServicePlan"</span><span class="sxs-lookup"><span data-stu-id="7f563-175">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="7f563-176">Paragem da execução de cmdlet caso seja emitida uma exceção ao adicionar um domínio personalizado a um site</span><span class="sxs-lookup"><span data-stu-id="7f563-176">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="7f563-177">Adicionado suporte para a realização de operações para Serviços de Aplicações em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="7f563-177">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="7f563-178">Aplicada restrição de acesso a WebApp/Função em diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="7f563-178">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="7f563-179">Corrigido problema para definir os nomes de anfitrião personalizados para WebAppSlots</span><span class="sxs-lookup"><span data-stu-id="7f563-179">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="7f563-180">3.5.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="7f563-180">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="7f563-181">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="7f563-181">Highlights since the last major release</span></span>
* <span data-ttu-id="7f563-182">Telemetria do lado do cliente atualizada.</span><span class="sxs-lookup"><span data-stu-id="7f563-182">Updated client side telemetry.</span></span>
* <span data-ttu-id="7f563-183">O Az.IotHub adicionou cmdlets para suportar a gestão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="7f563-183">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="7f563-184">O Az.SqlVirtualMachine adicionou cmdlets ao Serviço de Escuta do Grupo de Disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="7f563-184">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="7f563-185">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-185">Az.Accounts</span></span>
* <span data-ttu-id="7f563-186">SubscriptionId, TenantId e tempo de execução adicionados aos dados de telemetria do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="7f563-186">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="7f563-187">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f563-187">Az.Automation</span></span>
* <span data-ttu-id="7f563-188">Foi corrigido o erro no Exemplo 1 na documentação de referência de "New-AzAutomationSoftwareUpdateConfiguration"</span><span class="sxs-lookup"><span data-stu-id="7f563-188">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="7f563-189">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7f563-189">Az.CognitiveServices</span></span>
* <span data-ttu-id="7f563-190">SDK atualizado para a versão 7.0</span><span class="sxs-lookup"><span data-stu-id="7f563-190">Updated SDK to 7.0</span></span>
* <span data-ttu-id="7f563-191">Mensagem de erro melhorada quando o servidor responde ao corpo vazio</span><span class="sxs-lookup"><span data-stu-id="7f563-191">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-192">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-192">Az.Compute</span></span>
* <span data-ttu-id="7f563-193">Valor vazio permitido para ProximityPlacementGroupId durante a atualização</span><span class="sxs-lookup"><span data-stu-id="7f563-193">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="7f563-194">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="7f563-194">Az.FrontDoor</span></span>
* <span data-ttu-id="7f563-195">Cmdlet adicionado para obter definições de regras geridas que podem ser utilizadas na WAF</span><span class="sxs-lookup"><span data-stu-id="7f563-195">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="7f563-196">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="7f563-196">Az.IotHub</span></span>
* <span data-ttu-id="7f563-197">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="7f563-197">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="7f563-198">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="7f563-198">New Cmdlets are:</span></span>
    - <span data-ttu-id="7f563-199">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="7f563-199">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="7f563-200">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="7f563-200">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="7f563-201">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="7f563-201">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="7f563-202">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="7f563-202">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="7f563-203">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7f563-203">Az.KeyVault</span></span>
* <span data-ttu-id="7f563-204">Texto duplicado fixo para Add-AzKeyVaultKey.md</span><span class="sxs-lookup"><span data-stu-id="7f563-204">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="7f563-205">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="7f563-205">Az.Monitor</span></span>
* <span data-ttu-id="7f563-206">Descrição fixa do cmdlet Get-AzLog.</span><span class="sxs-lookup"><span data-stu-id="7f563-206">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="7f563-207">Foi adicionado um novo parâmetro chamado ActionGroupId ao comando "New-AzMetricAlertRuleV2".</span><span class="sxs-lookup"><span data-stu-id="7f563-207">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="7f563-208">O utilizador pode fornecer ActionGroupId(string) ou ActionGorup(ActivityLogAlertActionGroup).</span><span class="sxs-lookup"><span data-stu-id="7f563-208">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-209">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-209">Az.Network</span></span>
* <span data-ttu-id="7f563-210">Foi adicionada uma nota de parâmetro adicional para o parâmetro "-EnableProxyProtocol" para o cmdlet "New-AzPrivateLinkService".</span><span class="sxs-lookup"><span data-stu-id="7f563-210">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="7f563-211">Exemplo de FilterData fixo em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="7f563-211">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="7f563-212">Exemplo de Captura de Pacotes adicionado para capturar todos os pacotes internos e externos em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="7f563-212">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="7f563-213">Política do Azure Firewall suportada em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="7f563-213">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="7f563-214">Não foram adicionados novos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="7f563-214">No new cmdlets are added.</span></span> <span data-ttu-id="7f563-215">Simplificação da restrição da política de firewall em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="7f563-215">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-216">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-216">Az.RecoveryServices</span></span>
* <span data-ttu-id="7f563-217">Suporte adicionado da funcionalidade Restaurar como ficheiros para Bases de Dados SQL.</span><span class="sxs-lookup"><span data-stu-id="7f563-217">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-218">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-218">Az.Resources</span></span>
* <span data-ttu-id="7f563-219">Cmdlets de implementação de modelos refatorizados</span><span class="sxs-lookup"><span data-stu-id="7f563-219">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="7f563-220">Foram adicionados novos cmdlets para gerir implementações no grupo de gestão: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="7f563-220">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="7f563-221">Foram adicionados novos cmdlets para gerir implementações no inquilino: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="7f563-221">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="7f563-222">Cmdlets \*-AzDeployment refatorizados para trabalhar especificamente no âmbito da subscrição</span><span class="sxs-lookup"><span data-stu-id="7f563-222">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="7f563-223">Foram criados aliases \*-AzSubscriptionDeployment para os cmdlets \*-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="7f563-223">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="7f563-224">"Update-AzADApplication" fixo quando o parâmetro "AvailableToOtherTenants" não está definido</span><span class="sxs-lookup"><span data-stu-id="7f563-224">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="7f563-225">ApplicationObjectWithoutCredentialParameterSet removido para evitar AmbiguousParameterSetException.</span><span class="sxs-lookup"><span data-stu-id="7f563-225">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="7f563-226">Ficheiros de ajuda regenerados</span><span class="sxs-lookup"><span data-stu-id="7f563-226">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-227">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-227">Az.Sql</span></span>
* <span data-ttu-id="7f563-228">Suporte adicionado para restauro para um ponto anterior no tempo entre subscrições nas Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="7f563-228">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="7f563-229">Suporte adicionado para alterar a geração de hardware das Instâncias Geridas de SQL existentes</span><span class="sxs-lookup"><span data-stu-id="7f563-229">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="7f563-230">Exemplos de ajuda "Update-AzSqlServerVulnerabilityAssessmentSetting" fixos: saída do parâmetro/propriedade - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="7f563-230">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="7f563-231">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="7f563-231">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="7f563-232">Cmdlets adicionados para o Serviço de Escuta do Grupo de Disponibilidade</span><span class="sxs-lookup"><span data-stu-id="7f563-232">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="7f563-233">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="7f563-233">Az.StorageSync</span></span>
* <span data-ttu-id="7f563-234">Conjuntos de carateres suportados atualizados em "Invoke-AzStorageSyncCompatibilityCheck".</span><span class="sxs-lookup"><span data-stu-id="7f563-234">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="7f563-235">3.4.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="7f563-235">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="7f563-236">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="7f563-236">Highlights since the last major release</span></span>
* <span data-ttu-id="7f563-237">Versão inicial Az.CosmosDB 0.1.0 lançada</span><span class="sxs-lookup"><span data-stu-id="7f563-237">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="7f563-238">Foi adicionado suporte para Az.Network ConnectionMonitor V2</span><span class="sxs-lookup"><span data-stu-id="7f563-238">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="7f563-239">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-239">Az.Accounts</span></span>
* <span data-ttu-id="7f563-240">Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível</span><span class="sxs-lookup"><span data-stu-id="7f563-240">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="7f563-241">Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5</span><span class="sxs-lookup"><span data-stu-id="7f563-241">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="7f563-242">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7f563-242">Az.ApiManagement</span></span>
* <span data-ttu-id="7f563-243">**Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="7f563-243">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="7f563-244">**New-AzApiManagementProduct**\* e **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="7f563-244">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="7f563-245">Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472</span><span class="sxs-lookup"><span data-stu-id="7f563-245">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="7f563-246">**Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet</span><span class="sxs-lookup"><span data-stu-id="7f563-246">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-247">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-247">Az.Compute</span></span>
* <span data-ttu-id="7f563-248">Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.</span><span class="sxs-lookup"><span data-stu-id="7f563-248">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="7f563-249">Foi adicionado o cmdlet Update-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="7f563-249">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="7f563-250">Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7f563-250">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="7f563-251">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-251">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="7f563-252">Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="7f563-252">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="7f563-253">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="7f563-253">Az.DataFactory</span></span>
* <span data-ttu-id="7f563-254">Atualização do SDK .NET do ADF para a versão 4.7.0</span><span class="sxs-lookup"><span data-stu-id="7f563-254">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="7f563-255">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="7f563-255">Az.DeploymentManager</span></span>
* <span data-ttu-id="7f563-256">Adiciona operações LIST para os recursos</span><span class="sxs-lookup"><span data-stu-id="7f563-256">Adds LIST operations for resources</span></span>
* <span data-ttu-id="7f563-257">Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="7f563-257">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="7f563-258">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="7f563-258">Az.HDInsight</span></span>
* <span data-ttu-id="7f563-259">Foi corrigido o erro do documento de New-AzHDInsightCluster.</span><span class="sxs-lookup"><span data-stu-id="7f563-259">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="7f563-260">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7f563-260">Az.KeyVault</span></span>
* <span data-ttu-id="7f563-261">Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.</span><span class="sxs-lookup"><span data-stu-id="7f563-261">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-262">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-262">Az.Network</span></span>
* <span data-ttu-id="7f563-263">Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="7f563-263">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="7f563-264">Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão</span><span class="sxs-lookup"><span data-stu-id="7f563-264">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="7f563-265">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="7f563-265">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="7f563-266">Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="7f563-266">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="7f563-267">Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"</span><span class="sxs-lookup"><span data-stu-id="7f563-267">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="7f563-268">Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.</span><span class="sxs-lookup"><span data-stu-id="7f563-268">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="7f563-269">Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="7f563-269">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="7f563-270">Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="7f563-270">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="7f563-271">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7f563-271">New cmdlets added:</span></span>
        - <span data-ttu-id="7f563-272">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f563-272">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="7f563-273">Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f563-273">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="7f563-274">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="7f563-274">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="7f563-275">Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2</span><span class="sxs-lookup"><span data-stu-id="7f563-275">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="7f563-276">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="7f563-276">Az.PolicyInsights</span></span>
* <span data-ttu-id="7f563-277">Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar</span><span class="sxs-lookup"><span data-stu-id="7f563-277">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="7f563-278">Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation</span><span class="sxs-lookup"><span data-stu-id="7f563-278">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="7f563-279">Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política</span><span class="sxs-lookup"><span data-stu-id="7f563-279">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="7f563-280">Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="7f563-280">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-281">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-281">Az.RecoveryServices</span></span>
* <span data-ttu-id="7f563-282">Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.</span><span class="sxs-lookup"><span data-stu-id="7f563-282">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="7f563-283">O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.</span><span class="sxs-lookup"><span data-stu-id="7f563-283">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-284">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-284">Az.Resources</span></span>
* <span data-ttu-id="7f563-285">-Scope foi tornado opcional nos cmdlets \*-AzPolicyAssignment com subscrição de contexto predefinida</span><span class="sxs-lookup"><span data-stu-id="7f563-285">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="7f563-286">Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves</span><span class="sxs-lookup"><span data-stu-id="7f563-286">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-287">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-287">Az.Sql</span></span>
<span data-ttu-id="7f563-288">Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.</span><span class="sxs-lookup"><span data-stu-id="7f563-288">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-289">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-289">Az.Storage</span></span>
* <span data-ttu-id="7f563-290">Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7f563-290">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="7f563-291">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-291">New-AzStorageAccount</span></span>
* <span data-ttu-id="7f563-292">Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation</span><span class="sxs-lookup"><span data-stu-id="7f563-292">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="7f563-293">Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="7f563-293">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f563-294">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-294">Az.Websites</span></span>
* <span data-ttu-id="7f563-295">Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState</span><span class="sxs-lookup"><span data-stu-id="7f563-295">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="7f563-296">Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido</span><span class="sxs-lookup"><span data-stu-id="7f563-296">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="7f563-297">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="7f563-297">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="7f563-298">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-298">Az.Accounts</span></span>
* <span data-ttu-id="7f563-299">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="7f563-299">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="7f563-300">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="7f563-300">Az.Cdn</span></span>
* <span data-ttu-id="7f563-301">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="7f563-301">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-302">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-302">Az.Compute</span></span>
* <span data-ttu-id="7f563-303">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="7f563-303">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="7f563-304">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="7f563-304">Az.ContainerInstance</span></span>
* <span data-ttu-id="7f563-305">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="7f563-305">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="7f563-306">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="7f563-306">Az.DataBoxEdge</span></span>
* <span data-ttu-id="7f563-307">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="7f563-307">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="7f563-308">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="7f563-308">Get the Edge Storage Container</span></span>
* <span data-ttu-id="7f563-309">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="7f563-309">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="7f563-310">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="7f563-310">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="7f563-311">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="7f563-311">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="7f563-312">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="7f563-312">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="7f563-313">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="7f563-313">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="7f563-314">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="7f563-314">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="7f563-315">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="7f563-315">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="7f563-316">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="7f563-316">Get the Edge Storage Account</span></span>
* <span data-ttu-id="7f563-317">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="7f563-317">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="7f563-318">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="7f563-318">Create new Edge Storage Account</span></span>
* <span data-ttu-id="7f563-319">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="7f563-319">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="7f563-320">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="7f563-320">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="7f563-321">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="7f563-321">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="7f563-322">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="7f563-322">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="7f563-323">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="7f563-323">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="7f563-324">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="7f563-324">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="7f563-325">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="7f563-325">Az.DataFactory</span></span>
* <span data-ttu-id="7f563-326">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="7f563-326">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="7f563-327">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="7f563-327">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="7f563-328">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="7f563-328">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="7f563-329">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="7f563-329">Az.DevTestLabs</span></span>
* <span data-ttu-id="7f563-330">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="7f563-330">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="7f563-331">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="7f563-331">Az.EventHub</span></span>
* <span data-ttu-id="7f563-332">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="7f563-332">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="7f563-333">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="7f563-333">Az.HDInsight</span></span>
* <span data-ttu-id="7f563-334">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="7f563-334">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="7f563-335">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="7f563-335">Az.MachineLearning</span></span>
* <span data-ttu-id="7f563-336">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="7f563-336">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="7f563-337">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="7f563-337">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="7f563-338">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="7f563-338">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="7f563-339">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="7f563-339">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="7f563-340">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="7f563-340">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="7f563-341">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="7f563-341">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="7f563-342">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="7f563-342">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="7f563-343">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="7f563-343">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-344">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-344">Az.Network</span></span>
* <span data-ttu-id="7f563-345">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="7f563-345">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-346">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-346">Az.RecoveryServices</span></span>
* <span data-ttu-id="7f563-347">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-347">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="7f563-348">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-348">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="7f563-349">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-349">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="7f563-350">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-350">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-351">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-351">Az.Resources</span></span>
* <span data-ttu-id="7f563-352">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="7f563-352">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-353">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-353">Az.Sql</span></span>
* <span data-ttu-id="7f563-354">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="7f563-354">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="7f563-355">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="7f563-355">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="7f563-356">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="7f563-356">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="7f563-357">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="7f563-357">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-358">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-358">Az.Storage</span></span>
* <span data-ttu-id="7f563-359">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="7f563-359">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="7f563-360">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="7f563-360">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="7f563-361">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="7f563-361">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span> 
    - <span data-ttu-id="7f563-362">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-362">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="7f563-363">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-363">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="7f563-364">Geral</span><span class="sxs-lookup"><span data-stu-id="7f563-364">General</span></span>
* <span data-ttu-id="7f563-365">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="7f563-365">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="7f563-366">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-366">Az.Accounts</span></span>
* <span data-ttu-id="7f563-367">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="7f563-367">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="7f563-368">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="7f563-368">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="7f563-369">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="7f563-369">Az.Batch</span></span>
* <span data-ttu-id="7f563-370">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="7f563-370">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="7f563-371">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="7f563-371">Az.DataFactory</span></span>
* <span data-ttu-id="7f563-372">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="7f563-372">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="7f563-373">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="7f563-373">Az.FrontDoor</span></span>
* <span data-ttu-id="7f563-374">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="7f563-374">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="7f563-375">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="7f563-375">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="7f563-376">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="7f563-376">Az.HealthcareApis</span></span>
* <span data-ttu-id="7f563-377">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="7f563-377">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="7f563-378">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7f563-378">Az.KeyVault</span></span>
* <span data-ttu-id="7f563-379">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="7f563-379">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="7f563-380">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="7f563-380">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="7f563-381">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="7f563-381">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="7f563-382">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="7f563-382">Az.Monitor</span></span>
* <span data-ttu-id="7f563-383">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="7f563-383">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="7f563-384">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="7f563-384">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="7f563-385">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="7f563-385">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-386">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-386">Az.Network</span></span>
* <span data-ttu-id="7f563-387">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="7f563-387">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-388">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-388">Az.Resources</span></span>
* <span data-ttu-id="7f563-389">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="7f563-389">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="7f563-390">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="7f563-390">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-391">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-391">Az.Sql</span></span>
* <span data-ttu-id="7f563-392">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="7f563-392">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-393">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-393">Az.Storage</span></span>
* <span data-ttu-id="7f563-394">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="7f563-394">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="7f563-395">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="7f563-395">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="7f563-396">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="7f563-396">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="7f563-397">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="7f563-397">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="7f563-398">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="7f563-398">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="7f563-399">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="7f563-399">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="7f563-400">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="7f563-400">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span> 
    - <span data-ttu-id="7f563-401">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="7f563-401">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="7f563-402">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="7f563-402">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="7f563-403">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="7f563-403">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="7f563-404">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="7f563-404">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="7f563-405">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="7f563-405">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="7f563-406">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="7f563-406">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="7f563-407">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-407">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="7f563-408">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="7f563-408">Highlights since the last major release</span></span>
* <span data-ttu-id="7f563-409">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="7f563-409">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="7f563-410">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="7f563-410">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-411">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-411">Az.Compute</span></span>
* <span data-ttu-id="7f563-412">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="7f563-412">VM Reapply feature</span></span>
    - <span data-ttu-id="7f563-413">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="7f563-413">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="7f563-414">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="7f563-414">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="7f563-415">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="7f563-415">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="7f563-416">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="7f563-416">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="7f563-417">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="7f563-417">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="7f563-418">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="7f563-418">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="7f563-419">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="7f563-419">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="7f563-420">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="7f563-420">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="7f563-421">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="7f563-421">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="7f563-422">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="7f563-422">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="7f563-423">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="7f563-423">Az.DataBoxEdge</span></span>
* <span data-ttu-id="7f563-424">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="7f563-424">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="7f563-425">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="7f563-425">Get the Order</span></span>
* <span data-ttu-id="7f563-426">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="7f563-426">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="7f563-427">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="7f563-427">Create new Order</span></span>
* <span data-ttu-id="7f563-428">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="7f563-428">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="7f563-429">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="7f563-429">Remove the Order</span></span>
* <span data-ttu-id="7f563-430">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="7f563-430">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="7f563-431">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="7f563-431">Now creates Local Share</span></span>
* <span data-ttu-id="7f563-432">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="7f563-432">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="7f563-433">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="7f563-433">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="7f563-434">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="7f563-434">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="7f563-435">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="7f563-435">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="7f563-436">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="7f563-436">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="7f563-437">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="7f563-437">Gets the information about Triggers</span></span>
* <span data-ttu-id="7f563-438">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="7f563-438">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="7f563-439">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="7f563-439">Create new Triggers</span></span>
* <span data-ttu-id="7f563-440">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="7f563-440">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="7f563-441">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="7f563-441">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="7f563-442">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="7f563-442">Az.DataFactory</span></span>
* <span data-ttu-id="7f563-443">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="7f563-443">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="7f563-444">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="7f563-444">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="7f563-445">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f563-445">Az.DataLakeStore</span></span>
* <span data-ttu-id="7f563-446">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="7f563-446">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="7f563-447">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="7f563-447">Az.EventHub</span></span>
* <span data-ttu-id="7f563-448">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="7f563-448">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="7f563-449">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="7f563-449">Az.FrontDoor</span></span>
* <span data-ttu-id="7f563-450">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="7f563-450">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="7f563-451">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="7f563-451">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="7f563-452">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="7f563-452">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="7f563-453">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="7f563-453">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-454">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-454">Az.Network</span></span>
* <span data-ttu-id="7f563-455">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="7f563-455">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="7f563-456">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="7f563-456">Az.PrivateDns</span></span>
* <span data-ttu-id="7f563-457">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="7f563-457">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-458">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-458">Az.RecoveryServices</span></span>
* <span data-ttu-id="7f563-459">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="7f563-459">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="7f563-460">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="7f563-460">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="7f563-461">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="7f563-461">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="7f563-462">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="7f563-462">Az.RedisCache</span></span>
* <span data-ttu-id="7f563-463">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="7f563-463">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="7f563-464">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="7f563-464">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="7f563-465">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="7f563-465">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-466">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-466">Az.Resources</span></span>
- <span data-ttu-id="7f563-467">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="7f563-467">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="7f563-468">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="7f563-468">Updated create policy definition help example</span></span>
- <span data-ttu-id="7f563-469">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="7f563-469">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="7f563-470">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="7f563-470">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="7f563-471">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="7f563-471">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-472">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-472">Az.Sql</span></span>
* <span data-ttu-id="7f563-473">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="7f563-473">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="7f563-474">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="7f563-474">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="7f563-475">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-475">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="7f563-476">Geral</span><span class="sxs-lookup"><span data-stu-id="7f563-476">General</span></span>
* <span data-ttu-id="7f563-477">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="7f563-477">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="7f563-478">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-478">Az.Accounts</span></span>
* <span data-ttu-id="7f563-479">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="7f563-479">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="7f563-480">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="7f563-480">Az.Advisor</span></span>
* <span data-ttu-id="7f563-481">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="7f563-481">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="7f563-482">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="7f563-482">Az.Batch</span></span>
* <span data-ttu-id="7f563-483">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="7f563-483">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="7f563-484">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="7f563-484">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="7f563-485">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="7f563-485">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="7f563-486">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="7f563-486">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="7f563-487">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="7f563-487">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="7f563-488">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="7f563-488">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="7f563-489">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="7f563-489">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="7f563-490">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="7f563-490">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="7f563-491">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="7f563-491">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="7f563-492">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="7f563-492">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="7f563-493">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="7f563-493">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="7f563-494">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="7f563-494">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="7f563-495">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="7f563-495">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="7f563-496">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="7f563-496">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="7f563-497">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="7f563-497">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="7f563-498">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="7f563-498">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="7f563-499">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="7f563-499">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="7f563-500">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="7f563-500">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="7f563-501">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="7f563-501">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="7f563-502">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="7f563-502">This operation is no longer supported.</span></span>
* <span data-ttu-id="7f563-503">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="7f563-503">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="7f563-504">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="7f563-504">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="7f563-505">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="7f563-505">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="7f563-506">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="7f563-506">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span> 
  - <span data-ttu-id="7f563-507">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="7f563-507">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="7f563-508">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="7f563-508">New non-verified images are also now returned.</span></span> <span data-ttu-id="7f563-509">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="7f563-509">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="7f563-510">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="7f563-510">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="7f563-511">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="7f563-511">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="7f563-512">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="7f563-512">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="7f563-513">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="7f563-513">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="7f563-514">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="7f563-514">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="7f563-515">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="7f563-515">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="7f563-516">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="7f563-516">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="7f563-517">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="7f563-517">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="7f563-518">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="7f563-518">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="7f563-519">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="7f563-519">Az.Cdn</span></span>
* <span data-ttu-id="7f563-520">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="7f563-520">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="7f563-521">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="7f563-521">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-522">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-522">Az.Compute</span></span>
* <span data-ttu-id="7f563-523">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="7f563-523">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="7f563-524">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="7f563-524">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="7f563-525">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span><span class="sxs-lookup"><span data-stu-id="7f563-525">DiskEncryptionSetId parameter is added to the following cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span></span>        
        <span data-ttu-id="7f563-526">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="7f563-526">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="7f563-527">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-527">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="7f563-528">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-528">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="7f563-529">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="7f563-529">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="7f563-530">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="7f563-530">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="7f563-531">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="7f563-531">Breaking changes</span></span>
    - <span data-ttu-id="7f563-532">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="7f563-532">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="7f563-533">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="7f563-533">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="7f563-534">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="7f563-534">Az.DataFactory</span></span>
* <span data-ttu-id="7f563-535">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="7f563-535">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="7f563-536">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f563-536">Az.DataLakeStore</span></span>
* <span data-ttu-id="7f563-537">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="7f563-537">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="7f563-538">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="7f563-538">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="7f563-539">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="7f563-539">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="7f563-540">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="7f563-540">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="7f563-541">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="7f563-541">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="7f563-542">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="7f563-542">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="7f563-543">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="7f563-543">Az.FrontDoor</span></span>
* <span data-ttu-id="7f563-544">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="7f563-544">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="7f563-545">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="7f563-545">Az.HDInsight</span></span>
* <span data-ttu-id="7f563-546">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="7f563-546">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="7f563-547">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="7f563-547">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="7f563-548">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="7f563-548">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="7f563-549">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7f563-549">Removed five cmdlets:</span></span>
    - <span data-ttu-id="7f563-550">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="7f563-550">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="7f563-551">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="7f563-551">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="7f563-552">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="7f563-552">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="7f563-553">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="7f563-553">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="7f563-554">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="7f563-554">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="7f563-555">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7f563-555">Added three cmdlets:</span></span>
    - <span data-ttu-id="7f563-556">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="7f563-556">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="7f563-557">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="7f563-557">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="7f563-558">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="7f563-558">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="7f563-559">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="7f563-559">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="7f563-560">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="7f563-560">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="7f563-561">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="7f563-561">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="7f563-562">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7f563-562">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="7f563-563">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="7f563-563">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="7f563-564">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="7f563-564">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="7f563-565">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="7f563-565">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="7f563-566">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="7f563-566">Added some scenario test cases.</span></span>
* <span data-ttu-id="7f563-567">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="7f563-567">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="7f563-568">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="7f563-568">Az.IotHub</span></span>
* <span data-ttu-id="7f563-569">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="7f563-569">Breaking changes:</span></span>
    - <span data-ttu-id="7f563-570">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="7f563-570">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="7f563-571">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="7f563-571">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="7f563-572">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="7f563-572">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="7f563-573">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="7f563-573">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="7f563-574">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="7f563-574">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="7f563-575">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="7f563-575">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="7f563-576">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="7f563-576">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="7f563-577">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="7f563-577">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="7f563-578">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="7f563-578">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="7f563-579">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="7f563-579">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="7f563-580">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="7f563-580">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="7f563-581">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="7f563-581">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-582">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-582">Az.RecoveryServices</span></span>
* <span data-ttu-id="7f563-583">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-583">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="7f563-584">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-584">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="7f563-585">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-585">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="7f563-586">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-586">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="7f563-587">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-587">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="7f563-588">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-588">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="7f563-589">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-589">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="7f563-590">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-590">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="7f563-591">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="7f563-591">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-592">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-592">Az.Resources</span></span>
* <span data-ttu-id="7f563-593">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="7f563-593">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-594">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-594">Az.Network</span></span>
* <span data-ttu-id="7f563-595">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="7f563-595">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="7f563-596">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="7f563-596">Updated cmdlet:</span></span>
        - <span data-ttu-id="7f563-597">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-597">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="7f563-598">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-598">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="7f563-599">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-599">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="7f563-600">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-600">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="7f563-601">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-601">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="7f563-602">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="7f563-602">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="7f563-603">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="7f563-603">New cmdlet:</span></span>
        - <span data-ttu-id="7f563-604">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="7f563-604">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="7f563-605">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="7f563-605">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="7f563-606">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="7f563-606">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="7f563-607">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-607">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="7f563-608">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="7f563-608">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="7f563-609">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="7f563-609">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="7f563-610">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="7f563-610">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="7f563-611">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="7f563-611">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="7f563-612">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7f563-612">New cmdlets added:</span></span>
        - <span data-ttu-id="7f563-613">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="7f563-613">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="7f563-614">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="7f563-614">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="7f563-615">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="7f563-615">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="7f563-616">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="7f563-616">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="7f563-617">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="7f563-617">Set-AzVirtualHub</span></span>
* <span data-ttu-id="7f563-618">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="7f563-618">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="7f563-619">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="7f563-619">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="7f563-620">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="7f563-620">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="7f563-621">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="7f563-621">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="7f563-622">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="7f563-622">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="7f563-623">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="7f563-623">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="7f563-624">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-624">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="7f563-625">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7f563-625">New cmdlets added:</span></span>
        - <span data-ttu-id="7f563-626">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-626">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="7f563-627">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="7f563-627">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="7f563-628">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="7f563-628">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="7f563-629">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="7f563-629">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="7f563-630">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="7f563-630">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="7f563-631">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="7f563-631">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="7f563-632">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="7f563-632">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="7f563-633">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="7f563-633">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="7f563-634">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7f563-634">New cmdlets added:</span></span>
        - <span data-ttu-id="7f563-635">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="7f563-635">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="7f563-636">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="7f563-636">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="7f563-637">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="7f563-637">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="7f563-638">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="7f563-638">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="7f563-639">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="7f563-639">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="7f563-640">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="7f563-640">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="7f563-641">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="7f563-641">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="7f563-642">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="7f563-642">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="7f563-643">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="7f563-643">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="7f563-644">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="7f563-644">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="7f563-645">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="7f563-645">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="7f563-646">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="7f563-646">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="7f563-647">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="7f563-647">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="7f563-648">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="7f563-648">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="7f563-649">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="7f563-649">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="7f563-650">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="7f563-650">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="7f563-651">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="7f563-651">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="7f563-652">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7f563-652">New cmdlets added:</span></span>
        - <span data-ttu-id="7f563-653">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="7f563-653">New-AzIpGroup</span></span>
        - <span data-ttu-id="7f563-654">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="7f563-654">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="7f563-655">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="7f563-655">Get-AzIpGroup</span></span>
        - <span data-ttu-id="7f563-656">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="7f563-656">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="7f563-657">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7f563-657">Az.ServiceFabric</span></span>
* <span data-ttu-id="7f563-658">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="7f563-658">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-659">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-659">Az.Sql</span></span>
* <span data-ttu-id="7f563-660">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="7f563-660">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="7f563-661">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="7f563-661">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="7f563-662">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="7f563-662">Removed deprecated aliases:</span></span>
* <span data-ttu-id="7f563-663">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="7f563-663">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="7f563-664">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="7f563-664">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="7f563-665">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="7f563-665">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="7f563-666">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="7f563-666">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="7f563-667">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="7f563-667">Deprecate Advanced Threat Detection Settings cmdlets</span></span> 
* <span data-ttu-id="7f563-668">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="7f563-668">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-669">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-669">Az.Storage</span></span>
* <span data-ttu-id="7f563-670">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="7f563-670">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="7f563-671">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-671">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="7f563-672">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-672">Set-AzStorageAccount</span></span>
* <span data-ttu-id="7f563-673">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="7f563-673">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="7f563-674">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="7f563-674">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="7f563-675">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="7f563-675">Close-AzStorageFileHandle</span></span>
    
## <a name="280---october-2019"></a><span data-ttu-id="7f563-676">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-676">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="7f563-677">Geral</span><span class="sxs-lookup"><span data-stu-id="7f563-677">General</span></span>
* <span data-ttu-id="7f563-678">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="7f563-678">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="7f563-679">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-679">Az.Accounts</span></span>
* <span data-ttu-id="7f563-680">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="7f563-680">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="7f563-681">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7f563-681">Az.ApiManagement</span></span>
* <span data-ttu-id="7f563-682">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="7f563-682">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="7f563-683">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="7f563-683">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="7f563-684">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f563-684">Az.Automation</span></span>
* <span data-ttu-id="7f563-685">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="7f563-685">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="7f563-686">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="7f563-686">Az.Batch</span></span>
* <span data-ttu-id="7f563-687">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="7f563-687">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-688">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-688">Az.Compute</span></span>
* <span data-ttu-id="7f563-689">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="7f563-689">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="7f563-690">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="7f563-690">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="7f563-691">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="7f563-691">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="7f563-692">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="7f563-692">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="7f563-693">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="7f563-693">Az.DataFactory</span></span>
* <span data-ttu-id="7f563-694">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="7f563-694">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="7f563-695">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="7f563-695">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="7f563-696">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="7f563-696">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="7f563-697">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f563-697">Az.DataLakeStore</span></span>
* <span data-ttu-id="7f563-698">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="7f563-698">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="7f563-699">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="7f563-699">Az.HealthcareApis</span></span>
* <span data-ttu-id="7f563-700">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="7f563-700">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="7f563-701">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="7f563-701">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="7f563-702">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="7f563-702">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="7f563-703">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="7f563-703">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="7f563-704">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="7f563-704">Az.IotHub</span></span>
* <span data-ttu-id="7f563-705">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="7f563-705">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="7f563-706">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="7f563-706">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="7f563-707">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="7f563-707">Az.Monitor</span></span>
* <span data-ttu-id="7f563-708">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="7f563-708">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="7f563-709">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="7f563-709">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="7f563-710">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="7f563-710">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="7f563-711">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7f563-711">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-712">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-712">Az.Network</span></span>
* <span data-ttu-id="7f563-713">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="7f563-713">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="7f563-714">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="7f563-714">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="7f563-715">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7f563-715">New cmdlets added:</span></span>
        - <span data-ttu-id="7f563-716">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="7f563-716">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="7f563-717">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-717">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="7f563-718">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="7f563-718">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="7f563-719">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="7f563-719">Updated cmdlets:</span></span>
        - <span data-ttu-id="7f563-720">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-720">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="7f563-721">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-721">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="7f563-722">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-722">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="7f563-723">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="7f563-723">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="7f563-724">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="7f563-724">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="7f563-725">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="7f563-725">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="7f563-726">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="7f563-726">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="7f563-727">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="7f563-727">Az.RedisCache</span></span>
* <span data-ttu-id="7f563-728">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="7f563-728">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-729">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-729">Az.Sql</span></span>
* <span data-ttu-id="7f563-730">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="7f563-730">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-731">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-731">Az.Storage</span></span>
* <span data-ttu-id="7f563-732">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="7f563-732">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="7f563-733">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="7f563-733">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="7f563-734">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="7f563-734">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="7f563-735">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="7f563-735">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="7f563-736">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-736">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="7f563-737">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="7f563-737">Az.StorageSync</span></span>
* <span data-ttu-id="7f563-738">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="7f563-738">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f563-739">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-739">Az.Websites</span></span>
* <span data-ttu-id="7f563-740">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="7f563-740">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="7f563-741">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-741">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="7f563-742">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7f563-742">Az.ApiManagement</span></span>
* <span data-ttu-id="7f563-743">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="7f563-743">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="7f563-744">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="7f563-744">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="7f563-745">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="7f563-745">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="7f563-746">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f563-746">Az.Automation</span></span>
* <span data-ttu-id="7f563-747">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="7f563-747">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="7f563-748">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="7f563-748">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="7f563-749">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="7f563-749">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-750">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-750">Az.Compute</span></span>
* <span data-ttu-id="7f563-751">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-751">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="7f563-752">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-752">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="7f563-753">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="7f563-753">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="7f563-754">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="7f563-754">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="7f563-755">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="7f563-755">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="7f563-756">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="7f563-756">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="7f563-757">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="7f563-757">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="7f563-758">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="7f563-758">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="7f563-759">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="7f563-759">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="7f563-760">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="7f563-760">Az.DataFactory</span></span>
* <span data-ttu-id="7f563-761">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="7f563-761">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="7f563-762">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="7f563-762">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="7f563-763">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="7f563-763">Az.HDInsight</span></span>
* <span data-ttu-id="7f563-764">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="7f563-764">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="7f563-765">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="7f563-765">Az.IotHub</span></span>
* <span data-ttu-id="7f563-766">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="7f563-766">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="7f563-767">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="7f563-767">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="7f563-768">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="7f563-768">New cmdlets are:</span></span>
    - <span data-ttu-id="7f563-769">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="7f563-769">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="7f563-770">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="7f563-770">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="7f563-771">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="7f563-771">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="7f563-772">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="7f563-772">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="7f563-773">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="7f563-773">Az.Monitor</span></span>
* <span data-ttu-id="7f563-774">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="7f563-774">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="7f563-775">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="7f563-775">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="7f563-776">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="7f563-776">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="7f563-777">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="7f563-777">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="7f563-778">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="7f563-778">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="7f563-779">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="7f563-779">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="7f563-780">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="7f563-780">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="7f563-781">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="7f563-781">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="7f563-782">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="7f563-782">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="7f563-783">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="7f563-783">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="7f563-784">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="7f563-784">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="7f563-785">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="7f563-785">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="7f563-786">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="7f563-786">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="7f563-787">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="7f563-787">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="7f563-788">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="7f563-788">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="7f563-789">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="7f563-789">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="7f563-790">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="7f563-790">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="7f563-791">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="7f563-791">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="7f563-792">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="7f563-792">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="7f563-793">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="7f563-793">Overall improved help files</span></span>
* <span data-ttu-id="7f563-794">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="7f563-794">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-795">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-795">Az.Network</span></span>
* <span data-ttu-id="7f563-796">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="7f563-796">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="7f563-797">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="7f563-797">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="7f563-798">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="7f563-798">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="7f563-799">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="7f563-799">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="7f563-800">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="7f563-800">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="7f563-801">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="7f563-801">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="7f563-802">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="7f563-802">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="7f563-803">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="7f563-803">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="7f563-804">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f563-804">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="7f563-805">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="7f563-805">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="7f563-806">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="7f563-806">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="7f563-807">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="7f563-807">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="7f563-808">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="7f563-808">New cmdlets</span></span>
        - <span data-ttu-id="7f563-809">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="7f563-809">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="7f563-810">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-810">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="7f563-811">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="7f563-811">Updated cmdlet:</span></span>
        - <span data-ttu-id="7f563-812">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="7f563-812">New-VpnSite</span></span>
        - <span data-ttu-id="7f563-813">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="7f563-813">Update-VpnSite</span></span>
        - <span data-ttu-id="7f563-814">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-814">New-VpnConnection</span></span>
        - <span data-ttu-id="7f563-815">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-815">Update-VpnConnection</span></span>
* <span data-ttu-id="7f563-816">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="7f563-816">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-817">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-817">Az.RecoveryServices</span></span>
* <span data-ttu-id="7f563-818">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="7f563-818">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="7f563-819">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="7f563-819">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-820">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-820">Az.Resources</span></span>
* <span data-ttu-id="7f563-821">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="7f563-821">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="7f563-822">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7f563-822">Az.ServiceFabric</span></span>
* <span data-ttu-id="7f563-823">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="7f563-823">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="7f563-824">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="7f563-824">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="7f563-825">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="7f563-825">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="7f563-826">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="7f563-826">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="7f563-827">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="7f563-827">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="7f563-828">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="7f563-828">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="7f563-829">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="7f563-829">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="7f563-830">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="7f563-830">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="7f563-831">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="7f563-831">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="7f563-832">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="7f563-832">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="7f563-833">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="7f563-833">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="7f563-834">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="7f563-834">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="7f563-835">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="7f563-835">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="7f563-836">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="7f563-836">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="7f563-837">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="7f563-837">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="7f563-838">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="7f563-838">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="7f563-839">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="7f563-839">Az.SignalR</span></span>
* <span data-ttu-id="7f563-840">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="7f563-840">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-841">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-841">Az.Sql</span></span>
* <span data-ttu-id="7f563-842">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="7f563-842">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="7f563-843">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="7f563-843">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="7f563-844">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="7f563-844">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="7f563-845">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="7f563-845">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="7f563-846">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="7f563-846">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-847">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-847">Az.Storage</span></span>
* <span data-ttu-id="7f563-848">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="7f563-848">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="7f563-849">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="7f563-849">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="7f563-850">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="7f563-850">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="7f563-851">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="7f563-851">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="7f563-852">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="7f563-852">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="7f563-853">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="7f563-853">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="7f563-854">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="7f563-854">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="7f563-855">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="7f563-855">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="7f563-856">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="7f563-856">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="7f563-857">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="7f563-857">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="7f563-858">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="7f563-858">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f563-859">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-859">Az.Websites</span></span>
* <span data-ttu-id="7f563-860">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="7f563-860">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="7f563-861">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="7f563-861">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="7f563-862">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="7f563-862">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="7f563-863">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-863">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="7f563-864">Geral</span><span class="sxs-lookup"><span data-stu-id="7f563-864">General</span></span>
* <span data-ttu-id="7f563-865">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="7f563-865">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="7f563-866">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-866">Az.Accounts</span></span>
* <span data-ttu-id="7f563-867">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="7f563-867">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="7f563-868">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="7f563-868">Az.Aks</span></span>
* <span data-ttu-id="7f563-869">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="7f563-869">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="7f563-870">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="7f563-870">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="7f563-871">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7f563-871">Az.ApiManagement</span></span>
* <span data-ttu-id="7f563-872">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="7f563-872">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="7f563-873">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="7f563-873">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="7f563-874">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="7f563-874">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="7f563-875">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="7f563-875">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="7f563-876">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="7f563-876">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="7f563-877">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="7f563-877">Az.Batch</span></span>
* <span data-ttu-id="7f563-878">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="7f563-878">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="7f563-879">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="7f563-879">Az.Cdn</span></span>
* <span data-ttu-id="7f563-880">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="7f563-880">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-881">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-881">Az.Compute</span></span>
* <span data-ttu-id="7f563-882">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-882">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="7f563-883">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="7f563-883">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="7f563-884">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="7f563-884">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="7f563-885">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="7f563-885">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="7f563-886">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="7f563-886">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="7f563-887">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="7f563-887">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="7f563-888">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="7f563-888">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="7f563-889">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="7f563-889">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="7f563-890">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="7f563-890">Az.DataFactory</span></span>
* <span data-ttu-id="7f563-891">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="7f563-891">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="7f563-892">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="7f563-892">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="7f563-893">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="7f563-893">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="7f563-894">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="7f563-894">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="7f563-895">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f563-895">Az.DataLakeStore</span></span>
* <span data-ttu-id="7f563-896">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="7f563-896">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="7f563-897">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="7f563-897">Az.EventHub</span></span>
* <span data-ttu-id="7f563-898">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="7f563-898">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="7f563-899">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="7f563-899">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="7f563-900">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="7f563-900">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="7f563-901">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="7f563-901">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="7f563-902">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="7f563-902">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="7f563-903">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="7f563-903">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="7f563-904">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="7f563-904">Az.Monitor</span></span>
* <span data-ttu-id="7f563-905">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="7f563-905">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-906">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-906">Az.Network</span></span>
* <span data-ttu-id="7f563-907">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="7f563-907">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="7f563-908">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="7f563-908">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="7f563-909">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="7f563-909">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="7f563-910">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="7f563-910">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="7f563-911">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="7f563-911">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="7f563-912">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="7f563-912">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="7f563-913">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="7f563-913">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="7f563-914">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="7f563-914">Az.OperationalInsights</span></span>
* <span data-ttu-id="7f563-915">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="7f563-915">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="7f563-916">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="7f563-916">Added example</span></span>
    - <span data-ttu-id="7f563-917">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="7f563-917">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="7f563-918">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="7f563-918">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="7f563-919">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="7f563-919">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-920">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-920">Az.RecoveryServices</span></span>
* <span data-ttu-id="7f563-921">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="7f563-921">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-922">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-922">Az.Resources</span></span>
* <span data-ttu-id="7f563-923">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="7f563-923">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="7f563-924">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="7f563-924">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="7f563-925">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="7f563-925">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="7f563-926">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="7f563-926">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="7f563-927">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7f563-927">Az.ServiceBus</span></span>
* <span data-ttu-id="7f563-928">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="7f563-928">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="7f563-929">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="7f563-929">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="7f563-930">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="7f563-930">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="7f563-931">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7f563-931">Az.ServiceFabric</span></span>
* <span data-ttu-id="7f563-932">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="7f563-932">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="7f563-933">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="7f563-933">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="7f563-934">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="7f563-934">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="7f563-935">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="7f563-935">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="7f563-936">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="7f563-936">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="7f563-937">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="7f563-937">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-938">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-938">Az.Sql</span></span>
* <span data-ttu-id="7f563-939">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="7f563-939">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-940">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-940">Az.Storage</span></span>
* <span data-ttu-id="7f563-941">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="7f563-941">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="7f563-942">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="7f563-942">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="7f563-943">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="7f563-943">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="7f563-944">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="7f563-944">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="7f563-945">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="7f563-945">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="7f563-946">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="7f563-946">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f563-947">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-947">Az.Websites</span></span>
* <span data-ttu-id="7f563-948">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="7f563-948">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="7f563-949">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-949">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="7f563-950">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-950">Az.Accounts</span></span>
* <span data-ttu-id="7f563-951">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="7f563-951">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="7f563-952">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="7f563-952">Az.ApplicationInsights</span></span>
* <span data-ttu-id="7f563-953">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="7f563-953">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="7f563-954">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f563-954">Az.Automation</span></span>
* <span data-ttu-id="7f563-955">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="7f563-955">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="7f563-956">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7f563-956">Az.CognitiveServices</span></span>
* <span data-ttu-id="7f563-957">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="7f563-957">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-958">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-958">Az.Compute</span></span>
* <span data-ttu-id="7f563-959">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="7f563-959">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="7f563-960">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="7f563-960">Az.ContainerRegistry</span></span>
* <span data-ttu-id="7f563-961">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="7f563-961">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="7f563-962">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="7f563-962">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="7f563-963">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="7f563-963">Az.DataFactory</span></span>
* <span data-ttu-id="7f563-964">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="7f563-964">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="7f563-965">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="7f563-965">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="7f563-966">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="7f563-966">Az.EventHub</span></span>
* <span data-ttu-id="7f563-967">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="7f563-967">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="7f563-968">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="7f563-968">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="7f563-969">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7f563-969">Az.KeyVault</span></span>
* <span data-ttu-id="7f563-970">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="7f563-970">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="7f563-971">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="7f563-971">Az.LogicApp</span></span>
* <span data-ttu-id="7f563-972">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="7f563-972">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="7f563-973">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="7f563-973">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="7f563-974">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="7f563-974">Az.ManagedServices</span></span>
* <span data-ttu-id="7f563-975">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="7f563-975">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-976">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-976">Az.Network</span></span>
* <span data-ttu-id="7f563-977">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="7f563-977">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="7f563-978">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="7f563-978">New cmdlets</span></span>
        - <span data-ttu-id="7f563-979">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="7f563-979">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="7f563-980">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="7f563-980">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="7f563-981">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-981">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="7f563-982">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-982">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="7f563-983">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-983">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="7f563-984">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-984">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="7f563-985">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="7f563-985">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="7f563-986">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="7f563-986">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="7f563-987">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="7f563-987">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="7f563-988">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-988">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="7f563-989">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="7f563-989">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="7f563-990">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="7f563-990">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="7f563-991">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="7f563-991">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="7f563-992">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="7f563-992">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="7f563-993">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="7f563-993">Updated cmdlets</span></span>
        - <span data-ttu-id="7f563-994">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-994">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="7f563-995">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-995">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="7f563-996">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-996">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="7f563-997">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-997">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="7f563-998">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f563-998">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="7f563-999">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="7f563-999">Updated cmdlet:</span></span>
        - <span data-ttu-id="7f563-1000">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-1000">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="7f563-1001">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-1001">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="7f563-1002">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-1002">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="7f563-1003">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="7f563-1003">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="7f563-1004">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="7f563-1004">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="7f563-1005">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="7f563-1005">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="7f563-1006">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="7f563-1006">Az.OperationalInsights</span></span>
* <span data-ttu-id="7f563-1007">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="7f563-1007">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="7f563-1008">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="7f563-1008">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-1009">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1009">Az.RecoveryServices</span></span>
* <span data-ttu-id="7f563-1010">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="7f563-1010">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="7f563-1011">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="7f563-1011">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="7f563-1012">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="7f563-1012">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="7f563-1013">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="7f563-1013">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="7f563-1014">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="7f563-1014">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="7f563-1015">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="7f563-1015">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="7f563-1016">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="7f563-1016">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="7f563-1017">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="7f563-1017">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="7f563-1018">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="7f563-1018">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="7f563-1019">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="7f563-1019">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-1020">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-1020">Az.Resources</span></span>
- <span data-ttu-id="7f563-1021">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="7f563-1021">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="7f563-1022">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="7f563-1022">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="7f563-1023">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7f563-1023">Az.ServiceBus</span></span>
* <span data-ttu-id="7f563-1024">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="7f563-1024">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="7f563-1025">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="7f563-1025">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-1026">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1026">Az.Sql</span></span>
* <span data-ttu-id="7f563-1027">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="7f563-1027">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="7f563-1028">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="7f563-1028">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="7f563-1029">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="7f563-1029">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-1030">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-1030">Az.Storage</span></span>
* <span data-ttu-id="7f563-1031">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="7f563-1031">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="7f563-1032">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="7f563-1032">Az.StorageSync</span></span>
* <span data-ttu-id="7f563-1033">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="7f563-1033">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="7f563-1034">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="7f563-1034">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f563-1035">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-1035">Az.Websites</span></span>
* <span data-ttu-id="7f563-1036">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="7f563-1036">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="7f563-1037">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="7f563-1037">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="7f563-1038">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="7f563-1038">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="7f563-1039">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-1039">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="7f563-1040">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-1040">Az.Accounts</span></span>
* <span data-ttu-id="7f563-1041">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="7f563-1041">Add support for profile cmdlets</span></span>
* <span data-ttu-id="7f563-1042">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="7f563-1042">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="7f563-1043">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="7f563-1043">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="7f563-1044">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="7f563-1044">Az.Advisor</span></span>
* <span data-ttu-id="7f563-1045">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="7f563-1045">GA release of Az.Advisor</span></span>
* <span data-ttu-id="7f563-1046">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="7f563-1046">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="7f563-1047">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7f563-1047">Az.ApiManagement</span></span>
* <span data-ttu-id="7f563-1048">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="7f563-1048">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="7f563-1049">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="7f563-1049">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="7f563-1050">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="7f563-1050">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="7f563-1051">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="7f563-1051">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="7f563-1052">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="7f563-1052">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="7f563-1053">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="7f563-1053">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="7f563-1054">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="7f563-1054">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="7f563-1055">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f563-1055">Az.Automation</span></span>
* <span data-ttu-id="7f563-1056">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="7f563-1056">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-1057">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-1057">Az.Compute</span></span>
* <span data-ttu-id="7f563-1058">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-1058">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="7f563-1059">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="7f563-1059">Az.DataFactory</span></span>
* <span data-ttu-id="7f563-1060">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="7f563-1060">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="7f563-1061">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="7f563-1061">Az.EventGrid</span></span>
* <span data-ttu-id="7f563-1062">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="7f563-1062">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="7f563-1063">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="7f563-1063">Az.IotHub</span></span>
* <span data-ttu-id="7f563-1064">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="7f563-1064">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-1065">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1065">Az.Network</span></span>
* <span data-ttu-id="7f563-1066">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="7f563-1066">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="7f563-1067">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="7f563-1067">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="7f563-1068">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="7f563-1068">Az.PolicyInsights</span></span>
* <span data-ttu-id="7f563-1069">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="7f563-1069">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="7f563-1070">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="7f563-1070">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="7f563-1071">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="7f563-1071">Az.OperationalInsights</span></span>
* <span data-ttu-id="7f563-1072">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="7f563-1072">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-1073">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1073">Az.RecoveryServices</span></span>
* <span data-ttu-id="7f563-1074">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="7f563-1074">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-1075">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-1075">Az.Resources</span></span>
    - <span data-ttu-id="7f563-1076">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="7f563-1076">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="7f563-1077">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="7f563-1077">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="7f563-1078">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="7f563-1078">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="7f563-1079">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="7f563-1079">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="7f563-1080">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7f563-1080">Az.ServiceBus</span></span>
* <span data-ttu-id="7f563-1081">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="7f563-1081">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-1082">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1082">Az.Sql</span></span>
* <span data-ttu-id="7f563-1083">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="7f563-1083">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="7f563-1084">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="7f563-1084">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="7f563-1085">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="7f563-1085">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="7f563-1086">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="7f563-1086">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="7f563-1087">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="7f563-1087">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="7f563-1088">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="7f563-1088">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="7f563-1089">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="7f563-1089">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="7f563-1090">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="7f563-1090">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="7f563-1091">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="7f563-1091">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-1092">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-1092">Az.Storage</span></span>
* <span data-ttu-id="7f563-1093">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="7f563-1093">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="7f563-1094">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="7f563-1094">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="7f563-1095">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="7f563-1095">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="7f563-1096">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="7f563-1096">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="7f563-1097">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="7f563-1097">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="7f563-1098">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-1098">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="7f563-1099">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-1099">Set-AzStorageAccount</span></span>
* <span data-ttu-id="7f563-1100">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="7f563-1100">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="7f563-1101">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="7f563-1101">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="7f563-1102">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="7f563-1102">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="7f563-1103">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="7f563-1103">Az.StorageSync</span></span>
* <span data-ttu-id="7f563-1104">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="7f563-1104">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="7f563-1105">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-1105">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="7f563-1106">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-1106">Az.Accounts</span></span>
* <span data-ttu-id="7f563-1107">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="7f563-1107">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="7f563-1108">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="7f563-1108">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="7f563-1109">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="7f563-1109">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="7f563-1110">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="7f563-1110">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="7f563-1111">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="7f563-1111">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-1112">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-1112">Az.Compute</span></span>
* <span data-ttu-id="7f563-1113">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="7f563-1113">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="7f563-1114">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="7f563-1114">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="7f563-1115">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="7f563-1115">Az.Dns</span></span>
* <span data-ttu-id="7f563-1116">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="7f563-1116">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="7f563-1117">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="7f563-1117">Az.EventGrid</span></span>
* <span data-ttu-id="7f563-1118">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="7f563-1118">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="7f563-1119">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7f563-1119">New cmdlets:</span></span>
    - <span data-ttu-id="7f563-1120">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="7f563-1120">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="7f563-1121">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="7f563-1121">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="7f563-1122">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="7f563-1122">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="7f563-1123">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-1123">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="7f563-1124">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="7f563-1124">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="7f563-1125">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="7f563-1125">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="7f563-1126">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="7f563-1126">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="7f563-1127">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="7f563-1127">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="7f563-1128">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="7f563-1128">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="7f563-1129">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="7f563-1129">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="7f563-1130">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="7f563-1130">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="7f563-1131">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="7f563-1131">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="7f563-1132">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="7f563-1132">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="7f563-1133">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="7f563-1133">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="7f563-1134">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="7f563-1134">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="7f563-1135">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="7f563-1135">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="7f563-1136">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="7f563-1136">Updated cmdlets:</span></span>
    - <span data-ttu-id="7f563-1137">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="7f563-1137">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="7f563-1138">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="7f563-1138">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="7f563-1139">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="7f563-1139">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="7f563-1140">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="7f563-1140">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="7f563-1141">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="7f563-1141">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="7f563-1142">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="7f563-1142">Event subscription expiration date,</span></span>
            - <span data-ttu-id="7f563-1143">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="7f563-1143">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="7f563-1144">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="7f563-1144">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="7f563-1145">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="7f563-1145">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="7f563-1146">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="7f563-1146">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="7f563-1147">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="7f563-1147">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="7f563-1148">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="7f563-1148">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="7f563-1149">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="7f563-1149">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="7f563-1150">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="7f563-1150">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="7f563-1151">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="7f563-1151">Az.FrontDoor</span></span>
* <span data-ttu-id="7f563-1152">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="7f563-1152">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="7f563-1153">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="7f563-1153">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="7f563-1154">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="7f563-1154">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="7f563-1155">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="7f563-1155">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-1156">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1156">Az.Network</span></span>
* <span data-ttu-id="7f563-1157">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="7f563-1157">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="7f563-1158">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="7f563-1158">New cmdlets</span></span>
        - <span data-ttu-id="7f563-1159">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="7f563-1159">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="7f563-1160">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="7f563-1160">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="7f563-1161">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="7f563-1161">New cmdlets</span></span> 
        - <span data-ttu-id="7f563-1162">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="7f563-1162">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="7f563-1163">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="7f563-1163">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="7f563-1164">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="7f563-1164">New cmdlets</span></span> 
        - <span data-ttu-id="7f563-1165">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="7f563-1165">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="7f563-1166">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="7f563-1166">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="7f563-1167">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="7f563-1167">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="7f563-1168">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-1168">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="7f563-1169">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-1169">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="7f563-1170">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="7f563-1170">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="7f563-1171">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="7f563-1171">New cmdlets</span></span>
        - <span data-ttu-id="7f563-1172">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="7f563-1172">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="7f563-1173">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="7f563-1173">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="7f563-1174">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="7f563-1174">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="7f563-1175">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-1175">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="7f563-1176">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="7f563-1176">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="7f563-1177">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="7f563-1177">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="7f563-1178">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="7f563-1178">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="7f563-1179">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="7f563-1179">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="7f563-1180">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="7f563-1180">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="7f563-1181">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="7f563-1181">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="7f563-1182">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f563-1182">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="7f563-1183">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="7f563-1183">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="7f563-1184">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f563-1184">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="7f563-1185">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="7f563-1185">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="7f563-1186">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="7f563-1186">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="7f563-1187">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="7f563-1187">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="7f563-1188">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="7f563-1188">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="7f563-1189">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="7f563-1189">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="7f563-1190">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="7f563-1190">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="7f563-1191">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="7f563-1191">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="7f563-1192">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="7f563-1192">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="7f563-1193">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="7f563-1193">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="7f563-1194">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="7f563-1194">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="7f563-1195">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="7f563-1195">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="7f563-1196">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="7f563-1196">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="7f563-1197">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="7f563-1197">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="7f563-1198">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="7f563-1198">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="7f563-1199">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="7f563-1199">Az.OperationalInsights</span></span>
* <span data-ttu-id="7f563-1200">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="7f563-1200">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-1201">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-1201">Az.Resources</span></span>
* <span data-ttu-id="7f563-1202">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="7f563-1202">Support for additional Template Export options</span></span>
    - <span data-ttu-id="7f563-1203">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="7f563-1203">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="7f563-1204">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="7f563-1204">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="7f563-1205">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="7f563-1205">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="7f563-1206">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7f563-1206">Az.ServiceFabric</span></span>
* <span data-ttu-id="7f563-1207">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="7f563-1207">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-1208">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1208">Az.Sql</span></span>
* <span data-ttu-id="7f563-1209">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="7f563-1209">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="7f563-1210">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="7f563-1210">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="7f563-1211">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="7f563-1211">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="7f563-1212">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="7f563-1212">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="7f563-1213">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="7f563-1213">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="7f563-1214">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="7f563-1214">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="7f563-1215">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="7f563-1215">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="7f563-1216">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="7f563-1216">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-1217">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-1217">Az.Storage</span></span>
* <span data-ttu-id="7f563-1218">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="7f563-1218">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="7f563-1219">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-1219">New-AzStorageAccount</span></span>
* <span data-ttu-id="7f563-1220">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="7f563-1220">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="7f563-1221">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="7f563-1221">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f563-1222">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-1222">Az.Websites</span></span>
* <span data-ttu-id="7f563-1223">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="7f563-1223">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="7f563-1224">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="7f563-1224">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="7f563-1225">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-1225">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="7f563-1226">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="7f563-1226">Az.Cdn</span></span>
* <span data-ttu-id="7f563-1227">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="7f563-1227">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-1228">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-1228">Az.Compute</span></span>
* <span data-ttu-id="7f563-1229">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="7f563-1229">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="7f563-1230">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="7f563-1230">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="7f563-1231">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="7f563-1231">Az.EventHub</span></span>
* <span data-ttu-id="7f563-1232">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="7f563-1232">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="7f563-1233">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="7f563-1233">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-1234">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1234">Az.Network</span></span>
* <span data-ttu-id="7f563-1235">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="7f563-1235">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="7f563-1236">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="7f563-1236">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="7f563-1237">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="7f563-1237">Az.PolicyInsights</span></span>
* <span data-ttu-id="7f563-1238">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="7f563-1238">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-1239">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1239">Az.RecoveryServices</span></span>
* <span data-ttu-id="7f563-1240">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="7f563-1240">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="7f563-1241">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7f563-1241">Az.ServiceBus</span></span>
* <span data-ttu-id="7f563-1242">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="7f563-1242">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="7f563-1243">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7f563-1243">Az.ServiceFabric</span></span>
* <span data-ttu-id="7f563-1244">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="7f563-1244">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="7f563-1245">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7f563-1245">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-1246">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1246">Az.Sql</span></span>
* <span data-ttu-id="7f563-1247">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="7f563-1247">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="7f563-1248">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="7f563-1248">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="7f563-1249">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="7f563-1249">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="7f563-1250">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="7f563-1250">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f563-1251">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-1251">Az.Websites</span></span>
* <span data-ttu-id="7f563-1252">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="7f563-1252">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="7f563-1253">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-1253">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="7f563-1254">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7f563-1254">Az.ApiManagement</span></span>
* <span data-ttu-id="7f563-1255">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="7f563-1255">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="7f563-1256">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="7f563-1256">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="7f563-1257">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="7f563-1257">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="7f563-1258">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="7f563-1258">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="7f563-1259">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="7f563-1259">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="7f563-1260">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="7f563-1260">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="7f563-1261">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="7f563-1261">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="7f563-1262">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="7f563-1262">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="7f563-1263">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7f563-1263">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="7f563-1264">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="7f563-1264">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="7f563-1265">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="7f563-1265">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="7f563-1266">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="7f563-1266">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="7f563-1267">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="7f563-1267">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="7f563-1268">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="7f563-1268">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="7f563-1269">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="7f563-1269">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="7f563-1270">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="7f563-1270">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="7f563-1271">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="7f563-1271">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="7f563-1272">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="7f563-1272">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="7f563-1273">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="7f563-1273">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="7f563-1274">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="7f563-1274">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="7f563-1275">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="7f563-1275">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="7f563-1276">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="7f563-1276">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="7f563-1277">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="7f563-1277">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="7f563-1278">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7f563-1278">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="7f563-1279">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="7f563-1279">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="7f563-1280">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="7f563-1280">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="7f563-1281">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="7f563-1281">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="7f563-1282">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="7f563-1282">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="7f563-1283">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="7f563-1283">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="7f563-1284">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="7f563-1284">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="7f563-1285">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="7f563-1285">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="7f563-1286">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="7f563-1286">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="7f563-1287">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="7f563-1287">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="7f563-1288">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="7f563-1288">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="7f563-1289">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="7f563-1289">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="7f563-1290">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="7f563-1290">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="7f563-1291">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="7f563-1291">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="7f563-1292">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="7f563-1292">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="7f563-1293">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="7f563-1293">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="7f563-1294">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="7f563-1294">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="7f563-1295">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="7f563-1295">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="7f563-1296">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="7f563-1296">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="7f563-1297">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="7f563-1297">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="7f563-1298">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="7f563-1298">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="7f563-1299">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="7f563-1299">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="7f563-1300">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="7f563-1300">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="7f563-1301">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="7f563-1301">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="7f563-1302">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="7f563-1302">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="7f563-1303">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="7f563-1303">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="7f563-1304">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="7f563-1304">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="7f563-1305">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="7f563-1305">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="7f563-1306">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="7f563-1306">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="7f563-1307">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="7f563-1307">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="7f563-1308">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="7f563-1308">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="7f563-1309">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="7f563-1309">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="7f563-1310">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="7f563-1310">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="7f563-1311">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="7f563-1311">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="7f563-1312">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="7f563-1312">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="7f563-1313">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="7f563-1313">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="7f563-1314">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="7f563-1314">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="7f563-1315">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="7f563-1315">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="7f563-1316">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="7f563-1316">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="7f563-1317">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="7f563-1317">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="7f563-1318">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="7f563-1318">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="7f563-1319">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="7f563-1319">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="7f563-1320">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="7f563-1320">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="7f563-1321">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="7f563-1321">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="7f563-1322">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="7f563-1322">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="7f563-1323">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="7f563-1323">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="7f563-1324">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="7f563-1324">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="7f563-1325">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="7f563-1325">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="7f563-1326">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="7f563-1326">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="7f563-1327">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="7f563-1327">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="7f563-1328">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="7f563-1328">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="7f563-1329">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="7f563-1329">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="7f563-1330">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="7f563-1330">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="7f563-1331">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="7f563-1331">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="7f563-1332">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f563-1332">Az.Automation</span></span>
* <span data-ttu-id="7f563-1333">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="7f563-1333">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="7f563-1334">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="7f563-1334">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="7f563-1335">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="7f563-1335">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="7f563-1336">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="7f563-1336">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="7f563-1337">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="7f563-1337">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="7f563-1338">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="7f563-1338">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="7f563-1339">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="7f563-1339">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-1340">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-1340">Az.Compute</span></span>
* <span data-ttu-id="7f563-1341">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="7f563-1341">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="7f563-1342">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="7f563-1342">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="7f563-1343">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f563-1343">Az.DataLakeStore</span></span>
* <span data-ttu-id="7f563-1344">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="7f563-1344">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="7f563-1345">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="7f563-1345">Az.Monitor</span></span>
* <span data-ttu-id="7f563-1346">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="7f563-1346">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-1347">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1347">Az.Network</span></span>
* <span data-ttu-id="7f563-1348">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="7f563-1348">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="7f563-1349">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="7f563-1349">Updated cmdlet:</span></span>
        - <span data-ttu-id="7f563-1350">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="7f563-1350">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="7f563-1351">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7f563-1351">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-1352">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-1352">Az.Resources</span></span>
* <span data-ttu-id="7f563-1353">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="7f563-1353">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-1354">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1354">Az.Sql</span></span>
* <span data-ttu-id="7f563-1355">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="7f563-1355">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="7f563-1356">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-1356">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="7f563-1357">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-1357">Az.Accounts</span></span>
* <span data-ttu-id="7f563-1358">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="7f563-1358">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="7f563-1359">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1359">Az.CognitiveServices</span></span>
* <span data-ttu-id="7f563-1360">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="7f563-1360">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="7f563-1361">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="7f563-1361">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-1362">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-1362">Az.Compute</span></span>
* <span data-ttu-id="7f563-1363">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="7f563-1363">Proximity placement group feature.</span></span>
    - <span data-ttu-id="7f563-1364">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="7f563-1364">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="7f563-1365">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-1365">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="7f563-1366">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="7f563-1366">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="7f563-1367">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="7f563-1367">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="7f563-1368">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="7f563-1368">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="7f563-1369">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="7f563-1369">Breaking changes</span></span>
    - <span data-ttu-id="7f563-1370">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="7f563-1370">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="7f563-1371">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="7f563-1371">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="7f563-1372">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="7f563-1372">Az.DeploymentManager</span></span>
* <span data-ttu-id="7f563-1373">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="7f563-1373">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="7f563-1374">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="7f563-1374">Az.Dns</span></span>
* <span data-ttu-id="7f563-1375">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="7f563-1375">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="7f563-1376">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="7f563-1376">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="7f563-1377">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="7f563-1377">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="7f563-1378">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="7f563-1378">Az.FrontDoor</span></span>
* <span data-ttu-id="7f563-1379">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="7f563-1379">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="7f563-1380">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="7f563-1380">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="7f563-1381">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="7f563-1381">Az.HDInsight</span></span>
* <span data-ttu-id="7f563-1382">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7f563-1382">Removed two cmdlets:</span></span>
    - <span data-ttu-id="7f563-1383">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="7f563-1383">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="7f563-1384">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="7f563-1384">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="7f563-1385">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="7f563-1385">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="7f563-1386">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="7f563-1386">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="7f563-1387">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="7f563-1387">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="7f563-1388">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="7f563-1388">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="7f563-1389">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="7f563-1389">Az.Monitor</span></span>
* <span data-ttu-id="7f563-1390">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="7f563-1390">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="7f563-1391">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="7f563-1391">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="7f563-1392">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="7f563-1392">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="7f563-1393">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="7f563-1393">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="7f563-1394">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="7f563-1394">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="7f563-1395">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="7f563-1395">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="7f563-1396">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="7f563-1396">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="7f563-1397">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="7f563-1397">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="7f563-1398">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="7f563-1398">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="7f563-1399">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="7f563-1399">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="7f563-1400">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="7f563-1400">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="7f563-1401">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="7f563-1401">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="7f563-1402">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="7f563-1402">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="7f563-1403">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="7f563-1403">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-1404">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1404">Az.Network</span></span>
* <span data-ttu-id="7f563-1405">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="7f563-1405">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="7f563-1406">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="7f563-1406">New cmdlets</span></span>
        - <span data-ttu-id="7f563-1407">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="7f563-1407">New-AzNatGateway</span></span>
        - <span data-ttu-id="7f563-1408">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="7f563-1408">Get-AzNatGateway</span></span>
        - <span data-ttu-id="7f563-1409">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="7f563-1409">Set-AzNatGateway</span></span>
        - <span data-ttu-id="7f563-1410">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="7f563-1410">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="7f563-1411">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="7f563-1411">Updated cmdlets</span></span>
        - <span data-ttu-id="7f563-1412">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="7f563-1412">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="7f563-1413">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="7f563-1413">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="7f563-1414">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="7f563-1414">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="7f563-1415">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="7f563-1415">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="7f563-1416">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="7f563-1416">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="7f563-1417">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="7f563-1417">Az.PolicyInsights</span></span>
* <span data-ttu-id="7f563-1418">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="7f563-1418">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="7f563-1419">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="7f563-1419">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="7f563-1420">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="7f563-1420">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-1421">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1421">Az.RecoveryServices</span></span>
* <span data-ttu-id="7f563-1422">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="7f563-1422">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="7f563-1423">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="7f563-1423">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="7f563-1424">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="7f563-1424">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="7f563-1425">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-1425">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="7f563-1426">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="7f563-1426">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="7f563-1427">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="7f563-1427">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="7f563-1428">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="7f563-1428">Az.Relay</span></span>
* <span data-ttu-id="7f563-1429">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="7f563-1429">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="7f563-1430">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7f563-1430">Az.ServiceBus</span></span>
* <span data-ttu-id="7f563-1431">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="7f563-1431">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-1432">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-1432">Az.Storage</span></span>
* <span data-ttu-id="7f563-1433">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="7f563-1433">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="7f563-1434">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="7f563-1434">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="7f563-1435">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="7f563-1435">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="7f563-1436">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-1436">New-AzStorageAccount</span></span>
* <span data-ttu-id="7f563-1437">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="7f563-1437">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="7f563-1438">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-1438">New-AzStorageAccount</span></span>
    - <span data-ttu-id="7f563-1439">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-1439">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="7f563-1440">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-1440">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f563-1441">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-1441">Az.Websites</span></span>
* <span data-ttu-id="7f563-1442">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="7f563-1442">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="7f563-1443">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="7f563-1443">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="7f563-1444">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-1444">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="7f563-1445">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="7f563-1445">Highlights since the last major release</span></span>
* <span data-ttu-id="7f563-1446">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="7f563-1446">General availability of `Az` module</span></span>
* <span data-ttu-id="7f563-1447">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="7f563-1447">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="7f563-1448">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="7f563-1448">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="7f563-1449">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1449">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="7f563-1450">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="7f563-1450">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="7f563-1451">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f563-1451">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="7f563-1452">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="7f563-1452">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="7f563-1453">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-1453">Az.Accounts</span></span>
* <span data-ttu-id="7f563-1454">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="7f563-1454">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="7f563-1455">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="7f563-1455">Az.Batch</span></span>
* <span data-ttu-id="7f563-1456">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1456">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="7f563-1457">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="7f563-1457">Az.Cdn</span></span>
* <span data-ttu-id="7f563-1458">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1458">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="7f563-1459">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1459">Az.CognitiveServices</span></span>
* <span data-ttu-id="7f563-1460">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1460">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-1461">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-1461">Az.Compute</span></span>
* <span data-ttu-id="7f563-1462">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="7f563-1462">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="7f563-1463">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1463">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="7f563-1464">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="7f563-1464">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="7f563-1465">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="7f563-1465">Az.DataFactory</span></span>
* <span data-ttu-id="7f563-1466">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="7f563-1466">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="7f563-1467">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f563-1467">Az.DataLakeStore</span></span>
* <span data-ttu-id="7f563-1468">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1468">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="7f563-1469">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="7f563-1469">Az.EventGrid</span></span>
* <span data-ttu-id="7f563-1470">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="7f563-1470">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="7f563-1471">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="7f563-1471">Az.EventHub</span></span>
* <span data-ttu-id="7f563-1472">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="7f563-1472">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="7f563-1473">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="7f563-1473">Az.HDInsight</span></span>
* <span data-ttu-id="7f563-1474">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1474">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="7f563-1475">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="7f563-1475">Az.IotHub</span></span>
* <span data-ttu-id="7f563-1476">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1476">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="7f563-1477">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7f563-1477">Az.KeyVault</span></span>
* <span data-ttu-id="7f563-1478">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1478">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="7f563-1479">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="7f563-1479">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="7f563-1480">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="7f563-1480">Az.MachineLearning</span></span>
* <span data-ttu-id="7f563-1481">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1481">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="7f563-1482">Az.Media</span><span class="sxs-lookup"><span data-stu-id="7f563-1482">Az.Media</span></span>
* <span data-ttu-id="7f563-1483">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1483">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="7f563-1484">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="7f563-1484">Az.Monitor</span></span>
  * <span data-ttu-id="7f563-1485">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="7f563-1485">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="7f563-1486">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="7f563-1486">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="7f563-1487">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="7f563-1487">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="7f563-1488">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="7f563-1488">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="7f563-1489">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="7f563-1489">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="7f563-1490">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="7f563-1490">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="7f563-1491">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="7f563-1491">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-1492">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1492">Az.Network</span></span>
* <span data-ttu-id="7f563-1493">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1493">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="7f563-1494">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="7f563-1494">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="7f563-1495">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="7f563-1495">Az.NotificationHubs</span></span>
* <span data-ttu-id="7f563-1496">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1496">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="7f563-1497">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="7f563-1497">Az.OperationalInsights</span></span>
* <span data-ttu-id="7f563-1498">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1498">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="7f563-1499">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="7f563-1499">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="7f563-1500">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1500">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-1501">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1501">Az.RecoveryServices</span></span>
* <span data-ttu-id="7f563-1502">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1502">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="7f563-1503">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="7f563-1503">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="7f563-1504">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="7f563-1504">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="7f563-1505">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="7f563-1505">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="7f563-1506">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="7f563-1506">Az.RedisCache</span></span>
* <span data-ttu-id="7f563-1507">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1507">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-1508">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-1508">Az.Resources</span></span>
* <span data-ttu-id="7f563-1509">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="7f563-1509">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-1510">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1510">Az.Sql</span></span>
* <span data-ttu-id="7f563-1511">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="7f563-1511">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="7f563-1512">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1512">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="7f563-1513">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="7f563-1513">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="7f563-1514">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="7f563-1514">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="7f563-1515">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="7f563-1515">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="7f563-1516">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="7f563-1516">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="7f563-1517">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="7f563-1517">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f563-1518">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-1518">Az.Websites</span></span>
* <span data-ttu-id="7f563-1519">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="7f563-1519">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="7f563-1520">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="7f563-1520">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="7f563-1521">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="7f563-1521">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="7f563-1522">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="7f563-1522">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="7f563-1523">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-1523">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="7f563-1524">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="7f563-1524">Highlights since the last major release</span></span>
* <span data-ttu-id="7f563-1525">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="7f563-1525">General availability of `Az` module</span></span>
* <span data-ttu-id="7f563-1526">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="7f563-1526">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="7f563-1527">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="7f563-1527">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="7f563-1528">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1528">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="7f563-1529">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="7f563-1529">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="7f563-1530">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f563-1530">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="7f563-1531">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="7f563-1531">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="7f563-1532">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-1532">Az.Accounts</span></span>
* <span data-ttu-id="7f563-1533">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="7f563-1533">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="7f563-1534">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1534">Az.AnalysisServices</span></span>
* <span data-ttu-id="7f563-1535">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="7f563-1535">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="7f563-1536">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="7f563-1536">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="7f563-1537">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f563-1537">Az.Automation</span></span>
* <span data-ttu-id="7f563-1538">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="7f563-1538">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="7f563-1539">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="7f563-1539">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="7f563-1540">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="7f563-1540">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-1541">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-1541">Az.Compute</span></span>
* <span data-ttu-id="7f563-1542">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-1542">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="7f563-1543">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="7f563-1543">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="7f563-1544">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="7f563-1544">Az.ContainerInstance</span></span>
* <span data-ttu-id="7f563-1545">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="7f563-1545">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="7f563-1546">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="7f563-1546">Az.DataFactory</span></span>
* <span data-ttu-id="7f563-1547">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="7f563-1547">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="7f563-1548">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7f563-1548">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-1549">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-1549">Az.Resources</span></span>
* <span data-ttu-id="7f563-1550">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="7f563-1550">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="7f563-1551">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="7f563-1551">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="7f563-1552">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="7f563-1552">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="7f563-1553">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="7f563-1553">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="7f563-1554">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="7f563-1554">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="7f563-1555">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="7f563-1555">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-1556">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1556">Az.Sql</span></span>
* <span data-ttu-id="7f563-1557">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="7f563-1557">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-1558">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-1558">Az.Storage</span></span>
* <span data-ttu-id="7f563-1559">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="7f563-1559">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="7f563-1560">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="7f563-1560">New-AzStorageContext</span></span>
* <span data-ttu-id="7f563-1561">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="7f563-1561">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="7f563-1562">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="7f563-1562">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="7f563-1563">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="7f563-1563">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="7f563-1564">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="7f563-1564">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="7f563-1565">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="7f563-1565">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="7f563-1566">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="7f563-1566">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="7f563-1567">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="7f563-1567">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="7f563-1568">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="7f563-1568">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="7f563-1569">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="7f563-1569">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="7f563-1570">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="7f563-1570">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="7f563-1571">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-1571">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="7f563-1572">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="7f563-1572">Highlights since the last major release</span></span>
* <span data-ttu-id="7f563-1573">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="7f563-1573">General availability of `Az` module</span></span>
* <span data-ttu-id="7f563-1574">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="7f563-1574">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="7f563-1575">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="7f563-1575">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="7f563-1576">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1576">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="7f563-1577">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="7f563-1577">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="7f563-1578">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f563-1578">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="7f563-1579">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="7f563-1579">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="7f563-1580">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f563-1580">Az.Automation</span></span>
* <span data-ttu-id="7f563-1581">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="7f563-1581">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="7f563-1582">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="7f563-1582">Dynamic grouping</span></span>
    * <span data-ttu-id="7f563-1583">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="7f563-1583">Pre-Post script</span></span>
    * <span data-ttu-id="7f563-1584">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="7f563-1584">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-1585">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-1585">Az.Compute</span></span>
* <span data-ttu-id="7f563-1586">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="7f563-1586">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="7f563-1587">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="7f563-1587">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="7f563-1588">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7f563-1588">Az.KeyVault</span></span>
* <span data-ttu-id="7f563-1589">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="7f563-1589">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-1590">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1590">Az.Network</span></span>
* <span data-ttu-id="7f563-1591">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="7f563-1591">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="7f563-1592">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="7f563-1592">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-1593">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1593">Az.RecoveryServices</span></span>
* <span data-ttu-id="7f563-1594">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="7f563-1594">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="7f563-1595">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="7f563-1595">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-1596">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-1596">Az.Resources</span></span>
* <span data-ttu-id="7f563-1597">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="7f563-1597">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="7f563-1598">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="7f563-1598">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-1599">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1599">Az.Sql</span></span>
* <span data-ttu-id="7f563-1600">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="7f563-1600">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-1601">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-1601">Az.Storage</span></span>
* <span data-ttu-id="7f563-1602">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7f563-1602">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="7f563-1603">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="7f563-1603">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="7f563-1604">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="7f563-1604">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="7f563-1605">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="7f563-1605">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="7f563-1606">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="7f563-1606">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="7f563-1607">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="7f563-1607">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="7f563-1608">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="7f563-1608">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f563-1609">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-1609">Az.Websites</span></span>
* <span data-ttu-id="7f563-1610">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="7f563-1610">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="7f563-1611">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-1611">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="7f563-1612">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-1612">Az.Accounts</span></span>
* <span data-ttu-id="7f563-1613">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="7f563-1613">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="7f563-1614">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-1614">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="7f563-1615">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f563-1615">Az.Automation</span></span>
* <span data-ttu-id="7f563-1616">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="7f563-1616">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="7f563-1617">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="7f563-1617">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="7f563-1618">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="7f563-1618">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="7f563-1619">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="7f563-1619">Az.Cdn</span></span>
* <span data-ttu-id="7f563-1620">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="7f563-1620">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-1621">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-1621">Az.Compute</span></span>
* <span data-ttu-id="7f563-1622">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="7f563-1622">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="7f563-1623">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="7f563-1623">Az.DataFactory</span></span>
* <span data-ttu-id="7f563-1624">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="7f563-1624">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="7f563-1625">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="7f563-1625">Az.LogicApp</span></span>
* <span data-ttu-id="7f563-1626">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="7f563-1626">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-1627">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1627">Az.Network</span></span>
* <span data-ttu-id="7f563-1628">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1628">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-1629">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1629">Az.RecoveryServices</span></span>
* <span data-ttu-id="7f563-1630">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="7f563-1630">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="7f563-1631">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="7f563-1631">SDK Update</span></span>
* <span data-ttu-id="7f563-1632">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="7f563-1632">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="7f563-1633">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="7f563-1633">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-1634">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-1634">Az.Resources</span></span>
* <span data-ttu-id="7f563-1635">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="7f563-1635">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="7f563-1636">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="7f563-1636">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="7f563-1637">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="7f563-1637">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="7f563-1638">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="7f563-1638">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="7f563-1639">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="7f563-1639">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="7f563-1640">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="7f563-1640">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-1641">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1641">Az.Sql</span></span>
* <span data-ttu-id="7f563-1642">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="7f563-1642">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="7f563-1643">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="7f563-1643">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-1644">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-1644">Az.Storage</span></span>
* <span data-ttu-id="7f563-1645">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-1645">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="7f563-1646">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-1646">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="7f563-1647">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1647">Az.AnalysisServices</span></span>
* <span data-ttu-id="7f563-1648">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="7f563-1648">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="7f563-1649">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f563-1649">Az.Automation</span></span>
* <span data-ttu-id="7f563-1650">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f563-1650">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="7f563-1651">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f563-1651">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="7f563-1652">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f563-1652">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="7f563-1653">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1653">Az.CognitiveServices</span></span>
* <span data-ttu-id="7f563-1654">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="7f563-1654">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-1655">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-1655">Az.Compute</span></span>
* <span data-ttu-id="7f563-1656">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="7f563-1656">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="7f563-1657">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="7f563-1657">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="7f563-1658">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="7f563-1658">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="7f563-1659">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="7f563-1659">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="7f563-1660">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f563-1660">Az.DataLakeStore</span></span>
* <span data-ttu-id="7f563-1661">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="7f563-1661">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="7f563-1662">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="7f563-1662">Az.EventHub</span></span>
* <span data-ttu-id="7f563-1663">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="7f563-1663">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="7f563-1664">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7f563-1664">Az.KeyVault</span></span>
* <span data-ttu-id="7f563-1665">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="7f563-1665">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="7f563-1666">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="7f563-1666">Az.LogicApp</span></span>
* <span data-ttu-id="7f563-1667">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="7f563-1667">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="7f563-1668">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="7f563-1668">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="7f563-1669">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="7f563-1669">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="7f563-1670">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="7f563-1670">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="7f563-1671">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="7f563-1671">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="7f563-1672">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="7f563-1672">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="7f563-1673">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="7f563-1673">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="7f563-1674">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="7f563-1674">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="7f563-1675">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f563-1675">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="7f563-1676">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f563-1676">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="7f563-1677">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f563-1677">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="7f563-1678">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f563-1678">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="7f563-1679">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="7f563-1679">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="7f563-1680">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="7f563-1680">Az.Monitor</span></span>
* <span data-ttu-id="7f563-1681">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="7f563-1681">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-1682">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1682">Az.Network</span></span>
* <span data-ttu-id="7f563-1683">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="7f563-1683">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="7f563-1684">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="7f563-1684">Az.OperationalInsights</span></span>
* <span data-ttu-id="7f563-1685">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="7f563-1685">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="7f563-1686">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="7f563-1686">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="7f563-1687">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="7f563-1687">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="7f563-1688">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-1688">Az.Resources</span></span>
* <span data-ttu-id="7f563-1689">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="7f563-1689">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="7f563-1690">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="7f563-1690">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="7f563-1691">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="7f563-1691">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="7f563-1692">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="7f563-1692">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-1693">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1693">Az.Sql</span></span>
* <span data-ttu-id="7f563-1694">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="7f563-1694">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="7f563-1695">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="7f563-1695">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f563-1696">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-1696">Az.Websites</span></span>
* <span data-ttu-id="7f563-1697">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="7f563-1697">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="7f563-1698">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-1698">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="7f563-1699">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-1699">Az.Accounts</span></span>
* <span data-ttu-id="7f563-1700">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="7f563-1700">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="7f563-1701">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1701">Az.AnalysisServices</span></span>
<span data-ttu-id="7f563-1702">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="7f563-1702">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-1703">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-1703">Az.Compute</span></span>
* <span data-ttu-id="7f563-1704">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="7f563-1704">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="7f563-1705">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="7f563-1705">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="7f563-1706">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="7f563-1706">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-1707">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1707">Az.RecoveryServices</span></span>
<span data-ttu-id="7f563-1708">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="7f563-1708">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-1709">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-1709">Az.Resources</span></span>
* <span data-ttu-id="7f563-1710">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="7f563-1710">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="7f563-1711">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="7f563-1711">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="7f563-1712">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="7f563-1712">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="7f563-1713">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="7f563-1713">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-1714">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1714">Az.Sql</span></span>
* <span data-ttu-id="7f563-1715">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="7f563-1715">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="7f563-1716">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="7f563-1716">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="7f563-1717">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="7f563-1717">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="7f563-1718">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-1718">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="7f563-1719">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-1719">Az.Accounts</span></span>
* <span data-ttu-id="7f563-1720">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="7f563-1720">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="7f563-1721">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1721">Az.AnalysisServices</span></span>
* <span data-ttu-id="7f563-1722">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="7f563-1722">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-1723">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1723">Az.RecoveryServices</span></span>
* <span data-ttu-id="7f563-1724">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="7f563-1724">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="7f563-1725">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-1725">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="7f563-1726">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-1726">Az.Accounts</span></span>
* <span data-ttu-id="7f563-1727">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="7f563-1727">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="7f563-1728">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="7f563-1728">Update incorrect online help URLs</span></span>
* <span data-ttu-id="7f563-1729">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="7f563-1729">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="7f563-1730">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="7f563-1730">Az.Aks</span></span>
* <span data-ttu-id="7f563-1731">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="7f563-1731">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="7f563-1732">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f563-1732">Az.Automation</span></span>
* <span data-ttu-id="7f563-1733">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="7f563-1733">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="7f563-1734">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="7f563-1734">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="7f563-1735">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="7f563-1735">Az.Cdn</span></span>
* <span data-ttu-id="7f563-1736">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="7f563-1736">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-1737">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-1737">Az.Compute</span></span>
* <span data-ttu-id="7f563-1738">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="7f563-1738">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="7f563-1739">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="7f563-1739">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="7f563-1740">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="7f563-1740">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="7f563-1741">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="7f563-1741">Az.ContainerRegistry</span></span>
* <span data-ttu-id="7f563-1742">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="7f563-1742">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="7f563-1743">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="7f563-1743">Az.DataFactory</span></span>
* <span data-ttu-id="7f563-1744">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="7f563-1744">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="7f563-1745">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f563-1745">Az.DataLakeStore</span></span>
* <span data-ttu-id="7f563-1746">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="7f563-1746">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="7f563-1747">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="7f563-1747">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="7f563-1748">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="7f563-1748">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="7f563-1749">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="7f563-1749">Az.IotHub</span></span>
* <span data-ttu-id="7f563-1750">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="7f563-1750">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="7f563-1751">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7f563-1751">Az.KeyVault</span></span>
* <span data-ttu-id="7f563-1752">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="7f563-1752">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-1753">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1753">Az.Network</span></span>
* <span data-ttu-id="7f563-1754">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="7f563-1754">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-1755">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-1755">Az.Resources</span></span>
* <span data-ttu-id="7f563-1756">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="7f563-1756">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="7f563-1757">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="7f563-1757">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="7f563-1758">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="7f563-1758">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="7f563-1759">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="7f563-1759">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="7f563-1760">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="7f563-1760">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="7f563-1761">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="7f563-1761">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="7f563-1762">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="7f563-1762">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="7f563-1763">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7f563-1763">Az.ServiceFabric</span></span>
* <span data-ttu-id="7f563-1764">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="7f563-1764">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="7f563-1765">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="7f563-1765">Fix some error messages.</span></span>
* <span data-ttu-id="7f563-1766">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="7f563-1766">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="7f563-1767">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="7f563-1767">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="7f563-1768">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="7f563-1768">Az.SignalR</span></span>
* <span data-ttu-id="7f563-1769">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="7f563-1769">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-1770">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1770">Az.Sql</span></span>
* <span data-ttu-id="7f563-1771">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="7f563-1771">Update incorrect online help URLs</span></span>
* <span data-ttu-id="7f563-1772">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="7f563-1772">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="7f563-1773">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="7f563-1773">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="7f563-1774">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="7f563-1774">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-1775">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-1775">Az.Storage</span></span>
* <span data-ttu-id="7f563-1776">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="7f563-1776">Update incorrect online help URLs</span></span>
* <span data-ttu-id="7f563-1777">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="7f563-1777">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="7f563-1778">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="7f563-1778">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="7f563-1779">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="7f563-1779">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="7f563-1780">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="7f563-1780">Az.TrafficManager</span></span>
* <span data-ttu-id="7f563-1781">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="7f563-1781">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f563-1782">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-1782">Az.Websites</span></span>
* <span data-ttu-id="7f563-1783">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="7f563-1783">Update incorrect online help URLs</span></span>
* <span data-ttu-id="7f563-1784">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="7f563-1784">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="7f563-1785">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="7f563-1785">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="7f563-1786">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="7f563-1786">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="7f563-1787">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-1787">Az.Accounts</span></span>
* <span data-ttu-id="7f563-1788">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="7f563-1788">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-1789">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-1789">Az.Compute</span></span>
* <span data-ttu-id="7f563-1790">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="7f563-1790">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="7f563-1791">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="7f563-1791">Updated the description of ID in help files</span></span>
* <span data-ttu-id="7f563-1792">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-1792">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="7f563-1793">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f563-1793">Az.DataLakeStore</span></span>
* <span data-ttu-id="7f563-1794">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="7f563-1794">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="7f563-1795">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="7f563-1795">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="7f563-1796">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="7f563-1796">Az.EventGrid</span></span>
* <span data-ttu-id="7f563-1797">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="7f563-1797">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="7f563-1798">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="7f563-1798">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="7f563-1799">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="7f563-1799">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="7f563-1800">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="7f563-1800">Event Time-To-Live,</span></span>
        - <span data-ttu-id="7f563-1801">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="7f563-1801">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="7f563-1802">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="7f563-1802">Dead letter endpoint.</span></span>
    - <span data-ttu-id="7f563-1803">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="7f563-1803">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="7f563-1804">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="7f563-1804">Event Time-To-Live,</span></span>
        - <span data-ttu-id="7f563-1805">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="7f563-1805">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="7f563-1806">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="7f563-1806">Dead letter endpoint.</span></span>
* <span data-ttu-id="7f563-1807">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="7f563-1807">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="7f563-1808">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="7f563-1808">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="7f563-1809">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="7f563-1809">Az.IotHub</span></span>
* <span data-ttu-id="7f563-1810">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="7f563-1810">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="7f563-1811">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="7f563-1811">Az.LogicApp</span></span>
* <span data-ttu-id="7f563-1812">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="7f563-1812">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-1813">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-1813">Az.Resources</span></span>
* <span data-ttu-id="7f563-1814">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="7f563-1814">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="7f563-1815">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="7f563-1815">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="7f563-1816">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="7f563-1816">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="7f563-1817">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="7f563-1817">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="7f563-1818">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="7f563-1818">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="7f563-1819">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="7f563-1819">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="7f563-1820">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="7f563-1820">Az.SignalR</span></span>
* <span data-ttu-id="7f563-1821">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-1821">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-1822">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1822">Az.Sql</span></span>
* <span data-ttu-id="7f563-1823">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="7f563-1823">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="7f563-1824">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-1824">Az.Storage</span></span>
* <span data-ttu-id="7f563-1825">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="7f563-1825">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="7f563-1826">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="7f563-1826">New-AzStorageContext</span></span>
* <span data-ttu-id="7f563-1827">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="7f563-1827">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="7f563-1828">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="7f563-1828">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f563-1829">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-1829">Az.Websites</span></span>
* <span data-ttu-id="7f563-1830">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="7f563-1830">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="7f563-1831">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-1831">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="7f563-1832">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7f563-1832">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="7f563-1833">Geral</span><span class="sxs-lookup"><span data-stu-id="7f563-1833">General</span></span>

- <span data-ttu-id="7f563-1834">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="7f563-1834">General Availability of Az Module</span></span>
- <span data-ttu-id="7f563-1835">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="7f563-1835">Online help for each module</span></span>
- <span data-ttu-id="7f563-1836">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="7f563-1836">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="7f563-1837">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="7f563-1837">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="7f563-1838">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-1838">Az.Accounts</span></span>
- <span data-ttu-id="7f563-1839">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="7f563-1839">Changed from Az.Profile</span></span>
- <span data-ttu-id="7f563-1840">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="7f563-1840">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="7f563-1841">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7f563-1841">Az.ApiManagement</span></span>
- <span data-ttu-id="7f563-1842">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="7f563-1842">Fixes for #7002</span></span>
- <span data-ttu-id="7f563-1843">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="7f563-1843">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="7f563-1844">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="7f563-1844">Az.Batch</span></span>
- <span data-ttu-id="7f563-1845">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="7f563-1845">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="7f563-1846">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="7f563-1846">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="7f563-1847">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="7f563-1847">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="7f563-1848">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="7f563-1848">Az.Billing</span></span>
- <span data-ttu-id="7f563-1849">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="7f563-1849">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="7f563-1850">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1850">Az.CognitivServices</span></span>
- <span data-ttu-id="7f563-1851">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-1851">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="7f563-1852">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="7f563-1852">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="7f563-1853">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="7f563-1853">Az.ContainerInstance</span></span>
- <span data-ttu-id="7f563-1854">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="7f563-1854">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="7f563-1855">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="7f563-1855">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="7f563-1856">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="7f563-1856">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="7f563-1857">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f563-1857">Az.DataLakeStore</span></span>
- <span data-ttu-id="7f563-1858">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="7f563-1858">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="7f563-1859">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="7f563-1859">Az.Monitor</span></span>
- <span data-ttu-id="7f563-1860">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="7f563-1860">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="7f563-1861">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7f563-1861">Az.KeyVault</span></span>
- <span data-ttu-id="7f563-1862">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="7f563-1862">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="7f563-1863">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="7f563-1863">Az.MachineLearning</span></span>
- <span data-ttu-id="7f563-1864">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="7f563-1864">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="7f563-1865">Az.Media</span><span class="sxs-lookup"><span data-stu-id="7f563-1865">Az.Media</span></span>
- <span data-ttu-id="7f563-1866">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="7f563-1866">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="7f563-1867">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1867">Az.Network</span></span>
<span data-ttu-id="7f563-1868">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="7f563-1868">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="7f563-1869">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7f563-1869">New cmdlets added:</span></span>
        - <span data-ttu-id="7f563-1870">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="7f563-1870">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="7f563-1871">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="7f563-1871">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="7f563-1872">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="7f563-1872">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="7f563-1873">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="7f563-1873">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="7f563-1874">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="7f563-1874">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="7f563-1875">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="7f563-1875">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="7f563-1876">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="7f563-1876">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="7f563-1877">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f563-1877">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="7f563-1878">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="7f563-1878">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="7f563-1879">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="7f563-1879">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="7f563-1880">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="7f563-1880">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="7f563-1881">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="7f563-1881">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="7f563-1882">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-1882">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="7f563-1883">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-1883">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="7f563-1884">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="7f563-1884">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="7f563-1885">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="7f563-1885">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="7f563-1886">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="7f563-1886">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="7f563-1887">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="7f563-1887">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="7f563-1888">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="7f563-1888">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="7f563-1889">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="7f563-1889">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="7f563-1890">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="7f563-1890">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="7f563-1891">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="7f563-1891">Az.OperationalInsights</span></span>
- <span data-ttu-id="7f563-1892">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="7f563-1892">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="7f563-1893">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="7f563-1893">Az.Profile</span></span>
- <span data-ttu-id="7f563-1894">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f563-1894">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-1895">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1895">Az.RecoveryServices</span></span>
- <span data-ttu-id="7f563-1896">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="7f563-1896">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="7f563-1897">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-1897">Az.Resources</span></span>
- <span data-ttu-id="7f563-1898">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="7f563-1898">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="7f563-1899">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7f563-1899">Az.ServiceFabric</span></span>
- <span data-ttu-id="7f563-1900">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="7f563-1900">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="7f563-1901">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="7f563-1901">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="7f563-1902">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="7f563-1902">Az.SIgnalR</span></span>
- <span data-ttu-id="7f563-1903">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="7f563-1903">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="7f563-1904">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1904">Az.Sql</span></span>
- <span data-ttu-id="7f563-1905">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="7f563-1905">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="7f563-1906">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="7f563-1906">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="7f563-1907">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="7f563-1907">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="7f563-1908">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-1908">Az.Storage</span></span>
- <span data-ttu-id="7f563-1909">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="7f563-1909">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="7f563-1910">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-1910">Az.Websites</span></span>
- <span data-ttu-id="7f563-1911">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="7f563-1911">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="7f563-1912">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7f563-1912">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="7f563-1913">Geral</span><span class="sxs-lookup"><span data-stu-id="7f563-1913">General</span></span>

* <span data-ttu-id="7f563-1914">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="7f563-1914">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="7f563-1915">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-1915">Az.Compute</span></span>

* <span data-ttu-id="7f563-1916">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="7f563-1916">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="7f563-1917">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f563-1917">Az.DataLakeStore</span></span>

* <span data-ttu-id="7f563-1918">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="7f563-1918">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="7f563-1919">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="7f563-1919">Az.FrontDoor</span></span>

* <span data-ttu-id="7f563-1920">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="7f563-1920">Fixed some broken links</span></span>
    - <span data-ttu-id="7f563-1921">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="7f563-1921">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="7f563-1922">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="7f563-1922">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="7f563-1923">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f563-1923">Az.RecoveryServices</span></span>

* <span data-ttu-id="7f563-1924">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-1924">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="7f563-1925">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="7f563-1925">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="7f563-1926">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-1926">Az.Resources</span></span>

* <span data-ttu-id="7f563-1927">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="7f563-1927">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="7f563-1928">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="7f563-1928">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="7f563-1929">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1929">Az.Sql</span></span>

* <span data-ttu-id="7f563-1930">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="7f563-1930">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="7f563-1931">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="7f563-1931">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="7f563-1932">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="7f563-1932">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="7f563-1933">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-1933">Az.Storage</span></span>

* <span data-ttu-id="7f563-1934">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="7f563-1934">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="7f563-1935">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="7f563-1935">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="7f563-1936">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="7f563-1936">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="7f563-1937">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="7f563-1937">Support Static Website configuration</span></span>
    - <span data-ttu-id="7f563-1938">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="7f563-1938">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="7f563-1939">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="7f563-1939">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="7f563-1940">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-1940">Az.Websites</span></span>

* <span data-ttu-id="7f563-1941">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="7f563-1941">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="7f563-1942">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="7f563-1942">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="7f563-1943">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-1943">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="7f563-1944">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7f563-1944">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="7f563-1945">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7f563-1945">Az.ApiManagement</span></span>
* <span data-ttu-id="7f563-1946">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="7f563-1946">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="7f563-1947">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f563-1947">Az.Automation</span></span>
* <span data-ttu-id="7f563-1948">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="7f563-1948">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="7f563-1949">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="7f563-1949">Added Update Management cmdlets</span></span>
* <span data-ttu-id="7f563-1950">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="7f563-1950">Added Source Control cmdlets</span></span>
* <span data-ttu-id="7f563-1951">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="7f563-1951">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="7f563-1952">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="7f563-1952">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="7f563-1953">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-1953">Az.Compute</span></span>
* <span data-ttu-id="7f563-1954">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="7f563-1954">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="7f563-1955">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="7f563-1955">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="7f563-1956">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="7f563-1956">Az.ContainerInstance</span></span>
* <span data-ttu-id="7f563-1957">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="7f563-1957">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="7f563-1958">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="7f563-1958">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="7f563-1959">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="7f563-1959">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="7f563-1960">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-1960">Az.Network</span></span>
* <span data-ttu-id="7f563-1961">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="7f563-1961">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="7f563-1962">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="7f563-1962">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="7f563-1963">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="7f563-1963">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="7f563-1964">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="7f563-1964">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="7f563-1965">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="7f563-1965">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="7f563-1966">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="7f563-1966">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="7f563-1967">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="7f563-1967">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="7f563-1968">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="7f563-1968">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="7f563-1969">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="7f563-1969">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="7f563-1970">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="7f563-1970">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="7f563-1971">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="7f563-1971">Az.Relay</span></span>
* <span data-ttu-id="7f563-1972">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="7f563-1972">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="7f563-1973">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-1973">Az.Resources</span></span>
* <span data-ttu-id="7f563-1974">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="7f563-1974">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="7f563-1975">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="7f563-1975">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="7f563-1976">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="7f563-1976">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="7f563-1977">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7f563-1977">Az.ServiceFabric</span></span>
* <span data-ttu-id="7f563-1978">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="7f563-1978">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="7f563-1979">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-1979">Az.Sql</span></span>
* <span data-ttu-id="7f563-1980">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="7f563-1980">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="7f563-1981">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="7f563-1981">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="7f563-1982">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="7f563-1982">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="7f563-1983">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="7f563-1983">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="7f563-1984">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="7f563-1984">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="7f563-1985">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="7f563-1985">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="7f563-1986">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="7f563-1986">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="7f563-1987">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="7f563-1987">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="7f563-1988">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="7f563-1988">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="7f563-1989">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="7f563-1989">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="7f563-1990">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="7f563-1990">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="7f563-1991">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="7f563-1991">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="7f563-1992">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="7f563-1992">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="7f563-1993">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="7f563-1993">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="7f563-1994">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="7f563-1994">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="7f563-1995">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="7f563-1995">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="7f563-1996">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="7f563-1996">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="7f563-1997">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7f563-1997">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="7f563-1998">Geral</span><span class="sxs-lookup"><span data-stu-id="7f563-1998">General</span></span>
* <span data-ttu-id="7f563-1999">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="7f563-1999">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="7f563-2000">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="7f563-2000">Az.Profile</span></span>
* <span data-ttu-id="7f563-2001">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="7f563-2001">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="7f563-2002">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="7f563-2002">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="7f563-2003">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="7f563-2003">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="7f563-2004">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="7f563-2004">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="7f563-2005">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="7f563-2005">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="7f563-2006">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="7f563-2006">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="7f563-2007">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="7f563-2007">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="7f563-2008">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7f563-2008">Az.CognitiveServices</span></span>
* <span data-ttu-id="7f563-2009">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="7f563-2009">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-2010">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-2010">Az.Compute</span></span>
* <span data-ttu-id="7f563-2011">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="7f563-2011">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="7f563-2012">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="7f563-2012">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="7f563-2013">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="7f563-2013">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="7f563-2014">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f563-2014">Az.DataLakeStore</span></span>
* <span data-ttu-id="7f563-2015">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="7f563-2015">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="7f563-2016">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="7f563-2016">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="7f563-2017">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="7f563-2017">Az.Insights</span></span>
* <span data-ttu-id="7f563-2018">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="7f563-2018">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="7f563-2019">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="7f563-2019">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="7f563-2020">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="7f563-2020">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="7f563-2021">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="7f563-2021">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-2022">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-2022">Az.Network</span></span>
* <span data-ttu-id="7f563-2023">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="7f563-2023">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="7f563-2024">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="7f563-2024">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="7f563-2025">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="7f563-2025">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="7f563-2026">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="7f563-2026">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="7f563-2027">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="7f563-2027">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="7f563-2028">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="7f563-2028">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="7f563-2029">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="7f563-2029">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="7f563-2030">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="7f563-2030">Az.PolicyInsights</span></span>
* <span data-ttu-id="7f563-2031">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="7f563-2031">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-2032">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-2032">Az.Resources</span></span>
* <span data-ttu-id="7f563-2033">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="7f563-2033">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="7f563-2034">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="7f563-2034">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="7f563-2035">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7f563-2035">Az.ServiceBus</span></span>
* <span data-ttu-id="7f563-2036">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="7f563-2036">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="7f563-2037">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7f563-2037">Az.ServiceFabric</span></span>
* <span data-ttu-id="7f563-2038">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="7f563-2038">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="7f563-2039">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="7f563-2039">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="7f563-2040">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="7f563-2040">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="7f563-2041">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="7f563-2041">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="7f563-2042">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="7f563-2042">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="7f563-2043">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="7f563-2043">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="7f563-2044">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="7f563-2044">Az.Profile</span></span>
* <span data-ttu-id="7f563-2045">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="7f563-2045">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="7f563-2046">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="7f563-2046">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-2047">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-2047">Az.Compute</span></span>
* <span data-ttu-id="7f563-2048">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="7f563-2048">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="7f563-2049">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="7f563-2049">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="7f563-2050">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f563-2050">Az.DataLakeStore</span></span>
* <span data-ttu-id="7f563-2051">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="7f563-2051">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="7f563-2052">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-2052">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="7f563-2053">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="7f563-2053">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="7f563-2054">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="7f563-2054">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="7f563-2055">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="7f563-2055">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-2056">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-2056">Az.Network</span></span>
* <span data-ttu-id="7f563-2057">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="7f563-2057">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="7f563-2058">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="7f563-2058">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-2059">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-2059">Az.Resources</span></span>
* <span data-ttu-id="7f563-2060">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="7f563-2060">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="7f563-2061">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="7f563-2061">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="7f563-2062">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="7f563-2062">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="7f563-2063">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="7f563-2063">Azure.Storage</span></span>
* <span data-ttu-id="7f563-2064">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="7f563-2064">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="7f563-2065">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="7f563-2065">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="7f563-2066">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="7f563-2066">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="7f563-2067">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="7f563-2067">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="7f563-2068">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="7f563-2068">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="7f563-2069">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7f563-2069">Az.CognitiveServices</span></span>
* <span data-ttu-id="7f563-2070">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="7f563-2070">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f563-2071">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f563-2071">Az.Compute</span></span>
* <span data-ttu-id="7f563-2072">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="7f563-2072">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="7f563-2073">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="7f563-2073">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="7f563-2074">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="7f563-2074">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="7f563-2075">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="7f563-2075">Az.DataFactoryV2</span></span>
* <span data-ttu-id="7f563-2076">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="7f563-2076">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f563-2077">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f563-2077">Az.Network</span></span>
* <span data-ttu-id="7f563-2078">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="7f563-2078">Added NetworkProfile functionality.</span></span> <span data-ttu-id="7f563-2079">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="7f563-2079">new cmdlets added</span></span>
    - <span data-ttu-id="7f563-2080">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="7f563-2080">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="7f563-2081">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="7f563-2081">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="7f563-2082">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="7f563-2082">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="7f563-2083">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="7f563-2083">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="7f563-2084">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-2084">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="7f563-2085">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-2085">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="7f563-2086">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="7f563-2086">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="7f563-2087">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="7f563-2087">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="7f563-2088">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="7f563-2088">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="7f563-2089">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="7f563-2089">Az.RedisCache</span></span>
* <span data-ttu-id="7f563-2090">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="7f563-2090">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="7f563-2091">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="7f563-2091">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f563-2092">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f563-2092">Az.Resources</span></span>
* <span data-ttu-id="7f563-2093">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="7f563-2093">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="7f563-2094">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="7f563-2094">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f563-2095">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f563-2095">Az.Sql</span></span>
* <span data-ttu-id="7f563-2096">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="7f563-2096">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f563-2097">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f563-2097">Az.Websites</span></span>
* <span data-ttu-id="7f563-2098">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="7f563-2098">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="7f563-2099">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="7f563-2099">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="7f563-2100">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7f563-2100">0.2.0 - September 2018</span></span>
 <span data-ttu-id="7f563-2101">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="7f563-2101">Initial Release</span></span>
