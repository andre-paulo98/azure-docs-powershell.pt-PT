---
title: Introdução ao Azure PowerShell
description: ''
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: get-started-article
ms.date: 10/30/2018
ms.openlocfilehash: 7367648a0a84cd5be5c7501ef4bf743a4290ce0f
ms.sourcegitcommit: 6685809f054203bd733c84f68acc69e53e5cca8c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/02/2019
ms.locfileid: "53982914"
---
# <a name="get-started-with-azure-powershell"></a><span data-ttu-id="24a47-102">Introdução ao Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="24a47-102">Get started with Azure PowerShell</span></span>

<span data-ttu-id="24a47-103">O Azure PowerShell foi concebido para gerir e administrar recursos do Azure a partir da linha de comandos e para criar scripts de automatização que funcionam no âmbito do Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="24a47-103">Azure PowerShell is designed for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="24a47-104">Pode utilizá-lo no seu browser com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou instalá-lo na máquina local.</span><span class="sxs-lookup"><span data-stu-id="24a47-104">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview) or you install it on your local machine.</span></span> <span data-ttu-id="24a47-105">Este artigo ajuda-o a começar a utilizar o Azure PowerShell e explica os principais conceitos que lhe estão subjacentes.</span><span class="sxs-lookup"><span data-stu-id="24a47-105">This article helps get you started with Azure PowerShell and teaches the core concepts behind it.</span></span>

## <a name="install-azure-powershell"></a><span data-ttu-id="24a47-106">Instalar o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="24a47-106">Install Azure PowerShell</span></span>

