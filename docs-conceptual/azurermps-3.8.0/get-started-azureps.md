---
title: Introdução ao Azure PowerShell | Microsoft Docs
description: ''
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: get-started-article
ms.date: 11/15/2017
ms.openlocfilehash: 3a0d3d1d970f4458e66167fb55c840598ce59e13
ms.sourcegitcommit: 990f82648b0aa2e970f96c02466a7134077c8c56
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/11/2018
ms.locfileid: "38100295"
---
# <a name="getting-started-with-azure-powershell"></a><span data-ttu-id="4c849-102">Introdução ao Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="4c849-102">Getting started with Azure PowerShell</span></span>

<span data-ttu-id="4c849-103">O Azure PowerShell foi concebido para gerir e administrar recursos do Azure a partir da linha de comandos e para criar scripts de automatização que funcionam no âmbito do Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="4c849-103">Azure PowerShell is designed for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="4c849-104">Pode utilizá-lo no seu browser com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou pode instalá-lo no seu computador local e utilizá-lo em qualquer sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4c849-104">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can install it on your local machine and use it in any PowerShell session.</span></span> <span data-ttu-id="4c849-105">Este artigo ajuda-o a começar a utilizá-lo e explica-lhe os conceitos principais subjacentes.</span><span class="sxs-lookup"><span data-stu-id="4c849-105">This article helps get you started using it, and teaches you the core concepts behind it.</span></span>

## <a name="connect"></a><span data-ttu-id="4c849-106">Ligar</span><span class="sxs-lookup"><span data-stu-id="4c849-106">Connect</span></span>

