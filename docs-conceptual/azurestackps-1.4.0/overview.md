# <a name="azure-stack-module-140"></a><span data-ttu-id="8b066-101">Azure Stack Module 1.4.0</span><span class="sxs-lookup"><span data-stu-id="8b066-101">Azure Stack Module 1.4.0</span></span>

## <a name="requirements"></a><span data-ttu-id="8b066-102">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="8b066-102">Requirements:</span></span>
<span data-ttu-id="8b066-103">A versão mínima suportada do Azure Stack é a 1804.</span><span class="sxs-lookup"><span data-stu-id="8b066-103">Minimum supported Azure Stack version is 1804.</span></span>

<span data-ttu-id="8b066-104">Nota: Se estiver a utilizar uma versão anterior, instale a versão 1.2.11</span><span class="sxs-lookup"><span data-stu-id="8b066-104">Note: If you are using an earlier version install version 1.2.11</span></span>

## <a name="known-issues"></a><span data-ttu-id="8b066-105">Problemas conhecidos:</span><span class="sxs-lookup"><span data-stu-id="8b066-105">Known issues:</span></span>

- <span data-ttu-id="8b066-106">Fechar Alerta requer a versão 1803 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="8b066-106">Close Alert requires Azure Stack version 1803</span></span>
- <span data-ttu-id="8b066-107">O New-AzsOffer não permite criar uma oferta com o estado público.</span><span class="sxs-lookup"><span data-stu-id="8b066-107">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="8b066-108">O cmdlet Set-AzsOffer tem de ser chamado depois para alterar o estado.</span><span class="sxs-lookup"><span data-stu-id="8b066-108">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="8b066-109">Não é possível remover um Conjunto IP sem uma reimplementação</span><span class="sxs-lookup"><span data-stu-id="8b066-109">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="breaking-changes"></a><span data-ttu-id="8b066-110">Alterações Interruptivas</span><span class="sxs-lookup"><span data-stu-id="8b066-110">Breaking Changes</span></span>
<span data-ttu-id="8b066-111">Não há nenhuma alteração interruptiva a partir da versão 1.3.0.</span><span class="sxs-lookup"><span data-stu-id="8b066-111">There are no breaking changes from the version 1.3.0.</span></span> <span data-ttu-id="8b066-112">Todas as alterações interruptivas migradas da versão 1.2.11 estão documentadas aqui https://aka.ms/azspowershellmigration</span><span class="sxs-lookup"><span data-stu-id="8b066-112">All breaking changes migrating from 1.2.11 are documented here https://aka.ms/azspowershellmigration</span></span>

