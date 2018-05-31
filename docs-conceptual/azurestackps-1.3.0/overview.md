# <a name="azure-stack-module-130"></a><span data-ttu-id="8c6ca-101">Módulo 1.3.0 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="8c6ca-101">Azure Stack Module 1.3.0</span></span>

## <a name="requirements"></a><span data-ttu-id="8c6ca-102">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="8c6ca-102">Requirements:</span></span>
<span data-ttu-id="8c6ca-103">A versão mínima suportada do Azure Stack é a 1804.</span><span class="sxs-lookup"><span data-stu-id="8c6ca-103">Minimum supported Azure Stack version is 1804.</span></span>

<span data-ttu-id="8c6ca-104">Nota: Se estiver a utilizar uma versão anterior, instale a versão 1.2.11</span><span class="sxs-lookup"><span data-stu-id="8c6ca-104">Note: If you are using an earlier version install version 1.2.11</span></span>

## <a name="known-issues"></a><span data-ttu-id="8c6ca-105">Problemas conhecidos:</span><span class="sxs-lookup"><span data-stu-id="8c6ca-105">Known issues:</span></span>

- <span data-ttu-id="8c6ca-106">Fechar Alerta requer a versão 1803 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="8c6ca-106">Close Alert requires Azure Stack version 1803</span></span>
- <span data-ttu-id="8c6ca-107">Alguns cmdlets de Armazenamento requerem a versão 1804 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="8c6ca-107">Some Storage cmdlets do require Azure Stack version 1804</span></span>
- <span data-ttu-id="8c6ca-108">O New-AzsOffer não permite criar uma oferta com o estado público.</span><span class="sxs-lookup"><span data-stu-id="8c6ca-108">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="8c6ca-109">O cmdlet Set-AzsOffer tem de ser chamado depois para alterar o estado.</span><span class="sxs-lookup"><span data-stu-id="8c6ca-109">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="8c6ca-110">Não é possível remover um Conjunto IP sem uma reimplementação</span><span class="sxs-lookup"><span data-stu-id="8c6ca-110">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="breaking-changes"></a><span data-ttu-id="8c6ca-111">Alterações Interruptivas</span><span class="sxs-lookup"><span data-stu-id="8c6ca-111">Breaking Changes</span></span>
<span data-ttu-id="8c6ca-112">Todas as alterações interruptivas migradas da versão 1.2.11 estão documentadas aqui https://aka.ms/azspowershellmigration</span><span class="sxs-lookup"><span data-stu-id="8c6ca-112">All breaking changes migrating from 1.2.11 are documented here https://aka.ms/azspowershellmigration</span></span>

