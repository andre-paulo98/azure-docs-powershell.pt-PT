---
title: Introdução ao Azure PowerShell
description: ''
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: 36a689dcfbd311871fe8638a0e56b037f6d0292a
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "56144741"
---
# <a name="get-started-with-azure-powershell"></a><span data-ttu-id="c5a94-102">Introdução ao Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c5a94-102">Get started with Azure PowerShell</span></span>

<span data-ttu-id="c5a94-103">O Azure PowerShell foi concebido para gerir e administrar recursos do Azure a partir da linha de comandos e para criar scripts de automatização que funcionam no âmbito do Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="c5a94-103">Azure PowerShell is designed for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="c5a94-104">Pode utilizá-lo no seu browser com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou instalá-lo na máquina local.</span><span class="sxs-lookup"><span data-stu-id="c5a94-104">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview) or you install it on your local machine.</span></span> <span data-ttu-id="c5a94-105">Este artigo ajuda-o a começar a utilizar o Azure PowerShell e explica os principais conceitos que lhe estão subjacentes.</span><span class="sxs-lookup"><span data-stu-id="c5a94-105">This article helps get you started with Azure PowerShell and teaches the core concepts behind it.</span></span>

## <a name="install-azure-powershell"></a><span data-ttu-id="c5a94-106">Instalar o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c5a94-106">Install Azure PowerShell</span></span>

<span data-ttu-id="c5a94-107">O primeiro passo é confirmar que tem instalada a versão mais recente do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c5a94-107">The first step is to make sure you have the latest version of the Azure PowerShell installed.</span></span> <span data-ttu-id="c5a94-108">Para obter informações sobre a versão mais recente, veja as [notas de versão](./release-notes-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="c5a94-108">For information about the latest release, see the [release notes](./release-notes-azureps.md).</span></span>