## <a name="install"></a><span data-ttu-id="8b066-113">Instalar</span><span class="sxs-lookup"><span data-stu-id="8b066-113">Install</span></span>
```
# Remove previous versions of AzureStack modules
Uninstall-Module -Name AzureStack -Force 
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Get-Module Azs.* -ListAvailable | Uninstall-Module -Force


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2017-03-09-profile -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.4.0
```
## <a name="release-notes"></a><span data-ttu-id="8b066-114">Notas de Versão</span><span class="sxs-lookup"><span data-stu-id="8b066-114">Release Notes</span></span>
    * <span data-ttu-id="8b066-115">A versão 1.4.0 do Azurestack não tem alterações interruptivas a partir da versão 1.3.0</span><span class="sxs-lookup"><span data-stu-id="8b066-115">Azurestack 1.4.0 version has no breaking changes from the previous release 1.3.0</span></span>
    * <span data-ttu-id="8b066-116">Azs.AzureBridge.Admin</span><span class="sxs-lookup"><span data-stu-id="8b066-116">Azs.AzureBridge.Admin</span></span>
        - <span data-ttu-id="8b066-117">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="8b066-117">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="8b066-118">Azs.Backup.Admin</span><span class="sxs-lookup"><span data-stu-id="8b066-118">Azs.Backup.Admin</span></span>
        - <span data-ttu-id="8b066-119">Adicionados os novos parâmetros BackupFrequencyInHours, IsBackupSchedulerEnabled, BackupRetentionPeriodInDays no cmdlet Set-AzsBackupShare</span><span class="sxs-lookup"><span data-stu-id="8b066-119">Added new parameters BackupFrequencyInHours, IsBackupSchedulerEnabled, BackupRetentionPeriodInDays in cmdlet Set-AzsBackupShare</span></span>
        - <span data-ttu-id="8b066-120">Adicionado um cmdlet New-EncyptionKeyBase64 para facilitar a criação da chave de encriptação</span><span class="sxs-lookup"><span data-stu-id="8b066-120">Added a cmdlet New-EncyptionKeyBase64 to facilitate creating encryption key</span></span>
        - <span data-ttu-id="8b066-121">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="8b066-121">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="8b066-122">Azs.Commerce.Admin</span><span class="sxs-lookup"><span data-stu-id="8b066-122">Azs.Commerce.Admin</span></span>
        - <span data-ttu-id="8b066-123">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="8b066-123">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="8b066-124">Azs.Fabric.Admin</span><span class="sxs-lookup"><span data-stu-id="8b066-124">Azs.Fabric.Admin</span></span>
        - <span data-ttu-id="8b066-125">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="8b066-125">Fix for the bug that returned only a single page in paginated results</span></span>
        - <span data-ttu-id="8b066-126">Adicionado um cmdlet Add-AzsScaleUnitNode para permitir ao administrador adicionar novos nós de unidade de escala ao carimbo de azurestack</span><span class="sxs-lookup"><span data-stu-id="8b066-126">Added a cmdlet Add-AzsScaleUnitNode to enable admin to add new scale unit nodes to the azurestack stamp</span></span>
        - <span data-ttu-id="8b066-127">Adicionado o cmdlet e New-AzsScaleUnitNodeObject para facilitar os objetos de parâmetro de unidade de escala de criação</span><span class="sxs-lookup"><span data-stu-id="8b066-127">Added cmdlet and New-AzsScaleUnitNodeObject to facilitate the creation scale unit parameter objects</span></span>
    * <span data-ttu-id="8b066-128">Azs.Gallery.Admin</span><span class="sxs-lookup"><span data-stu-id="8b066-128">Azs.Gallery.Admin</span></span>
        - <span data-ttu-id="8b066-129">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="8b066-129">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="8b066-130">Azs.InfrastructureInsights.Admin</span><span class="sxs-lookup"><span data-stu-id="8b066-130">Azs.InfrastructureInsights.Admin</span></span>
        - <span data-ttu-id="8b066-131">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="8b066-131">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="8b066-132">Azs.Network.Admin</span><span class="sxs-lookup"><span data-stu-id="8b066-132">Azs.Network.Admin</span></span>
        - <span data-ttu-id="8b066-133">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="8b066-133">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="8b066-134">Azs.Update.Admin</span><span class="sxs-lookup"><span data-stu-id="8b066-134">Azs.Update.Admin</span></span>
        - <span data-ttu-id="8b066-135">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="8b066-135">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="8b066-136">Azs.Subscriptions</span><span class="sxs-lookup"><span data-stu-id="8b066-136">Azs.Subscriptions</span></span>
        - <span data-ttu-id="8b066-137">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="8b066-137">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="8b066-138">Azs.Subscriptions.Admin</span><span class="sxs-lookup"><span data-stu-id="8b066-138">Azs.Subscriptions.Admin</span></span>
        - <span data-ttu-id="8b066-139">Foi adicionado um cmdlet Move-AzsSubscription para mover subscrições entre ofertas de fornecedores delegados</span><span class="sxs-lookup"><span data-stu-id="8b066-139">Added a cmdlet Move-AzsSubscription to move subscriptions between delegated provider offers</span></span>
        - <span data-ttu-id="8b066-140">Adicionado um cmdlet Test-AzsMoveSubscription para validar que as subscrições do utilizador podem ser movidos entre as ofertas de fornecedor delegado</span><span class="sxs-lookup"><span data-stu-id="8b066-140">Added a cmdlet Test-AzsMoveSubscription to validate that user subscriptions can be moved between delegated provider offers</span></span>
        - <span data-ttu-id="8b066-141">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="8b066-141">Fix for the bug that returned only a single page in paginated results'</span></span>