## <a name="install"></a><span data-ttu-id="8c6ca-113">Instalar</span><span class="sxs-lookup"><span data-stu-id="8c6ca-113">Install</span></span>
```
# Remove previous Versions
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Uninstall-Module -Name AzureStack -Force 


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2017-03-09-profile -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.3.0
```
## <a name="content"></a><span data-ttu-id="8c6ca-114">Conteúdo:</span><span class="sxs-lookup"><span data-stu-id="8c6ca-114">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="8c6ca-115">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="8c6ca-115">Azure Bridge</span></span>
<span data-ttu-id="8c6ca-116">Versão de pré-visualização do módulo de administrador AzureBridge do Azure Stack que lhe permite sindicar imagens a partir do Azure.</span><span class="sxs-lookup"><span data-stu-id="8c6ca-116">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="8c6ca-117">Cópia de segurança</span><span class="sxs-lookup"><span data-stu-id="8c6ca-117">Backup</span></span>
<span data-ttu-id="8c6ca-118">Versão de pré-visualização do módulo de administrador Cópia de Segurança que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="8c6ca-118">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="8c6ca-119">Configurar em que local as cópias de segurança são armazenadas</span><span class="sxs-lookup"><span data-stu-id="8c6ca-119">Configure where backups are stored</span></span>
- <span data-ttu-id="8c6ca-120">Fazer cópias de segurança</span><span class="sxs-lookup"><span data-stu-id="8c6ca-120">Perform backups</span></span>
- <span data-ttu-id="8c6ca-121">Listar e restaurar cópias de segurança concluídas</span><span class="sxs-lookup"><span data-stu-id="8c6ca-121">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="8c6ca-122">Comércio</span><span class="sxs-lookup"><span data-stu-id="8c6ca-122">Commerce</span></span>
<span data-ttu-id="8c6ca-123">Versão de pré-visualização do módulo de administrador Comércio do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8c6ca-123">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="8c6ca-124">Computação</span><span class="sxs-lookup"><span data-stu-id="8c6ca-124">Compute</span></span>
<span data-ttu-id="8c6ca-125">Versão de pré-visualização do módulo de administrador Computação do Azure Stack que fornece funcionalidade que permite gerir quotas de computação, imagens de plataforma e extensões de máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="8c6ca-125">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="8c6ca-126">Recursos de infraestrutura</span><span class="sxs-lookup"><span data-stu-id="8c6ca-126">Fabric</span></span>
<span data-ttu-id="8c6ca-127">Versão de pré-visualização do módulo de administrador Recursos de infraestrutura do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack:</span><span class="sxs-lookup"><span data-stu-id="8c6ca-127">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="8c6ca-128">Parar, Iniciar e Encerrar nós de unidade de escala</span><span class="sxs-lookup"><span data-stu-id="8c6ca-128">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="8c6ca-129">Drenar e Retomar nós de unidade de escala para atividades relacionadas com FRU</span><span class="sxs-lookup"><span data-stu-id="8c6ca-129">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="8c6ca-130">Reparar nós de unidade de escala</span><span class="sxs-lookup"><span data-stu-id="8c6ca-130">Repair of scale unit nodes</span></span>
- <span data-ttu-id="8c6ca-131">Reiniciar a função Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="8c6ca-131">Restart of Infrastructure role</span></span>
- <span data-ttu-id="8c6ca-132">Parar, Iniciar e Encerrar instâncias de função Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="8c6ca-132">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="8c6ca-133">Criar novos Conjuntos IP</span><span class="sxs-lookup"><span data-stu-id="8c6ca-133">Create new IP Pools</span></span>