1. <span data-ttu-id="c5a94-109">[Instalar o Azure PowerShell](install-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="c5a94-109">[Install Azure PowerShell](install-azurerm-ps.md).</span></span>

2. <span data-ttu-id="c5a94-110">Para verificar se a instalação foi concluída com êxito, execute `Get-InstalledModule AzureRM -AllVersions` na sua linha de comandos.</span><span class="sxs-lookup"><span data-stu-id="c5a94-110">To verify the installation was successful, run `Get-InstalledModule AzureRM -AllVersions` from your command line.</span></span>

## <a name="azure-cloud-shell"></a><span data-ttu-id="c5a94-111">Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c5a94-111">Azure Cloud Shell</span></span>

<span data-ttu-id="c5a94-112">A forma mais simples de começar é [iniciar a Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="c5a94-112">The simplest way to get started is to [launch Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

1. <span data-ttu-id="c5a94-113">Inicie o Cloud Shell a partir do menu de navegação superior do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c5a94-113">Launch Cloud Shell from the top navigation of the Azure portal.</span></span>

   ![Ícone do Shell](~/media/get-started-azureps/shell-icon.png)

2. <span data-ttu-id="c5a94-115">Selecione a subscrição que quer utilizar e crie uma conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="c5a94-115">Choose the subscription you want to use and create a storage account.</span></span>

   ![Criar uma conta de armazenamento](~/media/get-started-azureps/storage-prompt.png)

<span data-ttu-id="c5a94-117">Assim que tiver sido criado o seu armazenamento, o Cloud Shell irá abrir uma sessão do PowerShell no browser.</span><span class="sxs-lookup"><span data-stu-id="c5a94-117">Once your storage has been created, the Cloud Shell will open a PowerShell session in the browser.</span></span>

![Cloud Shell para PowerShell](~/media/get-started-azureps/cloud-powershell.png)

<span data-ttu-id="c5a94-119">Também pode instalar o Azure PowerShell e utilizá-lo localmente numa sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c5a94-119">You can also install Azure PowerShell and use it locally in a PowerShell session.</span></span>

## <a name="sign-in-to-azure"></a><span data-ttu-id="c5a94-120">Iniciar sessão no Azure</span><span class="sxs-lookup"><span data-stu-id="c5a94-120">Sign in to Azure</span></span>

<span data-ttu-id="c5a94-121">Inicie sessão interativamente:</span><span class="sxs-lookup"><span data-stu-id="c5a94-121">Sign on interactively:</span></span>

1. <span data-ttu-id="c5a94-122">Digite `Connect-AzureRmAccount`.</span><span class="sxs-lookup"><span data-stu-id="c5a94-122">Type `Connect-AzureRmAccount`.</span></span> <span data-ttu-id="c5a94-123">Irá obter uma caixa de diálogo a pedir as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="c5a94-123">You'll get a dialog box asking for your Azure credentials.</span></span> <span data-ttu-id="c5a94-124">A opção "-Environment" permite-lhe autenticar-se no Azure China ou Azure Alemanha.</span><span class="sxs-lookup"><span data-stu-id="c5a94-124">Option '-Environment' can let you authenticate for Azure China or Azure Germany.</span></span>

   <span data-ttu-id="c5a94-125">por exemplo, Connect-AzureRmAccount -Environment AzureChinaCloud</span><span class="sxs-lookup"><span data-stu-id="c5a94-125">for example, Connect-AzureRmAccount -Environment AzureChinaCloud</span></span>

2. <span data-ttu-id="c5a94-126">Escreva o endereço de e-mail e a palavra-passe associados à sua conta.</span><span class="sxs-lookup"><span data-stu-id="c5a94-126">Type the email address and password associated with your account.</span></span> <span data-ttu-id="c5a94-127">O Azure autentica e guarda as informações das credenciais e, em seguida, fecha a janela.</span><span class="sxs-lookup"><span data-stu-id="c5a94-127">Azure authenticates and saves the credential information, and then closes the window.</span></span>

<span data-ttu-id="c5a94-128">Assim que tiver iniciado sessão numa conta do Azure, pode utilizar os cmdlets do Azure PowerShell para aceder e gerir os recursos na sua subscrição.</span><span class="sxs-lookup"><span data-stu-id="c5a94-128">Once you have signed in to an Azure account, you can use the Azure PowerShell cmdlets to access and manage the resources in your subscription.</span></span>

## <a name="create-a-windows-virtual-machine-using-simple-defaults"></a><span data-ttu-id="c5a94-129">Criar uma máquina virtual do Windows com predefinições simples</span><span class="sxs-lookup"><span data-stu-id="c5a94-129">Create a Windows virtual machine using simple defaults</span></span>

<span data-ttu-id="c5a94-130">O cmdlet `New-AzureRmVM` fornece uma sintaxe simplificada que facilita a criação de uma nova máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="c5a94-130">The `New-AzureRmVM` cmdlet provides a simplified syntax making it easy to create a new virtual machine.</span></span> <span data-ttu-id="c5a94-131">Existem apenas dois valores de parâmetros que tem de fornecer: o nome da VM e um conjunto de credenciais para a conta de administrador local na VM.</span><span class="sxs-lookup"><span data-stu-id="c5a94-131">There are only two parameter values you must provide: the name of the VM and a set of credentials for the local administrator account on the VM.</span></span>

<span data-ttu-id="c5a94-132">Primeiro, crie o objeto de credencial.</span><span class="sxs-lookup"><span data-stu-id="c5a94-132">First, create the credential object.</span></span>

```azurepowershell-interactive
$cred = Get-Credential -Message "Enter a username and password for the virtual machine."
```

```output
Windows PowerShell credential request.
Enter a username and password for the virtual machine.
User: localAdmin
Password for user localAdmin: *********
```

<span data-ttu-id="c5a94-133">Em seguida, crie a VM.</span><span class="sxs-lookup"><span data-stu-id="c5a94-133">Next, create the VM.</span></span>

```azurepowershell-interactive
New-AzureRmVM -Name SampleVM -Credential $cred
```

```output
ResourceGroupName        : SampleVM
Id                       : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/SampleVM/providers/Microsoft.Compute/virtualMachines/SampleVM
VmId                     : 43f6275d-ce50-49c8-a831-5d5974006e63
Name                     : SampleVM
Type                     : Microsoft.Compute/virtualMachines
Location                 : eastus
Tags                     : {}
HardwareProfile          : {VmSize}
NetworkProfile           : {NetworkInterfaces}
OSProfile                : {ComputerName, AdminUsername, WindowsConfiguration, Secrets}
ProvisioningState        : Succeeded
StorageProfile           : {ImageReference, OsDisk, DataDisks}
FullyQualifiedDomainName : samplevm-2c0867.eastus.cloudapp.azure.com
```

<span data-ttu-id="c5a94-134">Pode questionar-se sobre o que é criado e como a VM é configurada.</span><span class="sxs-lookup"><span data-stu-id="c5a94-134">You may wonder what else is created and how is the VM configured.</span></span> <span data-ttu-id="c5a94-135">Primeiro, vamos ver os nossos grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="c5a94-135">First, let's look at our resource groups.</span></span>

```azurepowershell-interactive
Get-AzureRmResourceGroup | Select-Object ResourceGroupName,Location
```

```output
ResourceGroupName          Location
-----------------          --------
cloud-shell-storage-westus westus
SampleVM                   eastus
```

<span data-ttu-id="c5a94-136">É criado o grupo de recursos **cloud-shell-storage-westus** quando utilizar o Cloud Shell pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="c5a94-136">The **cloud-shell-storage-westus** resource group is created the first time you use the Cloud Shell.</span></span> <span data-ttu-id="c5a94-137">O grupo de recursos **SampleVM** foi criado pelo cmdlet `New-AzureRmVM`.</span><span class="sxs-lookup"><span data-stu-id="c5a94-137">The **SampleVM** resource group was created by the `New-AzureRmVM` cmdlet.</span></span>

<span data-ttu-id="c5a94-138">Agora, que outros recursos foram criados neste novo grupo de recursos?</span><span class="sxs-lookup"><span data-stu-id="c5a94-138">Now, what other resources were created in this new resource group?</span></span>

```azurepowershell-interactive
Get-AzureRmResource |
  Where ResourceGroupName -eq SampleVM |
    Select-Object ResourceGroupName,Location,ResourceType,Name
```

```output
ResourceGroupName          Location ResourceType                            Name
-----------------          -------- ------------                            ----
SAMPLEVM                   eastus   Microsoft.Compute/disks                 SampleVM_OsDisk_1_9b286c54b168457fa1f8c47...
SampleVM                   eastus   Microsoft.Compute/virtualMachines       SampleVM
SampleVM                   eastus   Microsoft.Network/networkInterfaces     SampleVM
SampleVM                   eastus   Microsoft.Network/networkSecurityGroups SampleVM
SampleVM                   eastus   Microsoft.Network/publicIPAddresses     SampleVM
SampleVM                   eastus   Microsoft.Network/virtualNetworks       SampleVM
```

<span data-ttu-id="c5a94-139">Vamos obter mais detalhes sobre a VM.</span><span class="sxs-lookup"><span data-stu-id="c5a94-139">Let's get some more details about the VM.</span></span> <span data-ttu-id="c5a94-140">Este exemplo mostra como obter informações sobre a Imagem do SO utilizada para criar a VM.</span><span class="sxs-lookup"><span data-stu-id="c5a94-140">This example shows how to retrieve information about the OS Image used to create the VM.</span></span>

```azurepowershell-interactive
Get-AzureRmVM -Name SampleVM -ResourceGroupName SampleVM |
  Select-Object -ExpandProperty StorageProfile |
    Select-Object -ExpandProperty ImageReference
```

```output
Publisher : MicrosoftWindowsServer
Offer     : WindowsServer
Sku       : 2016-Datacenter
Version   : latest
Id        :
```

## <a name="create-a-fully-configured-linux-virtual-machine"></a><span data-ttu-id="c5a94-141">Criar uma Máquina Virtual do Linux totalmente configurada</span><span class="sxs-lookup"><span data-stu-id="c5a94-141">Create a fully configured Linux Virtual Machine</span></span>

<span data-ttu-id="c5a94-142">O exemplo anterior utilizou a sintaxe simplificada e os valores de parâmetros predefinidos para criar uma máquina virtual do Windows.</span><span class="sxs-lookup"><span data-stu-id="c5a94-142">The previous example used the simplified syntax and default parameter values to create a Windows virtual machine.</span></span> <span data-ttu-id="c5a94-143">Neste exemplo, fornecemos valores para todas as opções da máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="c5a94-143">In this example, we provide values for all options of the virtual machine.</span></span>

### <a name="create-a-resource-group"></a><span data-ttu-id="c5a94-144">Criar um grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="c5a94-144">Create a resource group</span></span>

<span data-ttu-id="c5a94-145">Neste exemplo, queremos criar um Grupo de Recursos.</span><span class="sxs-lookup"><span data-stu-id="c5a94-145">In this example, we want to create a Resource Group.</span></span> <span data-ttu-id="c5a94-146">Os Grupos de Recursos no Azure oferecem uma forma de gerir múltiplos recursos que quer agrupar logicamente.</span><span class="sxs-lookup"><span data-stu-id="c5a94-146">Resource Groups in Azure provide a way to manage multiple resources that you want to logically group together.</span></span> <span data-ttu-id="c5a94-147">Por exemplo, pode criar um Grupo de Recursos para uma aplicação ou projeto e adicionar uma máquina virtual, uma base de dados e um serviço de CDN ao mesmo.</span><span class="sxs-lookup"><span data-stu-id="c5a94-147">For example, you might create a Resource Group for an application or project and add a virtual machine, a database and a CDN service within it.</span></span>

<span data-ttu-id="c5a94-148">Vamos criar um grupo de recursos com o nome “MyResourceGroup" na região westeurope do Azure.</span><span class="sxs-lookup"><span data-stu-id="c5a94-148">Let's create a resource group named "MyResourceGroup" in the westeurope region of Azure.</span></span> <span data-ttu-id="c5a94-149">Para tal, escreva o comando seguinte:</span><span class="sxs-lookup"><span data-stu-id="c5a94-149">To do so type the following command:</span></span>

```azurepowershell-interactive
New-AzureRmResourceGroup -Name 'myResourceGroup' -Location 'westeurope'
```

```output
ResourceGroupName : myResourceGroup
Location          : westeurope
ProvisioningState : Succeeded
Tags              :
ResourceId        : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myResourceGroup
```

<span data-ttu-id="c5a94-150">Este novo grupo de recursos será utilizado para conter todos os recursos necessários para a nova VM criada.</span><span class="sxs-lookup"><span data-stu-id="c5a94-150">This new resource group will be used to contain all of the resources needed for the new VM we create.</span></span> <span data-ttu-id="c5a94-151">Para criar uma nova VM do Linux, temos de criar primeiro os outros recursos que são precisos e atribuí-los a uma configuração.</span><span class="sxs-lookup"><span data-stu-id="c5a94-151">To create a new Linux VM, we must first create the other required resources and assign them to a configuration.</span></span> <span data-ttu-id="c5a94-152">Em seguida, podemos utilizar a configuração para criar a VM.</span><span class="sxs-lookup"><span data-stu-id="c5a94-152">Then we can use that configuration to create the VM.</span></span> <span data-ttu-id="c5a94-153">Além disso, terá de ter uma chave pública SSH com o nome `id_rsa.pub` no diretório .ssh do seu perfil de utilizador.</span><span class="sxs-lookup"><span data-stu-id="c5a94-153">Also, you will need to have an SSH public key named `id_rsa.pub` in the .ssh directory of your user profile.</span></span>

#### <a name="create-the-required-network-resources"></a><span data-ttu-id="c5a94-154">Criar os recursos de rede necessários</span><span class="sxs-lookup"><span data-stu-id="c5a94-154">Create the required network resources</span></span>

<span data-ttu-id="c5a94-155">Primeiro, temos de criar uma configuração de sub-rede a utilizar no processo de criação da rede virtual.</span><span class="sxs-lookup"><span data-stu-id="c5a94-155">First we need to create a subnet configuration to be used with the virtual network creation process.</span></span> <span data-ttu-id="c5a94-156">Também podemos criar um endereço IP público para podermos ligar a esta VM.</span><span class="sxs-lookup"><span data-stu-id="c5a94-156">We also create a public IP address so that we can connect to this VM.</span></span> <span data-ttu-id="c5a94-157">Vamos criar um grupo de segurança de rede para proteger o acesso ao endereço público.</span><span class="sxs-lookup"><span data-stu-id="c5a94-157">We create a network security group to secure access to the public address.</span></span> <span data-ttu-id="c5a94-158">Por fim, criamos o NIC virtual através de todos os recursos anteriores.</span><span class="sxs-lookup"><span data-stu-id="c5a94-158">Finally we create the virtual NIC using all of the previous resources.</span></span>

```azurepowershell-interactive
# Variables for common values
$resourceGroup = "myResourceGroup"
$location = "westeurope"
$vmName = "myLinuxVM"

# Definer user name and blank password
$securePassword = ConvertTo-SecureString 'azurepassword' -AsPlainText -Force
$cred = New-Object System.Management.Automation.PSCredential ("azureuser", $securePassword)

# Create a subnet configuration
$subnetConfig = New-AzureRmVirtualNetworkSubnetConfig -Name mySubnet2 -AddressPrefix 192.168.2.0/24

# Create a virtual network
$vnet = New-AzureRmVirtualNetwork -ResourceGroupName $resourceGroup -Location $location `
  -Name MYvNET2 -AddressPrefix 192.168.0.0/16 -Subnet $subnetConfig

# Create a public IP address and specify a DNS name
$publicIp = New-AzureRmPublicIpAddress -ResourceGroupName $resourceGroup -Location $location `
  -Name "mypublicdns$(Get-Random)" -AllocationMethod Static -IdleTimeoutInMinutes 4
$publicIp | Select-Object Name,IpAddress

# Create an inbound network security group rule for port 22
$nsgRuleSSH = New-AzureRmNetworkSecurityRuleConfig -Name myNetworkSecurityGroupRuleSSH  -Protocol Tcp `
  -Direction Inbound -Priority 1000 -SourceAddressPrefix * -SourcePortRange * -DestinationAddressPrefix * `
  -DestinationPortRange 22 -Access Allow

# Create a network security group
$nsg = New-AzureRmNetworkSecurityGroup -ResourceGroupName $resourceGroup -Location $location `
  -Name myNetworkSecurityGroup2 -SecurityRules $nsgRuleSSH

# Create a virtual network card and associate with public IP address and NSG
$nic = New-AzureRmNetworkInterface -Name myNic2 -ResourceGroupName $resourceGroup -Location $location `
  -SubnetId $vnet.Subnets[0].Id -PublicIpAddressId $publicIp.Id -NetworkSecurityGroupId $nsg.Id
```

### <a name="create-the-vm-configuration"></a><span data-ttu-id="c5a94-159">Criar a configuração da VM</span><span class="sxs-lookup"><span data-stu-id="c5a94-159">Create the VM configuration</span></span>

<span data-ttu-id="c5a94-160">Agora que temos os recursos necessários, podemos criar o objeto de configuração da VM.</span><span class="sxs-lookup"><span data-stu-id="c5a94-160">Now that we have the required resources we can create the VM configuration object.</span></span>

```azurepowershell-interactive
# Create a virtual machine configuration
$vmConfig = New-AzureRmVMConfig -VMName $vmName -VMSize Standard_D1 |
  Set-AzureRmVMOperatingSystem -Linux -ComputerName $vmName -Credential $cred -DisablePasswordAuthentication |
  Set-AzureRmVMSourceImage -PublisherName Canonical -Offer UbuntuServer -Skus 14.04.2-LTS -Version latest |
  Add-AzureRmVMNetworkInterface -Id $nic.Id

# Configure SSH Keys
$sshPublicKey = Get-Content -Raw "$env:USERPROFILE\.ssh\id_rsa.pub"
Add-AzureRmVMSshPublicKey -VM $vmConfig -KeyData $sshPublicKey -Path "/home/azureuser/.ssh/authorized_keys"
```

### <a name="create-the-virtual-machine"></a><span data-ttu-id="c5a94-161">Criar a máquina virtual</span><span class="sxs-lookup"><span data-stu-id="c5a94-161">Create the virtual machine</span></span>

<span data-ttu-id="c5a94-162">Agora, podemos criar a VM com o respetivo objeto de configuração.</span><span class="sxs-lookup"><span data-stu-id="c5a94-162">Now we can create the VM using the VM configuration object.</span></span>

```azurepowershell-interactive
New-AzureRmVM -ResourceGroupName $resourceGroup -Location $location -VM $vmConfig
```

<span data-ttu-id="c5a94-163">Agora que a VM já está criada, pode iniciar sessão na sua nova VM do Linux através de SSH com o endereço IP público da VM que criou:</span><span class="sxs-lookup"><span data-stu-id="c5a94-163">Now that the VM has been created, you can sign in to your new Linux VM using SSH with the public IP address of the VM you created:</span></span>

```bash
ssh xx.xxx.xxx.xxx
```

```output
Welcome to Ubuntu 14.04.4 LTS (GNU/Linux 3.19.0-65-generic x86_64)

 * Documentation:  https://help.ubuntu.com/

  System information as of Sun Feb 19 00:32:28 UTC 2017

  System load: 0.31              Memory usage: 3%   Processes:       89
  Usage of /:  39.6% of 1.94GB   Swap usage:   0%   Users logged in: 0

  Graph this data and manage this system at:
    https://landscape.canonical.com/

  Get cloud support with Ubuntu Advantage Cloud Guest:
    http://www.ubuntu.com/business/services/cloud

0 packages can be updated.
0 updates are security updates.



The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

my-login@MyLinuxVM:../../..$
```

## <a name="creating-other-resources-in-azure"></a><span data-ttu-id="c5a94-164">Criar outros recursos no Azure</span><span class="sxs-lookup"><span data-stu-id="c5a94-164">Creating other resources in Azure</span></span>

<span data-ttu-id="c5a94-165">Acabámos de ver como são criados os Grupos de Recursos, as VMs do Linux e as VMs do Windows Server.</span><span class="sxs-lookup"><span data-stu-id="c5a94-165">We've now walked through how to create a Resource Group, a Linux VM, and a Windows Server VM.</span></span> <span data-ttu-id="c5a94-166">Também pode criar muitos outros tipos de recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="c5a94-166">You can create many other types of Azure resources as well.</span></span>

<span data-ttu-id="c5a94-167">Por exemplo, para criar um Balanceador de Carga da Rede do Azure que podemos, depois, associar às VMs acabadas de criar, podemos utilizar o comando de criação seguinte:</span><span class="sxs-lookup"><span data-stu-id="c5a94-167">For example, to create an Azure Network Load Balancer that we could then associate with our newly created VMs, we can use the following create command:</span></span>

```azurepowershell-interactive
New-AzureRmLoadBalancer -Name MyLoadBalancer -ResourceGroupName myResourceGroup -Location westeurope
```

<span data-ttu-id="c5a94-168">Também podemos criar uma Rede Virtual privada nova (geralmente conhecida como “VNet” no Azure) para a nossa infraestrutura, utilizando o comando seguinte:</span><span class="sxs-lookup"><span data-stu-id="c5a94-168">We could also create a new private Virtual Network (commonly referred to as a "VNet" within Azure) for our infrastructure using the following command:</span></span>

```azurepowershell-interactive
$subnetConfig = New-AzureRmVirtualNetworkSubnetConfig -Name mySubnet2 -AddressPrefix 10.0.0.0/16
$vnet = New-AzureRmVirtualNetwork -ResourceGroupName myResourceGroup -Location westeurope `
  -Name MYvNET3 -AddressPrefix 10.0.0.0/16 -Subnet $subnetConfig
```

<span data-ttu-id="c5a94-169">O que torna o Azure e o Azure PowerShell poderosos é o facto de poderem ser utilizados não só para obter a infraestrutura baseada na cloud, como também para criar serviços de plataformas geridos.</span><span class="sxs-lookup"><span data-stu-id="c5a94-169">What makes Azure and the Azure PowerShell powerful is that we can use it not just to get cloud-based infrastructure but also to create managed platform services.</span></span> <span data-ttu-id="c5a94-170">Os serviços de plataforma geridos podem, igualmente, ser combinados com a infraestrutura, para criar soluções ainda mais poderosas.</span><span class="sxs-lookup"><span data-stu-id="c5a94-170">The managed platform services can also be combined with infrastructure to build even more powerful solutions.</span></span>

<span data-ttu-id="c5a94-171">Por exemplo, pode utilizar o Azure PowerShell para criar um AppService do Azure.</span><span class="sxs-lookup"><span data-stu-id="c5a94-171">For example, you can use the Azure PowerShell to create an Azure AppService.</span></span> <span data-ttu-id="c5a94-172">O AppService do Azure é um serviço de plataforma gerido que proporciona uma excelente forma de alojar aplicações Web sem que tenha de se preocupar com a infraestrutura.</span><span class="sxs-lookup"><span data-stu-id="c5a94-172">Azure AppService is a managed platform service that provides a great way to host web apps without having to worry about infrastructure.</span></span> <span data-ttu-id="c5a94-173">Depois de criar o AppService do Azure, pode criar duas novas Aplicações Web do Azure no AppService com os comandos seguintes:</span><span class="sxs-lookup"><span data-stu-id="c5a94-173">After creating the Azure AppService, you can create two new Azure Web Apps within the AppService using the following commands:</span></span>

```azurepowershell-interactive
# Create an Azure AppService that we can host any number of web apps within
New-AzureRmAppServicePlan -Name MyAppServicePlan -Tier Basic -NumberofWorkers 2 -WorkerSize Small -ResourceGroupName myResourceGroup -Location westeurope

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
New-AzureRmWebApp -Name MyWebApp43432 -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westeurope
New-AzureRmWebApp -Name MyWebApp43433 -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westeurope
```

## <a name="listing-deployed-resources"></a><span data-ttu-id="c5a94-174">Listar recursos implementados</span><span class="sxs-lookup"><span data-stu-id="c5a94-174">Listing deployed resources</span></span>

<span data-ttu-id="c5a94-175">Pode utilizar o cmdlet `Get-AzureRmResource` para listar os recursos em execução no Azure.</span><span class="sxs-lookup"><span data-stu-id="c5a94-175">You can use the `Get-AzureRmResource` cmdlet to list the resources running in Azure.</span></span> <span data-ttu-id="c5a94-176">O exemplo seguinte mostra os recursos criados no novo grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="c5a94-176">The following example shows the resources we created in the new resource group.</span></span>

```azurepowershell-interactive
Get-AzureRmResource |
  Where-Object ResourceGroupName -eq myResourceGroup |
    Select-Object Name,Location,ResourceType
```

```output
Name                                                  Location   ResourceType
----                                                  --------   ------------
myLinuxVM_OsDisk_1_36ca038791f642ba91270879088c249a   westeurope Microsoft.Compute/disks
myWindowsVM_OsDisk_1_f627e6e2bb454c72897d72e9632adf9a westeurope Microsoft.Compute/disks
myLinuxVM                                             westeurope Microsoft.Compute/virtualMachines
myWindowsVM                                           westeurope Microsoft.Compute/virtualMachines
myWindowsVM/BGInfo                                    westeurope Microsoft.Compute/virtualMachines/extensions
myNic1                                                westeurope Microsoft.Network/networkInterfaces
myNic2                                                westeurope Microsoft.Network/networkInterfaces
myNetworkSecurityGroup1                               westeurope Microsoft.Network/networkSecurityGroups
myNetworkSecurityGroup2                               westeurope Microsoft.Network/networkSecurityGroups
mypublicdns245369171                                  westeurope Microsoft.Network/publicIPAddresses
mypublicdns779537141                                  westeurope Microsoft.Network/publicIPAddresses
MYvNET1                                               westeurope Microsoft.Network/virtualNetworks
MYvNET2                                               westeurope Microsoft.Network/virtualNetworks
micromyresomywi032907510                              westeurope Microsoft.Storage/storageAccounts
```

## <a name="deleting-resources"></a><span data-ttu-id="c5a94-177">Eliminar recursos</span><span class="sxs-lookup"><span data-stu-id="c5a94-177">Deleting resources</span></span>

<span data-ttu-id="c5a94-178">Para limpar a sua conta do Azure, tem de remover os recursos criados neste exemplo.</span><span class="sxs-lookup"><span data-stu-id="c5a94-178">To clean up your Azure account, you want to remove the resources we created in this example.</span></span> <span data-ttu-id="c5a94-179">Pode utilizar os cmdlets `Remove-AzureRm*` para eliminar recursos de que já não precisa.</span><span class="sxs-lookup"><span data-stu-id="c5a94-179">You can use the `Remove-AzureRm*` cmdlets to delete the resources you no longer need.</span></span> <span data-ttu-id="c5a94-180">Para remover a VM do Windows criada, utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="c5a94-180">To remove the Windows VM we created, using the following command:</span></span>

```azurepowershell-interactive
Remove-AzureRmVM -Name myWindowsVM -ResourceGroupName myResourceGroup
```

<span data-ttu-id="c5a94-181">Ser-lhe-á pedido para confirmar se quer remover o recurso.</span><span class="sxs-lookup"><span data-stu-id="c5a94-181">You'll be prompted to confirm that you want to remove the resource.</span></span>

```output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

<span data-ttu-id="c5a94-182">Também pode eliminar muitos recursos de uma só vez.</span><span class="sxs-lookup"><span data-stu-id="c5a94-182">You can also delete many resources at once.</span></span> <span data-ttu-id="c5a94-183">Por exemplo, o comando seguinte elimina o grupo de recursos "MyResourceGroup" que utilizámos em todos os exemplos até agora.</span><span class="sxs-lookup"><span data-stu-id="c5a94-183">For example, the following command deletes the resource group "MyResourceGroup" that we've used for all the samples so far.</span></span>
<span data-ttu-id="c5a94-184">Todos os recursos no grupo também são eliminados.</span><span class="sxs-lookup"><span data-stu-id="c5a94-184">All resources in the group are also deleted.</span></span>

```azurepowershell-interactive
Remove-AzureRmResourceGroup -Name myResourceGroup
```

```output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

<span data-ttu-id="c5a94-185">A tarefa pode demorar vários minutos a concluir, consoante o número e o tipo de recursos.</span><span class="sxs-lookup"><span data-stu-id="c5a94-185">The task can take several minutes to complete, depending on the number and type of resources.</span></span>

## <a name="get-samples"></a><span data-ttu-id="c5a94-186">Obter exemplos</span><span class="sxs-lookup"><span data-stu-id="c5a94-186">Get samples</span></span>

<span data-ttu-id="c5a94-187">Para saber mais sobre as formas como pode utilizar o Azure PowerShell, veja os nossos scripts mais comuns para [VMs do Linux](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Vms do Windows](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Aplicações Web](/azure/app-service-web/app-service-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json) e [Bases de Dados SQL](/azure/sql-database/sql-database-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json).</span><span class="sxs-lookup"><span data-stu-id="c5a94-187">To learn more about ways to use the Azure PowerShell, check out our most common scripts for [Linux VMs](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Windows VMs](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Web Apps](/azure/app-service-web/app-service-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), and [SQL Databases](/azure/sql-database/sql-database-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json).</span></span>

## <a name="next-steps"></a><span data-ttu-id="c5a94-188">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="c5a94-188">Next steps</span></span>

* [<span data-ttu-id="c5a94-189">Iniciar sessão com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c5a94-189">Sign in with Azure PowerShell</span></span>](authenticate-azureps.md)
* [<span data-ttu-id="c5a94-190">Gerir subscrições do Azure com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c5a94-190">Manage Azure subscriptions with Azure PowerShell</span></span>](manage-subscriptions-azureps.md)
* [<span data-ttu-id="c5a94-191">Criar principais de serviço no Azure com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c5a94-191">Create service principals in Azure using Azure PowerShell</span></span>](create-azure-service-principal-azureps.md)
* <span data-ttu-id="c5a94-192">Leia as notas de versão sobre a migração de uma versão mais antiga: [https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes](https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes).</span><span class="sxs-lookup"><span data-stu-id="c5a94-192">Read the release notes about migrating from an older release: [https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes](https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes).</span></span>
* <span data-ttu-id="c5a94-193">Obter ajuda da comunidade:</span><span class="sxs-lookup"><span data-stu-id="c5a94-193">Get help from the community:</span></span>
  * [<span data-ttu-id="c5a94-194">Fórum do Azure no MSDN</span><span class="sxs-lookup"><span data-stu-id="c5a94-194">Azure forum on MSDN</span></span>](http://go.microsoft.com/fwlink/p/?LinkId=320212)
  * [<span data-ttu-id="c5a94-195">Stackoverflow</span><span class="sxs-lookup"><span data-stu-id="c5a94-195">stackoverflow</span></span>](http://go.microsoft.com/fwlink/?LinkId=320213)
