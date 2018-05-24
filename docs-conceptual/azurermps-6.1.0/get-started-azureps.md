---
title: Introdução ao Azure PowerShell | Microsoft Docs
description: ''
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: get-started-article
ms.date: 11/15/2017
ms.openlocfilehash: 54ea76802ea3b1fa4f7c1ddc8cb960dcba443f73
ms.sourcegitcommit: 5971c92cb023bdd1d71fa2ad0a3b378abfbd092a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/23/2018
---
# <a name="getting-started-with-azure-powershell"></a><span data-ttu-id="b1e5a-102">Introdução ao Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b1e5a-102">Getting started with Azure PowerShell</span></span>

<span data-ttu-id="b1e5a-103">O Azure PowerShell foi concebido para gerir e administrar recursos do Azure a partir da linha de comandos e para criar scripts de automatização que funcionam no âmbito do Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-103">Azure PowerShell is designed for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="b1e5a-104">Pode utilizá-lo no seu browser com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou pode instalá-lo no seu computador local e utilizá-lo em qualquer sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-104">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can install it on your local machine and use it in any PowerShell session.</span></span> <span data-ttu-id="b1e5a-105">Este artigo ajuda-o a começar a utilizá-lo e explica-lhe os conceitos principais subjacentes.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-105">This article helps get you started using it, and teaches you the core concepts behind it.</span></span>

## <a name="connect"></a><span data-ttu-id="b1e5a-106">Ligar</span><span class="sxs-lookup"><span data-stu-id="b1e5a-106">Connect</span></span>