<span data-ttu-id="4c849-107">A forma mais simples de começar é [iniciar a Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="4c849-107">The simplest way to get started is to [launch Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

1. <span data-ttu-id="4c849-108">Inicie o Cloud Shell a partir do menu de navegação superior do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="4c849-108">Launch Cloud Shell from the top navigation of the Azure portal.</span></span>

   ![Ícone do Shell](~/media/get-started-azureps/shell-icon.png)

2. <span data-ttu-id="4c849-110">Selecione a subscrição que quer utilizar e crie uma conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="4c849-110">Choose the subscription you want to use and create a storage account.</span></span>

   ![Criar uma conta de armazenamento](~/media/get-started-azureps/storage-prompt.png)

<span data-ttu-id="4c849-112">Assim que tiver sido criado o seu armazenamento, o Cloud Shell irá abrir uma sessão do PowerShell no browser.</span><span class="sxs-lookup"><span data-stu-id="4c849-112">Once your storage has been created, the Cloud Shell will open a PowerShell session in the browser.</span></span>

![Cloud Shell para PowerShell](~/media/get-started-azureps/cloud-powershell.png)

<span data-ttu-id="4c849-114">Também pode instalar o Azure PowerShell e utilizá-lo localmente numa sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4c849-114">You can also install Azure PowerShell and use it locally in a PowerShell session.</span></span>

## <a name="install-azure-powershell"></a><span data-ttu-id="4c849-115">Instalar o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="4c849-115">Install Azure PowerShell</span></span>

<span data-ttu-id="4c849-116">O primeiro passo é confirmar que tem instalada a versão mais recente do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4c849-116">The first step is to make sure you have the latest version of the Azure PowerShell installed.</span></span> <span data-ttu-id="4c849-117">Para obter informações sobre a versão mais recente, veja as [notas de versão](./release-notes-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="4c849-117">For information about the latest release, see the [release notes](./release-notes-azureps.md).</span></span>

1. <span data-ttu-id="4c849-118">[Instalar o Azure PowerShell](install-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="4c849-118">[Install Azure PowerShell](install-azurerm-ps.md).</span></span>

2. <span data-ttu-id="4c849-119">Para verificar se a instalação foi concluída com êxito, execute `Get-Module AzureRM -ListAvailable` na sua linha de comandos.</span><span class="sxs-lookup"><span data-stu-id="4c849-119">To verify the installation was successful, run `Get-Module AzureRM -ListAvailable` from your command line.</span></span>

## <a name="log-in-to-azure"></a><span data-ttu-id="4c849-120">Iniciar sessão no Azure</span><span class="sxs-lookup"><span data-stu-id="4c849-120">Log in to Azure</span></span>

<span data-ttu-id="4c849-121">Inicie sessão interativamente:</span><span class="sxs-lookup"><span data-stu-id="4c849-121">Sign on interactively:</span></span>

1. <span data-ttu-id="4c849-122">Digite `Login-AzureRmAccount`.</span><span class="sxs-lookup"><span data-stu-id="4c849-122">Type `Login-AzureRmAccount`.</span></span> <span data-ttu-id="4c849-123">Obterá uma caixa de diálogo a solicitar as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="4c849-123">You will get dialog box asking for your Azure credentials.</span></span> <span data-ttu-id="4c849-124">A opção “-EnvironmentName” permite-lhe iniciar sessão no Azure China ou Azure Alemanha.</span><span class="sxs-lookup"><span data-stu-id="4c849-124">Option '-EnvironmentName' can let you login in Azure China or Azure Germany.</span></span>

   <span data-ttu-id="4c849-125">Por exemplo, Login-AzureRmAccount -EnvironmentName AzureChinaCloud</span><span class="sxs-lookup"><span data-stu-id="4c849-125">e.g. Login-AzureRmAccount -EnvironmentName AzureChinaCloud</span></span>

2. <span data-ttu-id="4c849-126">Escreva o endereço de e-mail e a palavra-passe associados à sua conta.</span><span class="sxs-lookup"><span data-stu-id="4c849-126">Type the email address and password associated with your account.</span></span> <span data-ttu-id="4c849-127">O Azure autentica e guarda as informações das credenciais e, em seguida, fecha a janela.</span><span class="sxs-lookup"><span data-stu-id="4c849-127">Azure authenticates and saves the credential information, and then closes the window.</span></span>

<span data-ttu-id="4c849-128">Assim que tiver iniciado sessão numa conta do Azure, pode utilizar os cmdlets do Azure PowerShell para aceder e gerir os recursos na sua subscrição.</span><span class="sxs-lookup"><span data-stu-id="4c849-128">Once you have signed in to an Azure account, you can use the Azure PowerShell cmdlets to access and manager the resources in your subscription.</span></span>

## <a name="create-a-resource-group"></a><span data-ttu-id="4c849-129">Criar um grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="4c849-129">Create a resource group</span></span>

<span data-ttu-id="4c849-130">Agora que já está tudo configurado, vamos utilizar o Azure PowerShell para criar recursos no Azure.</span><span class="sxs-lookup"><span data-stu-id="4c849-130">Now that we've got everything set up, let's use Azure PowerShell to create resources within Azure.</span></span>

<span data-ttu-id="4c849-131">Comece por criar um Grupo de Recursos.</span><span class="sxs-lookup"><span data-stu-id="4c849-131">First, create a Resource Group.</span></span> <span data-ttu-id="4c849-132">Os Grupos de Recursos no Azure oferecem uma forma de gerir múltiplos recursos que quer agrupar logicamente.</span><span class="sxs-lookup"><span data-stu-id="4c849-132">Resource Groups in Azure provide a way to manage multiple resources that you want to logically group together.</span></span> <span data-ttu-id="4c849-133">Por exemplo, pode criar um Grupo de Recursos para uma aplicação ou projeto e adicionar uma máquina virtual, uma base de dados e um serviço de CDN ao mesmo.</span><span class="sxs-lookup"><span data-stu-id="4c849-133">For example, you might create a Resource Group for an application or project and add a virtual machine, a database and a CDN service within it.</span></span>

<span data-ttu-id="4c849-134">Vamos criar um grupo de recursos com o nome “MyResourceGroup" na região westeurope do Azure.</span><span class="sxs-lookup"><span data-stu-id="4c849-134">Let's create a resource group named "MyResourceGroup" in the westeurope region of Azure.</span></span> <span data-ttu-id="4c849-135">Para tal, escreva o comando seguinte:</span><span class="sxs-lookup"><span data-stu-id="4c849-135">To do so type the following command:</span></span>

```powershell
New-AzureRmResourceGroup -Name 'myResourceGroup' -Location 'westeurope'
```

```Output
ResourceGroupName : myResourceGroup
Location          : westeurope
ProvisioningState : Succeeded
Tags              :
ResourceId        : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myResourceGroup
```

## <a name="create-a-windows-virtual-machine"></a><span data-ttu-id="4c849-136">Criar uma Máquina Virtual do Windows</span><span class="sxs-lookup"><span data-stu-id="4c849-136">Create a Windows Virtual Machine</span></span>

<span data-ttu-id="4c849-137">Agora que temos o nosso grupo de recursos, vamos criar uma VM do Windows no mesmo.</span><span class="sxs-lookup"><span data-stu-id="4c849-137">Now that we have our resource group, let's create a Windows VM within it.</span></span> <span data-ttu-id="4c849-138">Para criar uma nova VM, temos de criar primeiro os outros recursos necessários e atribuí-los a uma configuração.</span><span class="sxs-lookup"><span data-stu-id="4c849-138">To create a new VM we must first create the other required resources and assign them to a configuration.</span></span> <span data-ttu-id="4c849-139">Em seguida, podemos utilizar a configuração para criar a VM.</span><span class="sxs-lookup"><span data-stu-id="4c849-139">Then we can use that configuration to create the VM.</span></span>

### <a name="create-the-required-network-resources"></a><span data-ttu-id="4c849-140">Criar os recursos de rede necessários</span><span class="sxs-lookup"><span data-stu-id="4c849-140">Create the required network resources</span></span>

<span data-ttu-id="4c849-141">Primeiro, temos de criar uma configuração de sub-rede a utilizar no processo de criação da rede virtual.</span><span class="sxs-lookup"><span data-stu-id="4c849-141">First we need to create a subnet configuration to be used with the virtual network creation process.</span></span> <span data-ttu-id="4c849-142">Também podemos criar um endereço IP público para podermos ligar a esta VM.</span><span class="sxs-lookup"><span data-stu-id="4c849-142">We also create a public IP address so that we can connect to this VM.</span></span> <span data-ttu-id="4c849-143">Vamos criar um grupo de segurança de rede para proteger o acesso ao endereço público.</span><span class="sxs-lookup"><span data-stu-id="4c849-143">We create a network security group to secure access to the public address.</span></span> <span data-ttu-id="4c849-144">Por fim, criamos o NIC virtual através de todos os recursos anteriores.</span><span class="sxs-lookup"><span data-stu-id="4c849-144">Finally we create the virtual NIC using all of the previous resources.</span></span>

```powershell
# Variables for common values
$resourceGroup = "myResourceGroup"
$location = "westeurope"
$vmName = "myWindowsVM"

# Create a subnet configuration
$subnetConfig = New-AzureRmVirtualNetworkSubnetConfig -Name mySubnet1 -AddressPrefix 192.168.1.0/24

# Create a virtual network
$vnet = New-AzureRmVirtualNetwork -ResourceGroupName $resourceGroup -Location $location `
  -Name MYvNET1 -AddressPrefix 192.168.0.0/16 -Subnet $subnetConfig

# Create a public IP address and specify a DNS name
$publicIp = New-AzureRmPublicIpAddress -ResourceGroupName $resourceGroup -Location $location `
  -Name "mypublicdns$(Get-Random)" -AllocationMethod Static -IdleTimeoutInMinutes 4
$publicIp | Select-Object Name,IpAddress

# Create an inbound network security group rule for port 3389
$nsgRuleRDP = New-AzureRmNetworkSecurityRuleConfig -Name myNetworkSecurityGroupRuleRDP  -Protocol Tcp `
  -Direction Inbound -Priority 1000 -SourceAddressPrefix * -SourcePortRange * -DestinationAddressPrefix * `
  -DestinationPortRange 3389 -Access Allow

# Create a network security group
$nsg = New-AzureRmNetworkSecurityGroup -ResourceGroupName $resourceGroup -Location $location `
  -Name myNetworkSecurityGroup1 -SecurityRules $nsgRuleRDP

# Create a virtual network card and associate with public IP address and NSG
$nic = New-AzureRmNetworkInterface -Name myNic1 -ResourceGroupName $resourceGroup -Location $location `
  -SubnetId $vnet.Subnets[0].Id -PublicIpAddressId $publicIp.Id -NetworkSecurityGroupId $nsg.Id
```

### <a name="create-the-virtual-machine"></a><span data-ttu-id="4c849-145">Criar a máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c849-145">Create the virtual machine</span></span>

<span data-ttu-id="4c849-146">Primeiro, é necessário um conjunto de credenciais para o sistema operativo.</span><span class="sxs-lookup"><span data-stu-id="4c849-146">First we need a set of credentials for the OS.</span></span>

```powershell
# Create user object
$cred = Get-Credential -Message "Enter a username and password for the virtual machine."
```

<span data-ttu-id="4c849-147">Agora que temos os recursos necessários, podemos criar a VM.</span><span class="sxs-lookup"><span data-stu-id="4c849-147">Now that we have the required resources we can create the VM.</span></span> <span data-ttu-id="4c849-148">Para este passo, criamos um objeto de configuração de VM e, em seguida, utilizamos a configuração para criar a VM.</span><span class="sxs-lookup"><span data-stu-id="4c849-148">For this step, we create a VM configuration object, then we use the configuration to create the VM.</span></span>

```powershell
# Create a virtual machine configuration
$vmConfig = New-AzureRmVMConfig -VMName $vmName -VMSize Standard_D1 |
  Set-AzureRmVMOperatingSystem -Windows -ComputerName $vmName -Credential $cred |
  Set-AzureRmVMSourceImage -PublisherName MicrosoftWindowsServer -Offer WindowsServer -Skus 2016-Datacenter -Version latest |
  Add-AzureRmVMNetworkInterface -Id $nic.Id

# Create a virtual machine
New-AzureRmVM -ResourceGroupName $resourceGroup -Location $location -VM $vmConfig
```

<span data-ttu-id="4c849-149">O comando `New-AzureRmVM` gera o resultado assim que a VM tiver sido totalmente criada e estiver pronta para ser utilizada.</span><span class="sxs-lookup"><span data-stu-id="4c849-149">The `New-AzureRmVM` command outputs results once the VM has been fully created and is ready to be used.</span></span>

```Output
RequestId IsSuccessStatusCode StatusCode ReasonPhrase
--------- ------------------- ---------- ------------
                         True         OK OK
```

<span data-ttu-id="4c849-150">Agora, inicie sessão na VM do Windows Server acabada de criar com o Ambiente de Trabalho Remoto e o endereço IP público da VM.</span><span class="sxs-lookup"><span data-stu-id="4c849-150">Now log on to your newly created Windows Server VM using Remote Desktop and the public IP address of the VM.</span></span> <span data-ttu-id="4c849-151">O comando seguinte apresenta o endereço IP público criado no script anterior.</span><span class="sxs-lookup"><span data-stu-id="4c849-151">The following command displays the public IP address created in the previous script.</span></span>

```powershell
$publicIp | Select-Object Name,IpAddress
```

```Output
Name                  IpAddress
----                  ---------
mypublicdns1400512543 xx.xx.xx.xx
```

<span data-ttu-id="4c849-152">Se estiver num sistema baseado no Windows, pode fazê-lo a partir da linha de comandos com o comando mstsc:</span><span class="sxs-lookup"><span data-stu-id="4c849-152">If you are on a Windows-based system, you can do this from the command line using the mstsc command:</span></span>

```powershell
mstsc /v:xx.xxx.xx.xxx
```

<span data-ttu-id="4c849-153">Indique a combinação de nome de utilizador/palavra-passe que utilizou quando criou a VM para iniciar sessão.</span><span class="sxs-lookup"><span data-stu-id="4c849-153">Supply the same username/password combination you used when creating the VM to log in.</span></span>

## <a name="create-a-linux-virtual-machine"></a><span data-ttu-id="4c849-154">Criar uma Máquina Virtual do Linux</span><span class="sxs-lookup"><span data-stu-id="4c849-154">Create a Linux Virtual Machine</span></span>

<span data-ttu-id="4c849-155">Para criar uma nova VM do Linux, temos de criar primeiro os outros recursos necessários e atribuí-los a uma configuração.</span><span class="sxs-lookup"><span data-stu-id="4c849-155">To create a new Linux VM we must first create the other required resources and assign them to a configuration.</span></span> <span data-ttu-id="4c849-156">Em seguida, podemos utilizar a configuração para criar a VM.</span><span class="sxs-lookup"><span data-stu-id="4c849-156">Then we can use that configuration to create the VM.</span></span> <span data-ttu-id="4c849-157">Tal pressupõe que já criou o grupo de recursos, conforme mostrado anteriormente.</span><span class="sxs-lookup"><span data-stu-id="4c849-157">This assumes that you have already created the resource group as previously shown.</span></span> <span data-ttu-id="4c849-158">Além disso, terá de ter uma chave pública SSH com o nome `id_rsa.pub` no diretório .ssh do seu perfil de utilizador.</span><span class="sxs-lookup"><span data-stu-id="4c849-158">Also, you will need to have an SSH public key named `id_rsa.pub` in the .ssh directory of your user profile.</span></span>

### <a name="create-the-required-network-resources"></a><span data-ttu-id="4c849-159">Criar os recursos de rede necessários</span><span class="sxs-lookup"><span data-stu-id="4c849-159">Create the required network resources</span></span>

<span data-ttu-id="4c849-160">Primeiro, temos de criar uma configuração de sub-rede a utilizar no processo de criação da rede virtual.</span><span class="sxs-lookup"><span data-stu-id="4c849-160">First we need to create a subnet configuration to be used with the virtual network creation process.</span></span> <span data-ttu-id="4c849-161">Também podemos criar um endereço IP público para podermos ligar a esta VM.</span><span class="sxs-lookup"><span data-stu-id="4c849-161">We also create a public IP address so that we can connect to this VM.</span></span> <span data-ttu-id="4c849-162">Vamos criar um grupo de segurança de rede para proteger o acesso ao endereço público.</span><span class="sxs-lookup"><span data-stu-id="4c849-162">We create a network security group to secure access to the public address.</span></span> <span data-ttu-id="4c849-163">Por fim, criamos o NIC virtual através de todos os recursos anteriores.</span><span class="sxs-lookup"><span data-stu-id="4c849-163">Finally we create the virtual NIC using all of the previous resources.</span></span>

```powershell
# Variables for common values
$resourceGroup = "myResourceGroup"
$location = "westeurope"
$vmName = "myLinuxVM"

# Definer user name and blank password
$securePassword = ConvertTo-SecureString ' ' -AsPlainText -Force
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

### <a name="create-the-virtual-machine"></a><span data-ttu-id="4c849-164">Criar a máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4c849-164">Create the virtual machine</span></span>

<span data-ttu-id="4c849-165">Agora que temos os recursos necessários, podemos criar a VM.</span><span class="sxs-lookup"><span data-stu-id="4c849-165">Now that we have the required resources we can create the VM.</span></span> <span data-ttu-id="4c849-166">Para este passo, criamos um objeto de configuração de VM e, em seguida, utilizamos a configuração para criar a VM.</span><span class="sxs-lookup"><span data-stu-id="4c849-166">For this step, we create a VM configuration object, then we use the configuration to create the VM.</span></span>

```powershell
# Create a virtual machine configuration
$vmConfig = New-AzureRmVMConfig -VMName $vmName -VMSize Standard_D1 |
  Set-AzureRmVMOperatingSystem -Linux -ComputerName $vmName -Credential $cred -DisablePasswordAuthentication |
  Set-AzureRmVMSourceImage -PublisherName Canonical -Offer UbuntuServer -Skus 14.04.2-LTS -Version latest |
  Add-AzureRmVMNetworkInterface -Id $nic.Id

# Configure SSH Keys
$sshPublicKey = Get-Content "$env:USERPROFILE\.ssh\id_rsa.pub"
Add-AzureRmVMSshPublicKey -VM $vmConfig -KeyData $sshPublicKey -Path "/home/azureuser/.ssh/authorized_keys"

# Create a virtual machine
New-AzureRmVM -ResourceGroupName $resourceGroup -Location $location -VM $vmConfig
```

<span data-ttu-id="4c849-167">Agora que a VM já está criada, pode iniciar sessão na sua nova VM do Linux através de SSH com o endereço IP público da VM que criou:</span><span class="sxs-lookup"><span data-stu-id="4c849-167">Now that the VM has been created, you can log on to your new Linux VM using SSH with the public IP address of the VM you created:</span></span>

```bash
ssh xx.xxx.xxx.xxx
```

```Output
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

## <a name="creating-other-resources-in-azure"></a><span data-ttu-id="4c849-168">Criar outros recursos no Azure</span><span class="sxs-lookup"><span data-stu-id="4c849-168">Creating other resources in Azure</span></span>

<span data-ttu-id="4c849-169">Acabámos de ver como são criados os Grupos de Recursos, as VMs do Linux e as VMs do Windows Server.</span><span class="sxs-lookup"><span data-stu-id="4c849-169">We've now walked through how to create a Resource Group, a Linux VM, and a Windows Server VM.</span></span> <span data-ttu-id="4c849-170">Também pode criar muitos outros tipos de recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="4c849-170">You can create many other types of Azure resources as well.</span></span>

<span data-ttu-id="4c849-171">Por exemplo, para criar um Balanceador de Carga da Rede do Azure que podemos, depois, associar às VMs acabadas de criar, podemos utilizar o comando de criação seguinte:</span><span class="sxs-lookup"><span data-stu-id="4c849-171">For example, to create an Azure Network Load Balancer that we could then associate with our newly created VMs, we can use the following create command:</span></span>

```powershell
New-AzureRmLoadBalancer -Name MyLoadBalancer -ResourceGroupName myResourceGroup -Location westeurope
```

<span data-ttu-id="4c849-172">Também podemos criar uma Rede Virtual privada nova (geralmente conhecida como “VNet” no Azure) para a nossa infraestrutura, utilizando o comando seguinte:</span><span class="sxs-lookup"><span data-stu-id="4c849-172">We could also create a new private Virtual Network (commonly referred to as a "VNet" within Azure) for our infrastructure using the following command:</span></span>

```powershell
$subnetConfig = New-AzureRmVirtualNetworkSubnetConfig -Name mySubnet2 -AddressPrefix 10.0.0.0/16
$vnet = New-AzureRmVirtualNetwork -ResourceGroupName myResourceGroup -Location westeurope `
  -Name MYvNET3 -AddressPrefix 10.0.0.0/16 -Subnet $subnetConfig
```

<span data-ttu-id="4c849-173">O que torna o Azure e o Azure PowerShell poderosos é o facto de poderem ser utilizados não só para obter a infraestrutura baseada na cloud, como também para criar serviços de plataformas geridos.</span><span class="sxs-lookup"><span data-stu-id="4c849-173">What makes Azure and the Azure PowerShell powerful is that we can use it not just to get cloud-based infrastructure but also to create managed platform services.</span></span> <span data-ttu-id="4c849-174">Os serviços de plataforma geridos podem, igualmente, ser combinados com a infraestrutura, para criar soluções ainda mais poderosas.</span><span class="sxs-lookup"><span data-stu-id="4c849-174">The managed platform services can also be combined with infrastructure to build even more powerful solutions.</span></span>

<span data-ttu-id="4c849-175">Por exemplo, pode utilizar o Azure PowerShell para criar um AppService do Azure.</span><span class="sxs-lookup"><span data-stu-id="4c849-175">For example, you can use the Azure PowerShell to create an Azure AppService.</span></span> <span data-ttu-id="4c849-176">O AppService do Azure é um serviço de plataforma gerido que proporciona uma excelente forma de alojar aplicações Web sem que tenha de se preocupar com a infraestrutura.</span><span class="sxs-lookup"><span data-stu-id="4c849-176">Azure AppService is a managed platform service that provides a great way to host web apps without having to worry about infrastructure.</span></span> <span data-ttu-id="4c849-177">Depois de criar o AppService do Azure, pode criar duas novas Aplicações Web do Azure no AppService com os comandos seguintes:</span><span class="sxs-lookup"><span data-stu-id="4c849-177">After creating the Azure AppService, you can create two new Azure Web Apps within the AppService using the following commands:</span></span>

```powershell
# Create an Azure AppService that we can host any number of web apps within
New-AzureRmAppServicePlan -Name MyAppServicePlan -Tier Basic -NumberofWorkers 2 -WorkerSize Small -ResourceGroupName myResourceGroup -Location westeurope

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
New-AzureRmWebApp -Name MyWebApp43432 -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westeurope
New-AzureRmWebApp -Name MyWebApp43433 -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westeurope
```

## <a name="listing-deployed-resources"></a><span data-ttu-id="4c849-178">Listar recursos implementados</span><span class="sxs-lookup"><span data-stu-id="4c849-178">Listing deployed resources</span></span>

<span data-ttu-id="4c849-179">Pode utilizar o cmdlet `Get-AzureRmResource` para listar os recursos em execução no Azure.</span><span class="sxs-lookup"><span data-stu-id="4c849-179">You can use the `Get-AzureRmResource` cmdlet to list the resources running in Azure.</span></span> <span data-ttu-id="4c849-180">O exemplo seguinte mostra os recursos acabados de criar no novo grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="4c849-180">The following example shows the resources we just created in the new resource group.</span></span>

```powershell
Get-AzureRmResource |
  Where-Object ResourceGroupName -eq myResourceGroup |
    Select-Object Name,Location,ResourceType
```

```Output
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

## <a name="deleting-resources"></a><span data-ttu-id="4c849-181">Eliminar recursos</span><span class="sxs-lookup"><span data-stu-id="4c849-181">Deleting resources</span></span>

<span data-ttu-id="4c849-182">Para limpar a sua conta do Azure, tem de remover os recursos criados neste exemplo.</span><span class="sxs-lookup"><span data-stu-id="4c849-182">To clean up your Azure account, you want to remove the resources we created in this example.</span></span> <span data-ttu-id="4c849-183">Pode utilizar os cmdlets `Remove-AzureRm*` para eliminar recursos de que já não precisa.</span><span class="sxs-lookup"><span data-stu-id="4c849-183">You can use the `Remove-AzureRm*` cmdlets to delete the resources you no longer need.</span></span> <span data-ttu-id="4c849-184">Para remover a VM do Windows criada, utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="4c849-184">To remove the Windows VM we created, using the following command:</span></span>

```powershell
Remove-AzureRmVM -Name myWindowsVM -ResourceGroupName myResourceGroup
```

<span data-ttu-id="4c849-185">Ser-lhe-á pedido para confirmar se quer remover o recurso.</span><span class="sxs-lookup"><span data-stu-id="4c849-185">You will be prompted to confirm that you want to remove the resource.</span></span>

```Output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

<span data-ttu-id="4c849-186">Também pode utilizar o comando para eliminar muitos recursos ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="4c849-186">You can also use the delete many resources at one time.</span></span> <span data-ttu-id="4c849-187">Por exemplo, o comando seguinte elimina todos os recursos "MyResourceGroup" do grupo de recursos que utilizámos em todos os exemplos deste tutorial de Introdução.</span><span class="sxs-lookup"><span data-stu-id="4c849-187">For example, the following command deletes all the resource group "MyResourceGroup" that we've used for all the samples in this Get Started tutorial.</span></span> <span data-ttu-id="4c849-188">Esta ação remove o grupo de recursos e todos os recursos no mesmo.</span><span class="sxs-lookup"><span data-stu-id="4c849-188">This removes the resource group and all of the resources in it.</span></span>

```powershell
Remove-AzureRmResourceGroup -Name myResourceGroup
```

```Output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

<span data-ttu-id="4c849-189">Esta ação pode demorar vários minutos a concluir.</span><span class="sxs-lookup"><span data-stu-id="4c849-189">This can take several minutes to complete.</span></span>

## <a name="get-samples"></a><span data-ttu-id="4c849-190">Obter exemplos</span><span class="sxs-lookup"><span data-stu-id="4c849-190">Get samples</span></span>

<span data-ttu-id="4c849-191">Para saber mais sobre as formas como pode utilizar o Azure PowerShell, veja os nossos scripts mais comuns para [VMs do Linux](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Vms do Windows](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Aplicações Web](/azure/app-service-web/app-service-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json) e [Bases de Dados SQL](/azure/sql-database/sql-database-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json).</span><span class="sxs-lookup"><span data-stu-id="4c849-191">To learn more about ways to use the Azure PowerShell, check out our most common scripts for [Linux VMs](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Windows VMs](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Web Apps](/azure/app-service-web/app-service-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), and [SQL Databases](/azure/sql-database/sql-database-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json).</span></span>

## <a name="next-steps"></a><span data-ttu-id="4c849-192">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="4c849-192">Next steps</span></span>

* [<span data-ttu-id="4c849-193">Iniciar sessão com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="4c849-193">Login with Azure PowerShell</span></span>](authenticate-azureps.md)
* [<span data-ttu-id="4c849-194">Gerir subscrições do Azure com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="4c849-194">Manage Azure subscriptions with Azure PowerShell</span></span>](manage-subscriptions-azureps.md)
* [<span data-ttu-id="4c849-195">Criar principais de serviço no Azure com o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="4c849-195">Create service principals in Azure using Azure PowerShell</span></span>](create-azure-service-principal-azureps.md)
* <span data-ttu-id="4c849-196">Leia as Notas de versão sobre a migração de uma versão mais antiga: [https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes](https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes).</span><span class="sxs-lookup"><span data-stu-id="4c849-196">Read the Release notes about migrating from an older release: [https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes](https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes).</span></span>
* <span data-ttu-id="4c849-197">Obter ajuda da comunidade:</span><span class="sxs-lookup"><span data-stu-id="4c849-197">Get help from the community:</span></span>
  * [<span data-ttu-id="4c849-198">Fórum do Azure no MSDN</span><span class="sxs-lookup"><span data-stu-id="4c849-198">Azure forum on MSDN</span></span>](http://go.microsoft.com/fwlink/p/?LinkId=320212)
  * [<span data-ttu-id="4c849-199">Stackoverflow</span><span class="sxs-lookup"><span data-stu-id="4c849-199">stackoverflow</span></span>](http://go.microsoft.com/fwlink/?LinkId=320213)