## <a name="content"></a><span data-ttu-id="8b066-142">Conteúdo:</span><span class="sxs-lookup"><span data-stu-id="8b066-142">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="8b066-143">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="8b066-143">Azure Bridge</span></span>
<span data-ttu-id="8b066-144">Versão de pré-visualização do módulo de administrador AzureBridge do Azure Stack que lhe permite sindicar imagens a partir do Azure.</span><span class="sxs-lookup"><span data-stu-id="8b066-144">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="8b066-145">Cópia de segurança</span><span class="sxs-lookup"><span data-stu-id="8b066-145">Backup</span></span>
<span data-ttu-id="8b066-146">Versão de pré-visualização do módulo de administrador Cópia de Segurança que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="8b066-146">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="8b066-147">Configurar em que local as cópias de segurança são armazenadas</span><span class="sxs-lookup"><span data-stu-id="8b066-147">Configure where backups are stored</span></span>
- <span data-ttu-id="8b066-148">Fazer cópias de segurança</span><span class="sxs-lookup"><span data-stu-id="8b066-148">Perform backups</span></span>
- <span data-ttu-id="8b066-149">Listar e restaurar cópias de segurança concluídas</span><span class="sxs-lookup"><span data-stu-id="8b066-149">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="8b066-150">Comércio</span><span class="sxs-lookup"><span data-stu-id="8b066-150">Commerce</span></span>
<span data-ttu-id="8b066-151">Versão de pré-visualização do módulo de administrador Comércio do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8b066-151">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="8b066-152">Computação</span><span class="sxs-lookup"><span data-stu-id="8b066-152">Compute</span></span>
<span data-ttu-id="8b066-153">Versão de pré-visualização do módulo de administrador Computação do Azure Stack que fornece funcionalidade que permite gerir quotas de computação, imagens de plataforma e extensões de máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="8b066-153">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="8b066-154">Recursos de infraestrutura</span><span class="sxs-lookup"><span data-stu-id="8b066-154">Fabric</span></span>
<span data-ttu-id="8b066-155">Versão de pré-visualização do módulo de administrador Recursos de infraestrutura do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack:</span><span class="sxs-lookup"><span data-stu-id="8b066-155">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="8b066-156">Parar, Iniciar e Encerrar nós de unidade de escala</span><span class="sxs-lookup"><span data-stu-id="8b066-156">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="8b066-157">Drenar e Retomar nós de unidade de escala para atividades relacionadas com FRU</span><span class="sxs-lookup"><span data-stu-id="8b066-157">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="8b066-158">Reparar nós de unidade de escala</span><span class="sxs-lookup"><span data-stu-id="8b066-158">Repair of scale unit nodes</span></span>
- <span data-ttu-id="8b066-159">Reiniciar a função Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="8b066-159">Restart of Infrastructure role</span></span>
- <span data-ttu-id="8b066-160">Parar, Iniciar e Encerrar instâncias de função Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="8b066-160">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="8b066-161">Criar novos Conjuntos IP</span><span class="sxs-lookup"><span data-stu-id="8b066-161">Create new IP Pools</span></span>