<span data-ttu-id="b1e5a-107">A forma mais simples de começar é [iniciar a Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="b1e5a-107">The simplest way to get started is to [launch Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

1. <span data-ttu-id="b1e5a-108">Inicie o Cloud Shell a partir do menu de navegação superior do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-108">Launch Cloud Shell from the top navigation of the Azure portal.</span></span>

   ![Ícone do Shell](~/media/get-started-azureps/shell-icon.png)

2. <span data-ttu-id="b1e5a-110">Selecione a subscrição que quer utilizar e crie uma conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-110">Choose the subscription you want to use and create a storage account.</span></span>

   ![Criar uma conta de armazenamento](~/media/get-started-azureps/storage-prompt.png)

<span data-ttu-id="b1e5a-112">Assim que tiver sido criado o seu armazenamento, o Cloud Shell irá abrir uma sessão do PowerShell no browser.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-112">Once your storage has been created, the Cloud Shell will open a PowerShell session in the browser.</span></span>

![Cloud Shell para PowerShell](~/media/get-started-azureps/cloud-powershell.png)

<span data-ttu-id="b1e5a-114">Também pode instalar o Azure PowerShell e utilizá-lo localmente numa sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-114">You can also install Azure PowerShell and use it locally in a PowerShell session.</span></span>

## <a name="install-azure-powershell"></a><span data-ttu-id="b1e5a-115">Instalar o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b1e5a-115">Install Azure PowerShell</span></span>

<span data-ttu-id="b1e5a-116">O primeiro passo é confirmar que tem instalada a versão mais recente do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-116">The first step is to make sure you have the latest version of the Azure PowerShell installed.</span></span> <span data-ttu-id="b1e5a-117">Para obter informações sobre a versão mais recente, veja as [notas de versão](./release-notes-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="b1e5a-117">For information about the latest release, see the [release notes](./release-notes-azureps.md).</span></span>

1. <span data-ttu-id="b1e5a-118">[Instalar o Azure PowerShell](install-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="b1e5a-118">[Install Azure PowerShell](install-azurerm-ps.md).</span></span>

2. <span data-ttu-id="b1e5a-119">Para verificar se a instalação foi concluída com êxito, execute `Get-Module AzureRM -ListAvailable` na sua linha de comandos.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-119">To verify the installation was successful, run `Get-Module AzureRM -ListAvailable` from your command line.</span></span>

## <a name="log-in-to-azure"></a><span data-ttu-id="b1e5a-120">Iniciar sessão no Azure</span><span class="sxs-lookup"><span data-stu-id="b1e5a-120">Log in to Azure</span></span>

<span data-ttu-id="b1e5a-121">Inicie sessão interativamente:</span><span class="sxs-lookup"><span data-stu-id="b1e5a-121">Sign on interactively:</span></span>

1. <span data-ttu-id="b1e5a-122">Digite `Connect-AzureRmAccount`.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-122">Type `Connect-AzureRmAccount`.</span></span> <span data-ttu-id="b1e5a-123">Obterá uma caixa de diálogo a solicitar as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-123">You will get dialog box asking for your Azure credentials.</span></span> <span data-ttu-id="b1e5a-124">A opção "-Environment" permite-lhe iniciar sessão no Azure China ou Azure Alemanha.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-124">Option '-Environment' can let you login in Azure China or Azure Germany.</span></span>

   <span data-ttu-id="b1e5a-125">Por exemplo, Connect-AzureRmAccount -Environment AzureChinaCloud</span><span class="sxs-lookup"><span data-stu-id="b1e5a-125">e.g. Connect-AzureRmAccount -Environment AzureChinaCloud</span></span>

2. <span data-ttu-id="b1e5a-126">Escreva o endereço de e-mail e a palavra-passe associados à sua conta.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-126">Type the email address and password associated with your account.</span></span> <span data-ttu-id="b1e5a-127">O Azure autentica e guarda as informações das credenciais e, em seguida, fecha a janela.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-127">Azure authenticates and saves the credential information, and then closes the window.</span></span>

<span data-ttu-id="b1e5a-128">Assim que tiver iniciado sessão numa conta do Azure, pode utilizar os cmdlets do Azure PowerShell para aceder e gerir os recursos na sua subscrição.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-128">Once you have signed in to an Azure account, you can use the Azure PowerShell cmdlets to access and manager the resources in your subscription.</span></span>

## <a name="create-a-windows-virtual-machine-using-simple-defaults"></a><span data-ttu-id="b1e5a-129">Criar uma máquina virtual do Windows com predefinições simples</span><span class="sxs-lookup"><span data-stu-id="b1e5a-129">Create a Windows virtual machine using simple defaults</span></span>

<span data-ttu-id="b1e5a-130">O cmdlet `New-AzureRmVM` fornece uma sintaxe simplificada que facilita a criação de uma nova máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-130">The `New-AzureRmVM` cmdlet provides a simplified syntax making it easy to create a new virtual machine.</span></span> <span data-ttu-id="b1e5a-131">Existem apenas dois valores de parâmetros que tem de fornecer: o nome da VM e um conjunto de credenciais para a conta de administrador local na VM.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-131">There are only two parameter values you must provide: the name of the VM and a set of credentials for the local administrator account on the VM.</span></span>

<span data-ttu-id="b1e5a-132">Primeiro, crie o objeto de credencial.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-132">First, create the credential object.</span></span>

```azurepowershell-interactive
$cred = Get-Credential -Message "Enter a username and password for the virtual machine."
```

```output
Windows PowerShell credential request.
Enter a username and password for the virtual machine.
User: localAdmin
Password for user localAdmin: *********
```
<span data-ttu-id="b1e5a-133">Em seguida, crie a VM.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-133">Next, create the VM.</span></span>

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

<span data-ttu-id="b1e5a-134">Foi fácil.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-134">That was easy.</span></span> <span data-ttu-id="b1e5a-135">No entanto, pode questionar-se sobre o que é criado e como a VM é configurada.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-135">But, you may wonder what else is created and how is the VM configured.</span></span> <span data-ttu-id="b1e5a-136">Primeiro, vamos ver os nossos grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-136">First, let's look at our resource groups.</span></span>

```azurepowershell-interactive
Get-AzureRmResourceGroup | Select-Object ResourceGroupName,Location
```

```output
ResourceGroupName          Location
-----------------          --------
cloud-shell-storage-westus westus
SampleVM                   eastus
```

<span data-ttu-id="b1e5a-137">É criado o grupo de recursos **cloud-shell-storage-westus** quando utilizar o Cloud Shell pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-137">The **cloud-shell-storage-westus** resource group is created the first time you use the Cloud Shell.</span></span> <span data-ttu-id="b1e5a-138">O grupo de recursos **SampleVM** foi criado pelo cmdlet `New-AzureRmVM`.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-138">The **SampleVM** resource group was created by the `New-AzureRmVM` cmdlet.</span></span>

<span data-ttu-id="b1e5a-139">Agora, que outros recursos foram criados neste novo grupo de recursos?</span><span class="sxs-lookup"><span data-stu-id="b1e5a-139">Now, what other resources were created in this new resource group?</span></span>

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

<span data-ttu-id="b1e5a-140">Vamos obter mais detalhes sobre a VM.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-140">Let's get some more details about the VM.</span></span> <span data-ttu-id="b1e5a-141">Este exemplo mostra como obter informações sobre a Imagem do SO utilizada para criar a VM.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-141">This examples shows how to retrieve information about the OS Image used to create the VM.</span></span>

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

## <a name="create-a-fully-configured-linux-virtual-machine"></a><span data-ttu-id="b1e5a-142">Criar uma Máquina Virtual do Linux totalmente configurada</span><span class="sxs-lookup"><span data-stu-id="b1e5a-142">Create a fully configured Linux Virtual Machine</span></span>

<span data-ttu-id="b1e5a-143">O exemplo anterior utilizou a sintaxe simplificada e os valores de parâmetros predefinidos para criar uma máquina virtual do Windows.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-143">The previous example used the simplified syntax and default parameter values to create a Windows virtual machine.</span></span> <span data-ttu-id="b1e5a-144">Neste exemplo, fornecemos valores para todas as opções da máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-144">In this example, we provide values for all options of the virtual machine.</span></span>

### <a name="create-a-resource-group"></a><span data-ttu-id="b1e5a-145">Criar um grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="b1e5a-145">Create a resource group</span></span>

<span data-ttu-id="b1e5a-146">Para este exemplo, queremos criar um Grupo de Recursos.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-146">For this example we want to create a Resource Group.</span></span> <span data-ttu-id="b1e5a-147">Os Grupos de Recursos no Azure oferecem uma forma de gerir múltiplos recursos que quer agrupar logicamente.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-147">Resource Groups in Azure provide a way to manage multiple resources that you want to logically group together.</span></span> <span data-ttu-id="b1e5a-148">Por exemplo, pode criar um Grupo de Recursos para uma aplicação ou projeto e adicionar uma máquina virtual, uma base de dados e um serviço de CDN ao mesmo.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-148">For example, you might create a Resource Group for an application or project and add a virtual machine, a database and a CDN service within it.</span></span>

<span data-ttu-id="b1e5a-149">Vamos criar um grupo de recursos com o nome “MyResourceGroup" na região westeurope do Azure.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-149">Let's create a resource group named "MyResourceGroup" in the westeurope region of Azure.</span></span> <span data-ttu-id="b1e5a-150">Para tal, escreva o comando seguinte:</span><span class="sxs-lookup"><span data-stu-id="b1e5a-150">To do so type the following command:</span></span>

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

<span data-ttu-id="b1e5a-151">Este novo grupo de recursos será utilizado para conter todos os recursos necessários para a nova VM criada.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-151">This new resource group will be used to contain all of the resources needed for the new VM we create.</span></span> <span data-ttu-id="b1e5a-152">Para criar uma nova VM do Linux, temos de criar primeiro os outros recursos necessários e atribuí-los a uma configuração.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-152">To create a new Linux VM we must first create the other required resources and assign them to a configuration.</span></span> <span data-ttu-id="b1e5a-153">Em seguida, podemos utilizar a configuração para criar a VM.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-153">Then we can use that configuration to create the VM.</span></span> <span data-ttu-id="b1e5a-154">Além disso, terá de ter uma chave pública SSH com o nome `id_rsa.pub` no diretório .ssh do seu perfil de utilizador.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-154">Also, you will need to have an SSH public key named `id_rsa.pub` in the .ssh directory of your user profile.</span></span>

#### <a name="create-the-required-network-resources"></a><span data-ttu-id="b1e5a-155">Criar os recursos de rede necessários</span><span class="sxs-lookup"><span data-stu-id="b1e5a-155">Create the required network resources</span></span>

<span data-ttu-id="b1e5a-156">Primeiro, temos de criar uma configuração de sub-rede a utilizar no processo de criação da rede virtual.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-156">First we need to create a subnet configuration to be used with the virtual network creation process.</span></span> <span data-ttu-id="b1e5a-157">Também podemos criar um endereço IP público para podermos ligar a esta VM.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-157">We also create a public IP address so that we can connect to this VM.</span></span> <span data-ttu-id="b1e5a-158">Vamos criar um grupo de segurança de rede para proteger o acesso ao endereço público.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-158">We create a network security group to secure access to the public address.</span></span> <span data-ttu-id="b1e5a-159">Por fim, criamos o NIC virtual através de todos os recursos anteriores.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-159">Finally we create the virtual NIC using all of the previous resources.</span></span>

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

### <a name="create-the-vm-configuration"></a><span data-ttu-id="b1e5a-160">Criar a configuração da VM</span><span class="sxs-lookup"><span data-stu-id="b1e5a-160">Create the VM configuration</span></span>

<span data-ttu-id="b1e5a-161">Agora que temos os recursos necessários, podemos criar o objeto de configuração da VM.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-161">Now that we have the required resources we can create the VM configuration object.</span></span>

```azurepowershell-interactive
# Create a virtual machine configuration
$vmConfig = New-AzureRmVMConfig -VMName $vmName -VMSize Standard_D1 |
  Set-AzureRmVMOperatingSystem -Linux -ComputerName $vmName -Credential $cred -DisablePasswordAuthentication |
  Set-AzureRmVMSourceImage -PublisherName Canonical -Offer UbuntuServer -Skus 14.04.2-LTS -Version latest |
  Add-AzureRmVMNetworkInterface -Id $nic.Id

# Configure SSH Keys
$sshPublicKey = Get-Content "$env:USERPROFILE\.ssh\id_rsa.pub"
Add-AzureRmVMSshPublicKey -VM $vmConfig -KeyData $sshPublicKey -Path "/home/azureuser/.ssh/authorized_keys"
```

### <a name="create-the-virtual-machine"></a><span data-ttu-id="b1e5a-162">Criar a máquina virtual</span><span class="sxs-lookup"><span data-stu-id="b1e5a-162">Create the virtual machine</span></span>

<span data-ttu-id="b1e5a-163">Agora, podemos criar a VM com o respetivo objeto de configuração.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-163">Now we can create the VM using the VM configuration object.</span></span>

```azurepowershell-interactive
New-AzureRmVM -ResourceGroupName $resourceGroup -Location $location -VM $vmConfig
```

<span data-ttu-id="b1e5a-164">Agora que a VM já está criada, pode iniciar sessão na sua nova VM do Linux através de SSH com o endereço IP público da VM que criou:</span><span class="sxs-lookup"><span data-stu-id="b1e5a-164">Now that the VM has been created, you can log on to your new Linux VM using SSH with the public IP address of the VM you created:</span></span>

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

## <a name="creating-other-resources-in-azure"></a><span data-ttu-id="b1e5a-165">Criar outros recursos no Azure</span><span class="sxs-lookup"><span data-stu-id="b1e5a-165">Creating other resources in Azure</span></span>

<span data-ttu-id="b1e5a-166">Acabámos de ver como são criados os Grupos de Recursos, as VMs do Linux e as VMs do Windows Server.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-166">We've now walked through how to create a Resource Group, a Linux VM, and a Windows Server VM.</span></span> <span data-ttu-id="b1e5a-167">Também pode criar muitos outros tipos de recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-167">You can create many other types of Azure resources as well.</span></span>

<span data-ttu-id="b1e5a-168">Por exemplo, para criar um Balanceador de Carga da Rede do Azure que podemos, depois, associar às VMs acabadas de criar, podemos utilizar o comando de criação seguinte:</span><span class="sxs-lookup"><span data-stu-id="b1e5a-168">For example, to create an Azure Network Load Balancer that we could then associate with our newly created VMs, we can use the following create command:</span></span>

```azurepowershell-interactive
New-AzureRmLoadBalancer -Name MyLoadBalancer -ResourceGroupName myResourceGroup -Location westeurope
```

<span data-ttu-id="b1e5a-169">Também podemos criar uma Rede Virtual privada nova (geralmente conhecida como “VNet” no Azure) para a nossa infraestrutura, utilizando o comando seguinte:</span><span class="sxs-lookup"><span data-stu-id="b1e5a-169">We could also create a new private Virtual Network (commonly referred to as a "VNet" within Azure) for our infrastructure using the following command:</span></span>

```azurepowershell-interactive
$subnetConfig = New-AzureRmVirtualNetworkSubnetConfig -Name mySubnet2 -AddressPrefix 10.0.0.0/16
$vnet = New-AzureRmVirtualNetwork -ResourceGroupName myResourceGroup -Location westeurope `
  -Name MYvNET3 -AddressPrefix 10.0.0.0/16 -Subnet $subnetConfig
```

<span data-ttu-id="b1e5a-170">O que torna o Azure e o Azure PowerShell poderosos é o facto de poderem ser utilizados não só para obter a infraestrutura baseada na cloud, como também para criar serviços de plataformas geridos.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-170">What makes Azure and the Azure PowerShell powerful is that we can use it not just to get cloud-based infrastructure but also to create managed platform services.</span></span> <span data-ttu-id="b1e5a-171">Os serviços de plataforma geridos podem, igualmente, ser combinados com a infraestrutura, para criar soluções ainda mais poderosas.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-171">The managed platform services can also be combined with infrastructure to build even more powerful solutions.</span></span>

<span data-ttu-id="b1e5a-172">Por exemplo, pode utilizar o Azure PowerShell para criar um AppService do Azure.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-172">For example, you can use the Azure PowerShell to create an Azure AppService.</span></span> <span data-ttu-id="b1e5a-173">O AppService do Azure é um serviço de plataforma gerido que proporciona uma excelente forma de alojar aplicações Web sem que tenha de se preocupar com a infraestrutura.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-173">Azure AppService is a managed platform service that provides a great way to host web apps without having to worry about infrastructure.</span></span> <span data-ttu-id="b1e5a-174">Depois de criar o AppService do Azure, pode criar duas novas Aplicações Web do Azure no AppService com os comandos seguintes:</span><span class="sxs-lookup"><span data-stu-id="b1e5a-174">After creating the Azure AppService, you can create two new Azure Web Apps within the AppService using the following commands:</span></span>

```azurepowershell-interactive
# Create an Azure AppService that we can host any number of web apps within
New-AzureRmAppServicePlan -Name MyAppServicePlan -Tier Basic -NumberofWorkers 2 -WorkerSize Small -ResourceGroupName myResourceGroup -Location westeurope

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
New-AzureRmWebApp -Name MyWebApp43432 -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westeurope
New-AzureRmWebApp -Name MyWebApp43433 -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westeurope
```

## <a name="listing-deployed-resources"></a><span data-ttu-id="b1e5a-175">Listar recursos implementados</span><span class="sxs-lookup"><span data-stu-id="b1e5a-175">Listing deployed resources</span></span>

<span data-ttu-id="b1e5a-176">Pode utilizar o cmdlet `Get-AzureRmResource` para listar os recursos em execução no Azure.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-176">You can use the `Get-AzureRmResource` cmdlet to list the resources running in Azure.</span></span> <span data-ttu-id="b1e5a-177">O exemplo seguinte mostra os recursos acabados de criar no novo grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-177">The following example shows the resources we just created in the new resource group.</span></span>

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

## <a name="deleting-resources"></a><span data-ttu-id="b1e5a-178">Eliminar recursos</span><span class="sxs-lookup"><span data-stu-id="b1e5a-178">Deleting resources</span></span>

<span data-ttu-id="b1e5a-179">Para limpar a sua conta do Azure, tem de remover os recursos criados neste exemplo.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-179">To clean up your Azure account, you want to remove the resources we created in this example.</span></span> <span data-ttu-id="b1e5a-180">Pode utilizar os cmdlets `Remove-AzureRm*` para eliminar recursos de que já não precisa.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-180">You can use the `Remove-AzureRm*` cmdlets to delete the resources you no longer need.</span></span> <span data-ttu-id="b1e5a-181">Para remover a VM do Windows criada, utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="b1e5a-181">To remove the Windows VM we created, using the following command:</span></span>

```azurepowershell-interactive
Remove-AzureRmVM -Name myWindowsVM -ResourceGroupName myResourceGroup
```

<span data-ttu-id="b1e5a-182">Ser-lhe-á pedido para confirmar se quer remover o recurso.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-182">You will be prompted to confirm that you want to remove the resource.</span></span>

```output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

<span data-ttu-id="b1e5a-183">Também pode utilizar o comando para eliminar muitos recursos ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-183">You can also use the delete many resources at one time.</span></span> <span data-ttu-id="b1e5a-184">Por exemplo, o comando seguinte elimina todos os recursos "MyResourceGroup" do grupo de recursos que utilizámos em todos os exemplos deste tutorial de Introdução.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-184">For example, the following command deletes all the resource group "MyResourceGroup" that we've used for all the samples in this Get Started tutorial.</span></span> <span data-ttu-id="b1e5a-185">Esta ação remove o grupo de recursos e todos os recursos no mesmo.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-185">This removes the resource group and all of the resources in it.</span></span>

```azurepowershell-interactive
Remove-AzureRmResourceGroup -Name myResourceGroup
```

```output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

<span data-ttu-id="b1e5a-186">Esta ação pode demorar vários minutos a concluir.</span><span class="sxs-lookup"><span data-stu-id="b1e5a-186">This can take several minutes to complete.</span></span>

## <a name="get-samples"></a><span data-ttu-id="b1e5a-187">Obter exemplos</span><span class="sxs-lookup"><span data-stu-id="b1e5a-187">Get samples</span></span>

<span data-ttu-id="b1e5a-188">Para saber mais sobre as formas como pode utilizar o Azure PowerShell, veja os nossos scripts mais comuns para [VMs do Linux](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Vms do Windows](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Aplicações Web](/azure/app-service-web/app-service-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json) e [Bases de Dados SQL](/azure/sql-database/sql-database-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json).</span><span class="sxs-lookup"><span data-stu-id="b1e5a-188">To learn more about ways to use the Azure PowerShell, check out our most common scripts for [Linux VMs](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Windows VMs](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Web Apps](/azure/app-service-web/app-service-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), and [SQL Databases](/azure/sql-database/sql-database-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json).</span></span>

## <a name="next-steps"></a><span data-ttu-id="b1e5a-189">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="b1e5a-189">Next steps</span></span>

* [<span data-ttu-id="b1e5a-190">Iniciar sessão com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b1e5a-190">Login with Azure PowerShell</span></span>](authenticate-azureps.md)
* [<span data-ttu-id="b1e5a-191">Gerir subscrições do Azure com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b1e5a-191">Manage Azure subscriptions with Azure PowerShell</span></span>](manage-subscriptions-azureps.md)
* [<span data-ttu-id="b1e5a-192">Criar principais de serviço no Azure com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b1e5a-192">Create service principals in Azure using Azure PowerShell</span></span>](create-azure-service-principal-azureps.md)
* <span data-ttu-id="b1e5a-193">Leia as Notas de versão sobre a migração de uma versão mais antiga: [https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes](https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes).</span><span class="sxs-lookup"><span data-stu-id="b1e5a-193">Read the Release notes about migrating from an older release: [https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes](https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes).</span></span>
* <span data-ttu-id="b1e5a-194">Obter ajuda da comunidade:</span><span class="sxs-lookup"><span data-stu-id="b1e5a-194">Get help from the community:</span></span>
  * [<span data-ttu-id="b1e5a-195">Fórum do Azure no MSDN</span><span class="sxs-lookup"><span data-stu-id="b1e5a-195">Azure forum on MSDN</span></span>](http://go.microsoft.com/fwlink/p/?LinkId=320212)
  * [<span data-ttu-id="b1e5a-196">Stackoverflow</span><span class="sxs-lookup"><span data-stu-id="b1e5a-196">stackoverflow</span></span>](http://go.microsoft.com/fwlink/?LinkId=320213)