<span data-ttu-id="24a47-107">O primeiro passo é confirmar que tem instalada a versão mais recente do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="24a47-107">The first step is to make sure you have the latest version of the Azure PowerShell installed.</span></span> <span data-ttu-id="24a47-108">Para obter informações sobre a versão mais recente, veja as [notas de versão](./release-notes-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="24a47-108">For information about the latest release, see the [release notes](./release-notes-azureps.md).</span></span>

1. <span data-ttu-id="24a47-109">[Instalar o Azure PowerShell](install-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="24a47-109">[Install Azure PowerShell](install-az-ps.md).</span></span>

2. <span data-ttu-id="24a47-110">Para verificar se a instalação foi concluída com êxito, execute `Get-InstalledModule Az -AllVersions` na sua linha de comandos.</span><span class="sxs-lookup"><span data-stu-id="24a47-110">To verify the installation was successful, run `Get-InstalledModule Az -AllVersions` from your command line.</span></span>

## <a name="azure-cloud-shell"></a><span data-ttu-id="24a47-111">Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="24a47-111">Azure Cloud Shell</span></span>

<span data-ttu-id="24a47-112">A forma mais simples de começar é [iniciar a Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="24a47-112">The simplest way to get started is to [launch Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

1. <span data-ttu-id="24a47-113">Inicie o Cloud Shell a partir do menu de navegação superior do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="24a47-113">Launch Cloud Shell from the top navigation of the Azure portal.</span></span>

   ![Ícone do Shell](~/media/get-started-azureps/shell-icon.png)

2. <span data-ttu-id="24a47-115">Selecione a subscrição que quer utilizar e crie uma conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="24a47-115">Choose the subscription you want to use and create a storage account.</span></span>

   ![Criar uma conta de armazenamento](~/media/get-started-azureps/storage-prompt.png)

<span data-ttu-id="24a47-117">Assim que tiver sido criado o seu armazenamento, o Cloud Shell irá abrir uma sessão do PowerShell no browser.</span><span class="sxs-lookup"><span data-stu-id="24a47-117">Once your storage has been created, the Cloud Shell will open a PowerShell session in the browser.</span></span>

![Cloud Shell for PowerShell](~/media/get-started-azureps/cloud-powershell.png)

## <a name="sign-in-to-azure"></a><span data-ttu-id="24a47-119">Iniciar sessão no Azure</span><span class="sxs-lookup"><span data-stu-id="24a47-119">Sign in to Azure</span></span>

<span data-ttu-id="24a47-120">Inicie sessão interativamente:</span><span class="sxs-lookup"><span data-stu-id="24a47-120">Sign on interactively:</span></span>

1. <span data-ttu-id="24a47-121">Digite `Connect-AzAccount`.</span><span class="sxs-lookup"><span data-stu-id="24a47-121">Type `Connect-AzAccount`.</span></span> <span data-ttu-id="24a47-122">O argumento `-Environment` permite-lhe autenticar-se numa região ou cloud diferente.</span><span class="sxs-lookup"><span data-stu-id="24a47-122">The `-Environment` argument lets you authenticate for a different region or cloud.</span></span> <span data-ttu-id="24a47-123">Por exemplo, para se ligar ao Azure China:</span><span class="sxs-lookup"><span data-stu-id="24a47-123">For example, to connect to Azure China:</span></span>

    ```powershell-interactive
    Connect-AzAccount -Environment AzureChinaCloud
    ```

2. <span data-ttu-id="24a47-124">Obterá um token para utilizar em https://microsoft.com/devicelogin.</span><span class="sxs-lookup"><span data-stu-id="24a47-124">You'll get a token to use on https://microsoft.com/devicelogin.</span></span> <span data-ttu-id="24a47-125">Abra esta página no seu browser e introduza o token para iniciar sessão com as suas credenciais do Azure e autorizar o Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="24a47-125">Open this page in your browser and enter the token to sign in with your Azure credentials, and authorize Azure PowerShell.</span></span> 

<span data-ttu-id="24a47-126">Assim que tiver iniciado sessão numa conta do Azure, pode utilizar os cmdlets do Azure PowerShell para aceder e gerir os recursos na sua subscrição.</span><span class="sxs-lookup"><span data-stu-id="24a47-126">Once you have signed in to an Azure account, you can use the Azure PowerShell cmdlets to access and manage the resources in your subscription.</span></span> <span data-ttu-id="24a47-127">Para saber mais sobre o processo de início de sessão e os métodos de autenticação disponíveis, veja [Iniciar sessão com o Azure PowerShell](authenticate-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="24a47-127">To learn more about the sign in process and available authentication methods, see [Sign in with Azure PowerShell](authenticate-azureps.md).</span></span>

## <a name="create-a-windows-virtual-machine-using-simple-defaults"></a><span data-ttu-id="24a47-128">Criar uma máquina virtual do Windows com predefinições simples</span><span class="sxs-lookup"><span data-stu-id="24a47-128">Create a Windows virtual machine using simple defaults</span></span>

<span data-ttu-id="24a47-129">O cmdlet `New-AzVM` fornece uma sintaxe simplificada que facilita a criação de uma nova máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="24a47-129">The `New-AzVM` cmdlet provides a simplified syntax making it easy to create a new virtual machine.</span></span> <span data-ttu-id="24a47-130">Existem apenas dois valores de parâmetros que tem de fornecer: o nome da VM e um conjunto de credenciais para a conta de administrador local na VM.</span><span class="sxs-lookup"><span data-stu-id="24a47-130">There are only two parameter values you must provide: the name of the VM and a set of credentials for the local administrator account on the VM.</span></span>

<span data-ttu-id="24a47-131">Primeiro, crie o objeto de credencial.</span><span class="sxs-lookup"><span data-stu-id="24a47-131">First, create the credential object.</span></span>

```azurepowershell-interactive
$cred = Get-Credential -Message "Enter a username and password for the virtual machine."
```

```output
Windows PowerShell credential request.
Enter a username and password for the virtual machine.
User: localAdmin
Password for user localAdmin: *********
```

<span data-ttu-id="24a47-132">Em seguida, crie a VM.</span><span class="sxs-lookup"><span data-stu-id="24a47-132">Next, create the VM.</span></span>

```azurepowershell-interactive
New-AzVM -Name SampleVM -Credential $cred
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

<span data-ttu-id="24a47-133">Pode questionar-se sobre o que é criado e como a VM é configurada.</span><span class="sxs-lookup"><span data-stu-id="24a47-133">You may wonder what else is created and how is the VM configured.</span></span> <span data-ttu-id="24a47-134">Primeiro, vamos ver os nossos grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="24a47-134">First, let's look at our resource groups.</span></span>

```azurepowershell-interactive
Get-AzResourceGroup | Select-Object ResourceGroupName,Location
```

```output
ResourceGroupName          Location
-----------------          --------
cloud-shell-storage-westus westus
SampleVM                   eastus
```

<span data-ttu-id="24a47-135">É criado o grupo de recursos **cloud-shell-storage-westus** quando utilizar o Cloud Shell pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="24a47-135">The **cloud-shell-storage-westus** resource group is created the first time you use the Cloud Shell.</span></span> <span data-ttu-id="24a47-136">O grupo de recursos **SampleVM** foi criado pelo cmdlet `New-AzVM`.</span><span class="sxs-lookup"><span data-stu-id="24a47-136">The **SampleVM** resource group was created by the `New-AzVM` cmdlet.</span></span>

<span data-ttu-id="24a47-137">Agora, que outros recursos foram criados neste novo grupo de recursos?</span><span class="sxs-lookup"><span data-stu-id="24a47-137">Now, what other resources were created in this new resource group?</span></span>

```azurepowershell-interactive
Get-AzResource |
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

<span data-ttu-id="24a47-138">Vamos obter mais detalhes sobre a VM.</span><span class="sxs-lookup"><span data-stu-id="24a47-138">Let's get some more details about the VM.</span></span> <span data-ttu-id="24a47-139">Este exemplo mostra como obter informações sobre a Imagem do SO utilizada para criar a VM.</span><span class="sxs-lookup"><span data-stu-id="24a47-139">This example shows how to retrieve information about the OS Image used to create the VM.</span></span>

```azurepowershell-interactive
Get-AzVM -Name SampleVM -ResourceGroupName SampleVM |
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

## <a name="create-a-fully-configured-linux-virtual-machine"></a><span data-ttu-id="24a47-140">Criar uma Máquina Virtual do Linux totalmente configurada</span><span class="sxs-lookup"><span data-stu-id="24a47-140">Create a fully configured Linux Virtual Machine</span></span>

<span data-ttu-id="24a47-141">O exemplo anterior utilizou a sintaxe simplificada e os valores de parâmetros predefinidos para criar uma máquina virtual do Windows.</span><span class="sxs-lookup"><span data-stu-id="24a47-141">The previous example used the simplified syntax and default parameter values to create a Windows virtual machine.</span></span> <span data-ttu-id="24a47-142">Neste exemplo, fornecemos valores para todas as opções da máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="24a47-142">In this example, we provide values for all options of the virtual machine.</span></span>

### <a name="create-a-resource-group"></a><span data-ttu-id="24a47-143">Criar um grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="24a47-143">Create a resource group</span></span>

<span data-ttu-id="24a47-144">Neste exemplo, queremos criar um Grupo de Recursos.</span><span class="sxs-lookup"><span data-stu-id="24a47-144">In this example, we want to create a Resource Group.</span></span> <span data-ttu-id="24a47-145">Os Grupos de Recursos no Azure oferecem uma forma de gerir múltiplos recursos que quer agrupar logicamente.</span><span class="sxs-lookup"><span data-stu-id="24a47-145">Resource Groups in Azure provide a way to manage multiple resources that you want to logically group together.</span></span> <span data-ttu-id="24a47-146">Por exemplo, pode criar um Grupo de Recursos para uma aplicação ou projeto e adicionar uma máquina virtual, uma base de dados e um serviço de CDN ao mesmo.</span><span class="sxs-lookup"><span data-stu-id="24a47-146">For example, you might create a Resource Group for an application or project and add a virtual machine, a database and a CDN service within it.</span></span>

<span data-ttu-id="24a47-147">Vamos criar um grupo de recursos com o nome "MyResourceGroup" na região uswest2 do Azure.</span><span class="sxs-lookup"><span data-stu-id="24a47-147">Let's create a resource group named "MyResourceGroup" in the uswest2 region of Azure.</span></span> <span data-ttu-id="24a47-148">Para tal, escreva o comando seguinte:</span><span class="sxs-lookup"><span data-stu-id="24a47-148">To do so type the following command:</span></span>

```azurepowershell-interactive
New-AzResourceGroup -Name 'myResourceGroup' -Location 'westus2'
```

```output
ResourceGroupName : myResourceGroup
Location          : westus2
ProvisioningState : Succeeded
Tags              :
ResourceId        : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myResourceGroup
```

<span data-ttu-id="24a47-149">Este novo grupo de recursos será utilizado para conter todos os recursos necessários para a nova VM criada.</span><span class="sxs-lookup"><span data-stu-id="24a47-149">This new resource group will be used to contain all of the resources needed for the new VM we create.</span></span> <span data-ttu-id="24a47-150">Para criar uma nova VM do Linux, temos de criar primeiro os outros recursos que são precisos e atribuí-los a uma configuração.</span><span class="sxs-lookup"><span data-stu-id="24a47-150">To create a new Linux VM, we must first create the other required resources and assign them to a configuration.</span></span> <span data-ttu-id="24a47-151">Em seguida, podemos utilizar a configuração para criar a VM.</span><span class="sxs-lookup"><span data-stu-id="24a47-151">Then we can use that configuration to create the VM.</span></span> <span data-ttu-id="24a47-152">Além disso, terá de ter uma chave pública SSH com o nome `id_rsa.pub` no diretório `.ssh` do seu perfil de utilizador.</span><span class="sxs-lookup"><span data-stu-id="24a47-152">Also, you will need to have an SSH public key named `id_rsa.pub` in the `.ssh` directory of your user profile.</span></span>

#### <a name="create-the-required-network-resources"></a><span data-ttu-id="24a47-153">Criar os recursos de rede necessários</span><span class="sxs-lookup"><span data-stu-id="24a47-153">Create the required network resources</span></span>

<span data-ttu-id="24a47-154">Primeiro, temos de criar uma configuração de sub-rede a utilizar no processo de criação da rede virtual.</span><span class="sxs-lookup"><span data-stu-id="24a47-154">First we need to create a subnet configuration to be used with the virtual network creation process.</span></span> <span data-ttu-id="24a47-155">Também podemos criar um endereço IP público para podermos ligar a esta VM.</span><span class="sxs-lookup"><span data-stu-id="24a47-155">We also create a public IP address so that we can connect to this VM.</span></span> <span data-ttu-id="24a47-156">Vamos criar um grupo de segurança de rede para proteger o acesso ao endereço público.</span><span class="sxs-lookup"><span data-stu-id="24a47-156">We create a network security group to secure access to the public address.</span></span> <span data-ttu-id="24a47-157">Por fim, criamos o NIC virtual através de todos os recursos anteriores.</span><span class="sxs-lookup"><span data-stu-id="24a47-157">Finally we create the virtual NIC using all of the previous resources.</span></span>

```azurepowershell-interactive
# Variables for common values
$resourceGroup = "myResourceGroup"
$location = "westus2"
$vmName = "myLinuxVM"

# Definer user name and blank password
$securePassword = ConvertTo-SecureString 'azurepassword' -AsPlainText -Force
$cred = New-Object System.Management.Automation.PSCredential ("azureuser", $securePassword)

# Create a subnet configuration
$subnetConfig = New-AzVirtualNetworkSubnetConfig -Name mySubnet2 -AddressPrefix 192.168.2.0/24

# Create a virtual network
$vnet = New-AzVirtualNetwork -ResourceGroupName $resourceGroup -Location $location `
  -Name MYvNET2 -AddressPrefix 192.168.0.0/16 -Subnet $subnetConfig

# Create a public IP address and specify a DNS name
$publicIp = New-AzPublicIpAddress -ResourceGroupName $resourceGroup -Location $location `
  -Name "mypublicdns$(Get-Random)" -AllocationMethod Static -IdleTimeoutInMinutes 4
$publicIp | Select-Object Name,IpAddress

# Create an inbound network security group rule for port 22
$nsgRuleSSH = New-AzNetworkSecurityRuleConfig -Name myNetworkSecurityGroupRuleSSH  -Protocol Tcp `
  -Direction Inbound -Priority 1000 -SourceAddressPrefix * -SourcePortRange * -DestinationAddressPrefix * `
  -DestinationPortRange 22 -Access Allow

# Create a network security group
$nsg = New-AzNetworkSecurityGroup -ResourceGroupName $resourceGroup -Location $location `
  -Name myNetworkSecurityGroup2 -SecurityRules $nsgRuleSSH

# Create a virtual network card and associate with public IP address and NSG
$nic = New-AzNetworkInterface -Name myNic2 -ResourceGroupName $resourceGroup -Location $location `
  -SubnetId $vnet.Subnets[0].Id -PublicIpAddressId $publicIp.Id -NetworkSecurityGroupId $nsg.Id
```

### <a name="create-the-vm-configuration"></a><span data-ttu-id="24a47-158">Criar a configuração da VM</span><span class="sxs-lookup"><span data-stu-id="24a47-158">Create the VM configuration</span></span>

<span data-ttu-id="24a47-159">Agora que temos os recursos necessários, podemos criar o objeto de configuração da VM.</span><span class="sxs-lookup"><span data-stu-id="24a47-159">Now that we have the required resources we can create the VM configuration object.</span></span>

```azurepowershell-interactive
# Create a virtual machine configuration
$vmConfig = New-AzVMConfig -VMName $vmName -VMSize Standard_B1s |
  Set-AzVMOperatingSystem -Linux -ComputerName $vmName -Credential $cred -DisablePasswordAuthentication |
  Set-AzVMSourceImage -PublisherName Canonical -Offer UbuntuServer -Skus 14.04.2-LTS -Version latest |
  Add-AzVMNetworkInterface -Id $nic.Id

# Configure SSH Keys
$sshPublicKey = Get-Content -Raw "$env:USERPROFILE\.ssh\id_rsa.pub"
Add-AzVMSshPublicKey -VM $vmConfig -KeyData $sshPublicKey -Path "/home/azureuser/.ssh/authorized_keys"
```

### <a name="create-the-virtual-machine"></a><span data-ttu-id="24a47-160">Criar a máquina virtual</span><span class="sxs-lookup"><span data-stu-id="24a47-160">Create the virtual machine</span></span>

<span data-ttu-id="24a47-161">Agora, podemos criar a VM com o respetivo objeto de configuração.</span><span class="sxs-lookup"><span data-stu-id="24a47-161">Now we can create the VM using the VM configuration object.</span></span>

```azurepowershell-interactive
New-AzVM -ResourceGroupName $resourceGroup -Location $location -VM $vmConfig
```

<span data-ttu-id="24a47-162">Agora que a VM já está criada, pode iniciar sessão na sua nova VM do Linux através de SSH com o endereço IP público da VM que criou:</span><span class="sxs-lookup"><span data-stu-id="24a47-162">Now that the VM has been created, you can sign in to your new Linux VM using SSH with the public IP address of the VM you created:</span></span>

```powershell-interactive
ssh azureuser@$($publicIp.IpAddress)
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

## <a name="creating-other-resources-in-azure"></a><span data-ttu-id="24a47-163">Criar outros recursos no Azure</span><span class="sxs-lookup"><span data-stu-id="24a47-163">Creating other resources in Azure</span></span>

<span data-ttu-id="24a47-164">Acabámos de ver como são criados os Grupos de Recursos, as VMs do Linux e as VMs do Windows Server.</span><span class="sxs-lookup"><span data-stu-id="24a47-164">We've now walked through how to create a Resource Group, a Linux VM, and a Windows Server VM.</span></span> <span data-ttu-id="24a47-165">Também pode criar muitos outros tipos de recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="24a47-165">You can create many other types of Azure resources as well.</span></span>

<span data-ttu-id="24a47-166">Por exemplo, para criar um Balanceador de Carga da Rede do Azure que podemos, depois, associar às VMs acabadas de criar, podemos utilizar o comando de criação seguinte:</span><span class="sxs-lookup"><span data-stu-id="24a47-166">For example, to create an Azure Network Load Balancer that we could then associate with our newly created VMs, we can use the following create command:</span></span>

```azurepowershell-interactive
New-AzLoadBalancer -Name MyLoadBalancer -ResourceGroupName myResourceGroup -Location westus2
```

<span data-ttu-id="24a47-167">Também podemos criar uma Rede Virtual privada nova (geralmente conhecida como “VNet” no Azure) para a nossa infraestrutura, utilizando o comando seguinte:</span><span class="sxs-lookup"><span data-stu-id="24a47-167">We could also create a new private Virtual Network (commonly referred to as a "VNet" within Azure) for our infrastructure using the following command:</span></span>

```azurepowershell-interactive
$subnetConfig = New-AzVirtualNetworkSubnetConfig -Name mySubnet2 -AddressPrefix 10.0.0.0/16
$vnet = New-AzVirtualNetwork -ResourceGroupName myResourceGroup -Location westus2 `
  -Name MYvNET3 -AddressPrefix 10.0.0.0/16 -Subnet $subnetConfig
```

<span data-ttu-id="24a47-168">O que torna o Azure e o Azure PowerShell poderosos é o facto de poderem ser utilizados não só para obter a infraestrutura baseada na cloud, como também para criar serviços de plataformas geridos.</span><span class="sxs-lookup"><span data-stu-id="24a47-168">What makes Azure and the Azure PowerShell powerful is that we can use it not just to get cloud-based infrastructure but also to create managed platform services.</span></span> <span data-ttu-id="24a47-169">Os serviços de plataforma geridos podem, igualmente, ser combinados com a infraestrutura, para criar soluções ainda mais poderosas.</span><span class="sxs-lookup"><span data-stu-id="24a47-169">The managed platform services can also be combined with infrastructure to build even more powerful solutions.</span></span>

<span data-ttu-id="24a47-170">Por exemplo, pode utilizar o Azure PowerShell para criar um AppService do Azure.</span><span class="sxs-lookup"><span data-stu-id="24a47-170">For example, you can use the Azure PowerShell to create an Azure AppService.</span></span> <span data-ttu-id="24a47-171">O AppService do Azure é um serviço de plataforma gerido que proporciona uma excelente forma de alojar aplicações Web sem que tenha de se preocupar com a infraestrutura.</span><span class="sxs-lookup"><span data-stu-id="24a47-171">Azure AppService is a managed platform service that provides a great way to host web apps without having to worry about infrastructure.</span></span> <span data-ttu-id="24a47-172">Depois de criar o AppService do Azure, pode criar duas novas Aplicações Web do Azure no AppService com os comandos seguintes:</span><span class="sxs-lookup"><span data-stu-id="24a47-172">After creating the Azure AppService, you can create two new Azure Web Apps within the AppService using the following commands:</span></span>

```azurepowershell-interactive
# Get a UUID for creating the apps to avoid name conflicts
$guid = [System.Guid]::NewGuid().ToString()

# Create an Azure AppService that we can host any number of web apps within
New-AzAppServicePlan -Name MyAppServicePlan -Tier Basic -NumberofWorkers 2 -WorkerSize Small -ResourceGroupName myResourceGroup -Location westus2

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
New-AzWebApp -Name MyWebApp-$guid -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westus2
New-AzWebApp -Name MyWebApp2-$guid -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westus2
```

## <a name="listing-deployed-resources"></a><span data-ttu-id="24a47-173">Listar recursos implementados</span><span class="sxs-lookup"><span data-stu-id="24a47-173">Listing deployed resources</span></span>

<span data-ttu-id="24a47-174">Pode utilizar o cmdlet `Get-AzResource` para listar os recursos em execução no Azure.</span><span class="sxs-lookup"><span data-stu-id="24a47-174">You can use the `Get-AzResource` cmdlet to list the resources running in Azure.</span></span> <span data-ttu-id="24a47-175">O exemplo seguinte mostra os recursos criados no novo grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="24a47-175">The following example shows the resources we created in the new resource group.</span></span>

```azurepowershell-interactive
Get-AzResource |
  Where-Object ResourceGroupName -eq myResourceGroup |
    Select-Object Name,Location,ResourceType
```

```output
Name                                                  Location   ResourceType
----                                                  --------   ------------
myLinuxVM_OsDisk_1_36ca038791f642ba91270879088c249a   westus2 Microsoft.Compute/disks
myWindowsVM_OsDisk_1_f627e6e2bb454c72897d72e9632adf9a westus2 Microsoft.Compute/disks
myLinuxVM                                             westus2 Microsoft.Compute/virtualMachines
myWindowsVM                                           westus2 Microsoft.Compute/virtualMachines
myWindowsVM/BGInfo                                    westus2 Microsoft.Compute/virtualMachines/extensions
myNic1                                                westus2 Microsoft.Network/networkInterfaces
myNic2                                                westus2 Microsoft.Network/networkInterfaces
myNetworkSecurityGroup1                               westus2 Microsoft.Network/networkSecurityGroups
myNetworkSecurityGroup2                               westus2 Microsoft.Network/networkSecurityGroups
mypublicdns245369171                                  westus2 Microsoft.Network/publicIPAddresses
mypublicdns779537141                                  westus2 Microsoft.Network/publicIPAddresses
MYvNET1                                               westus2 Microsoft.Network/virtualNetworks
MYvNET2                                               westus2 Microsoft.Network/virtualNetworks
micromyresomywi032907510                              westus2 Microsoft.Storage/storageAccounts
```

## <a name="deleting-resources"></a><span data-ttu-id="24a47-176">Eliminar recursos</span><span class="sxs-lookup"><span data-stu-id="24a47-176">Deleting resources</span></span>

<span data-ttu-id="24a47-177">Para limpar a sua conta do Azure, tem de remover os recursos criados neste exemplo.</span><span class="sxs-lookup"><span data-stu-id="24a47-177">To clean up your Azure account, you want to remove the resources we created in this example.</span></span> <span data-ttu-id="24a47-178">Pode utilizar os cmdlets `Remove-Az*` para eliminar recursos de que já não precisa.</span><span class="sxs-lookup"><span data-stu-id="24a47-178">You can use the `Remove-Az*` cmdlets to delete the resources you no longer need.</span></span> <span data-ttu-id="24a47-179">Para remover a VM do Windows criada, utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="24a47-179">To remove the Windows VM we created, using the following command:</span></span>

```azurepowershell-interactive
Remove-AzVM -Name myWindowsVM -ResourceGroupName myResourceGroup
```

<span data-ttu-id="24a47-180">Ser-lhe-á pedido para confirmar se quer remover o recurso.</span><span class="sxs-lookup"><span data-stu-id="24a47-180">You'll be prompted to confirm that you want to remove the resource.</span></span>

```output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

<span data-ttu-id="24a47-181">Também pode eliminar muitos recursos de uma só vez.</span><span class="sxs-lookup"><span data-stu-id="24a47-181">You can also delete many resources at once.</span></span> <span data-ttu-id="24a47-182">Por exemplo, o comando seguinte elimina o grupo de recursos "MyResourceGroup" que utilizámos em todos os exemplos até agora.</span><span class="sxs-lookup"><span data-stu-id="24a47-182">For example, the following command deletes the resource group "MyResourceGroup" that we've used for all the samples so far.</span></span>
<span data-ttu-id="24a47-183">Todos os recursos no grupo também são eliminados.</span><span class="sxs-lookup"><span data-stu-id="24a47-183">All resources in the group are also deleted.</span></span>

```azurepowershell-interactive
Remove-AzResourceGroup -Name myResourceGroup
```

```output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

<span data-ttu-id="24a47-184">A tarefa pode demorar vários minutos a concluir, consoante o número e o tipo de recursos.</span><span class="sxs-lookup"><span data-stu-id="24a47-184">The task can take several minutes to complete, depending on the number and type of resources.</span></span>

## <a name="get-samples"></a><span data-ttu-id="24a47-185">Obter exemplos</span><span class="sxs-lookup"><span data-stu-id="24a47-185">Get samples</span></span>

<span data-ttu-id="24a47-186">Para saber mais sobre as formas como pode utilizar o Azure PowerShell, veja os nossos scripts mais comuns para [VMs do Linux](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Vms do Windows](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Aplicações Web](/azure/app-service-web/app-service-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json) e [Bases de Dados SQL](/azure/sql-database/sql-database-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json).</span><span class="sxs-lookup"><span data-stu-id="24a47-186">To learn more about ways to use the Azure PowerShell, check out our most common scripts for [Linux VMs](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Windows VMs](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Web Apps](/azure/app-service-web/app-service-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), and [SQL Databases](/azure/sql-database/sql-database-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json).</span></span>

## <a name="next-steps"></a><span data-ttu-id="24a47-187">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="24a47-187">Next steps</span></span>

* [<span data-ttu-id="24a47-188">Iniciar sessão com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="24a47-188">Sign in with Azure PowerShell</span></span>](authenticate-azureps.md)
* [<span data-ttu-id="24a47-189">Gerir subscrições do Azure com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="24a47-189">Manage Azure subscriptions with Azure PowerShell</span></span>](manage-subscriptions-azureps.md)
* [<span data-ttu-id="24a47-190">Criar principais de serviço no Azure com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="24a47-190">Create service principals in Azure using Azure PowerShell</span></span>](create-azure-service-principal-azureps.md)
* <span data-ttu-id="24a47-191">Obter ajuda da comunidade:</span><span class="sxs-lookup"><span data-stu-id="24a47-191">Get help from the community:</span></span>
  * [<span data-ttu-id="24a47-192">Fórum do Azure no MSDN</span><span class="sxs-lookup"><span data-stu-id="24a47-192">Azure forum on MSDN</span></span>](http://go.microsoft.com/fwlink/p/?LinkId=320212)
  * [<span data-ttu-id="24a47-193">Stackoverflow</span><span class="sxs-lookup"><span data-stu-id="24a47-193">stackoverflow</span></span>](http://go.microsoft.com/fwlink/?LinkId=320213)