### <a name="gallery"></a><span data-ttu-id="8b066-162">Galeria</span><span class="sxs-lookup"><span data-stu-id="8b066-162">Gallery</span></span>
<span data-ttu-id="8b066-163">Versão de pré-visualização do módulo de administrador Galeria do Azure Stack que fornece funcionalidade que permite gerir itens da galeria no marketplace do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8b066-163">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="8b066-164">Informações de Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="8b066-164">Infrastructure Insights</span></span>
<span data-ttu-id="8b066-165">Versão de pré-visualização do módulo de administrador Informações de Infraestrutura que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="8b066-165">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="8b066-166">Ver o estado de funcionamento dos recursos de carimbo do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="8b066-166">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="8b066-167">Ver e gerir alertas</span><span class="sxs-lookup"><span data-stu-id="8b066-167">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="8b066-168">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8b066-168">KeyVault</span></span>
<span data-ttu-id="8b066-169">Versão de pré-visualização do módulo de administrador KeyVault do Azure Stack que permite ao administrador ver as quotas do KeyVault.</span><span class="sxs-lookup"><span data-stu-id="8b066-169">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="8b066-170">Rede</span><span class="sxs-lookup"><span data-stu-id="8b066-170">Network</span></span>
<span data-ttu-id="8b066-171">Versão de pré-visualização do módulo de administrador Rede que permite:</span><span class="sxs-lookup"><span data-stu-id="8b066-171">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="8b066-172">Gerir quotas de rede</span><span class="sxs-lookup"><span data-stu-id="8b066-172">Management of network quotas</span></span>
- <span data-ttu-id="8b066-173">Ver recursos de rede alocados, como endereços IP públicos, redes virtuais, balanceadores de carga</span><span class="sxs-lookup"><span data-stu-id="8b066-173">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="8b066-174">Fornece um cmdlet que apresenta uma descrição geral de administrador</span><span class="sxs-lookup"><span data-stu-id="8b066-174">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="8b066-175">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8b066-175">Storage</span></span>
<span data-ttu-id="8b066-176">Versão de pré-visualização do módulo de administrador Armazenamento do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8b066-176">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="8b066-177">Nesta versão, fornecemos funcionalidade para:</span><span class="sxs-lookup"><span data-stu-id="8b066-177">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="8b066-178">Gerir quotas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="8b066-178">Manage storage quotas</span></span>
- <span data-ttu-id="8b066-179">Libertar memória de recursos de armazenamento eliminados</span><span class="sxs-lookup"><span data-stu-id="8b066-179">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="8b066-180">Restaurar contas de armazenamento eliminadas</span><span class="sxs-lookup"><span data-stu-id="8b066-180">Restore deleted storage accounts</span></span>
- <span data-ttu-id="8b066-181">Migrar contentores de uma partilha para outra</span><span class="sxs-lookup"><span data-stu-id="8b066-181">Migrate containers from one share to another</span></span>
- <span data-ttu-id="8b066-182">Ver informações sobre os componentes de armazenamento individuais</span><span class="sxs-lookup"><span data-stu-id="8b066-182">View information about the individual storage components</span></span>
- <span data-ttu-id="8b066-183">Ver informações de utilização e desempenho</span><span class="sxs-lookup"><span data-stu-id="8b066-183">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="8b066-184">Administrador da Subscrição</span><span class="sxs-lookup"><span data-stu-id="8b066-184">Subscription Admin</span></span>
<span data-ttu-id="8b066-185">Versão de pré-visualização do módulo de administrador Subscrição do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8b066-185">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="8b066-186">Este módulo fornece funcionalidade que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="8b066-186">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="8b066-187">Gerir planos e ofertas</span><span class="sxs-lookup"><span data-stu-id="8b066-187">Manage plans and offers</span></span>
- <span data-ttu-id="8b066-188">Ver informações de utilização e desempenho</span><span class="sxs-lookup"><span data-stu-id="8b066-188">View usage and performance information</span></span>
- <span data-ttu-id="8b066-189">Gerir o RBAC</span><span class="sxs-lookup"><span data-stu-id="8b066-189">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="8b066-190">Subscrição</span><span class="sxs-lookup"><span data-stu-id="8b066-190">Subscription</span></span>
<span data-ttu-id="8b066-191">Versão de pré-visualização do módulo Subscrição do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8b066-191">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="8b066-192">Este módulo fornece funcionalidade que permite aos Utilizadores:</span><span class="sxs-lookup"><span data-stu-id="8b066-192">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="8b066-193">Criar, Eliminar e Atualizar Subscrições</span><span class="sxs-lookup"><span data-stu-id="8b066-193">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="8b066-194">Atualizar</span><span class="sxs-lookup"><span data-stu-id="8b066-194">Update</span></span>
<span data-ttu-id="8b066-195">Versão de pré-visualização do módulo de administrador Atualizar do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8b066-195">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="8b066-196">Neste módulo, os administradores podem:</span><span class="sxs-lookup"><span data-stu-id="8b066-196">In this module administrators can:</span></span>
- <span data-ttu-id="8b066-197">Listar e instalar atualizações disponíveis</span><span class="sxs-lookup"><span data-stu-id="8b066-197">List and install available updates</span></span>
- <span data-ttu-id="8b066-198">Retomar atualizações interrompidas</span><span class="sxs-lookup"><span data-stu-id="8b066-198">Resume interrupted updates</span></span>
- <span data-ttu-id="8b066-199">Ver atualizações instaladas</span><span class="sxs-lookup"><span data-stu-id="8b066-199">View installed updates</span></span>