### <a name="gallery"></a><span data-ttu-id="8c6ca-134">Galeria</span><span class="sxs-lookup"><span data-stu-id="8c6ca-134">Gallery</span></span>
<span data-ttu-id="8c6ca-135">Versão de pré-visualização do módulo de administrador Galeria do Azure Stack que fornece funcionalidade que permite gerir itens da galeria no marketplace do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8c6ca-135">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="8c6ca-136">Informações de Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="8c6ca-136">Infrastructure Insights</span></span>
<span data-ttu-id="8c6ca-137">Versão de pré-visualização do módulo de administrador Informações de Infraestrutura que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="8c6ca-137">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="8c6ca-138">Ver o estado de funcionamento dos recursos de carimbo do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="8c6ca-138">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="8c6ca-139">Ver e gerir alertas</span><span class="sxs-lookup"><span data-stu-id="8c6ca-139">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="8c6ca-140">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8c6ca-140">KeyVault</span></span>
<span data-ttu-id="8c6ca-141">Versão de pré-visualização do módulo de administrador KeyVault do Azure Stack que permite ao administrador ver as quotas do KeyVault.</span><span class="sxs-lookup"><span data-stu-id="8c6ca-141">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="8c6ca-142">Rede</span><span class="sxs-lookup"><span data-stu-id="8c6ca-142">Network</span></span>
<span data-ttu-id="8c6ca-143">Versão de pré-visualização do módulo de administrador Rede que permite:</span><span class="sxs-lookup"><span data-stu-id="8c6ca-143">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="8c6ca-144">Gerir quotas de rede</span><span class="sxs-lookup"><span data-stu-id="8c6ca-144">Management of network quotas</span></span>
- <span data-ttu-id="8c6ca-145">Ver recursos de rede alocados, como endereços IP públicos, redes virtuais, balanceadores de carga</span><span class="sxs-lookup"><span data-stu-id="8c6ca-145">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="8c6ca-146">Fornece um cmdlet que apresenta uma descrição geral de administrador</span><span class="sxs-lookup"><span data-stu-id="8c6ca-146">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="8c6ca-147">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8c6ca-147">Storage</span></span>
<span data-ttu-id="8c6ca-148">Versão de pré-visualização do módulo de administrador Armazenamento do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8c6ca-148">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="8c6ca-149">Nesta versão, fornecemos funcionalidade para:</span><span class="sxs-lookup"><span data-stu-id="8c6ca-149">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="8c6ca-150">Gerir quotas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="8c6ca-150">Manage storage quotas</span></span>
- <span data-ttu-id="8c6ca-151">Libertar memória de recursos de armazenamento eliminados</span><span class="sxs-lookup"><span data-stu-id="8c6ca-151">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="8c6ca-152">Restaurar contas de armazenamento eliminadas</span><span class="sxs-lookup"><span data-stu-id="8c6ca-152">Restore deleted storage accounts</span></span>
- <span data-ttu-id="8c6ca-153">Migrar contentores de uma partilha para outra</span><span class="sxs-lookup"><span data-stu-id="8c6ca-153">Migrate containers from one share to another</span></span>
- <span data-ttu-id="8c6ca-154">Ver informações sobre os componentes de armazenamento individuais</span><span class="sxs-lookup"><span data-stu-id="8c6ca-154">View information about the individual storage components</span></span>
- <span data-ttu-id="8c6ca-155">Ver informações de utilização e desempenho</span><span class="sxs-lookup"><span data-stu-id="8c6ca-155">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="8c6ca-156">Administrador da Subscrição</span><span class="sxs-lookup"><span data-stu-id="8c6ca-156">Subscription Admin</span></span>
<span data-ttu-id="8c6ca-157">Versão de pré-visualização do módulo de administrador Subscrição do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8c6ca-157">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="8c6ca-158">Este módulo fornece funcionalidade que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="8c6ca-158">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="8c6ca-159">Gerir planos e ofertas</span><span class="sxs-lookup"><span data-stu-id="8c6ca-159">Manage plans and offers</span></span>
- <span data-ttu-id="8c6ca-160">Ver informações de utilização e desempenho</span><span class="sxs-lookup"><span data-stu-id="8c6ca-160">View usage and performance information</span></span>
- <span data-ttu-id="8c6ca-161">Gerir o RBAC</span><span class="sxs-lookup"><span data-stu-id="8c6ca-161">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="8c6ca-162">Subscrição</span><span class="sxs-lookup"><span data-stu-id="8c6ca-162">Subscription</span></span>
<span data-ttu-id="8c6ca-163">Versão de pré-visualização do módulo Subscrição do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8c6ca-163">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="8c6ca-164">Este módulo fornece funcionalidade que permite aos Utilizadores:</span><span class="sxs-lookup"><span data-stu-id="8c6ca-164">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="8c6ca-165">Criar, Eliminar e Atualizar Subscrições</span><span class="sxs-lookup"><span data-stu-id="8c6ca-165">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="8c6ca-166">Atualizar</span><span class="sxs-lookup"><span data-stu-id="8c6ca-166">Update</span></span>
<span data-ttu-id="8c6ca-167">Versão de pré-visualização do módulo de administrador Atualizar do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8c6ca-167">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="8c6ca-168">Neste módulo, os administradores podem:</span><span class="sxs-lookup"><span data-stu-id="8c6ca-168">In this module administrators can:</span></span>
- <span data-ttu-id="8c6ca-169">Listar e instalar atualizações disponíveis</span><span class="sxs-lookup"><span data-stu-id="8c6ca-169">List and install available updates</span></span>
- <span data-ttu-id="8c6ca-170">Retomar atualizações interrompidas</span><span class="sxs-lookup"><span data-stu-id="8c6ca-170">Resume interrupted updates</span></span>
- <span data-ttu-id="8c6ca-171">Ver atualizações instaladas</span><span class="sxs-lookup"><span data-stu-id="8c6ca-171">View installed updates</span></span>
