---
title: Elementos de arquivo de configuração de agentes para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Agents
api_type:
- schema
ms.assetid: 3047653b-d712-46c1-ae0a-73f3975f5e9d
description: Encontre informações sobre os elementos XML no arquivo de configuração Agents. config e fetagents. config no Exchange 2013.
ms.openlocfilehash: f19fe8316a78cef668db881e630562d3be8be64a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461566"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a><span data-ttu-id="0df08-103">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0df08-103">Agents configuration file elements for Exchange 2013</span></span>

<span data-ttu-id="0df08-104">Encontre informações sobre os elementos XML no arquivo de configuração Agents. config e fetagents. config no Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="0df08-104">Find information about the XML elements in the agents.config and fetagents.config configuration file in Exchange 2013.</span></span>
  
<span data-ttu-id="0df08-105">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="0df08-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="0df08-106">Quando você instala a função de servidor Acesso para cliente ou caixa de correio em um servidor Exchange, o instalador cria um arquivo XML que contém informações de configuração sobre os agentes instalados no servidor.</span><span class="sxs-lookup"><span data-stu-id="0df08-106">When you install the Client Access or the Mailbox server role on an Exchange server, the installer creates an XML file that contains configuration information about agents that are installed on the server.</span></span> <span data-ttu-id="0df08-107">Você não pode gravar diretamente neste arquivo.</span><span class="sxs-lookup"><span data-stu-id="0df08-107">You cannot write directly to this file.</span></span> 
  
<span data-ttu-id="0df08-108">O serviço de transporte de front-end é executado em servidores de acesso para cliente e grava em um arquivo chamado fetagents. config. O serviço de transporte e o serviço de transporte de caixa de correio são executados em servidores de caixa de correio e grava em um arquivo chamado Agents. config. Um computador que tenha a função de servidor de acesso para cliente e a função de servidor de caixa de correio terá um fetagents. config e um arquivo agents. config.</span><span class="sxs-lookup"><span data-stu-id="0df08-108">The Front End Transport service runs on Client Access servers and writes to a file named fetagents.config. The Transport service and the Mailbox Transport service run on Mailbox servers, and write to a file named agents.config. A computer that has both the Client Access server role and the Mailbox server role will have both a fetagents.config and an agents.config file.</span></span> 
  
<span data-ttu-id="0df08-109">A única maneira compatível de gravar nesses arquivos é usando os cmdlets do agente de transporte no Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0df08-109">The only supported way to write to these files is by using the transport agent cmdlets in the Exchange Management Shell.</span></span> <span data-ttu-id="0df08-110">Para obter informações sobre os cmdlets do agente de transporte, consulte [cmdlets de fluxo de emails](https://technet.microsoft.com/library/aa998553%28v=exchg.150%29.aspx) no TechNet.</span><span class="sxs-lookup"><span data-stu-id="0df08-110">For information about the transport agent cmdlets, see [Mail Flow Cmdlets](https://technet.microsoft.com/library/aa998553%28v=exchg.150%29.aspx) on TechNet.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0df08-111">Para distinguir entre agentes que estendem o serviço de transporte de front-end no servidor de acesso para cliente e o serviço de transporte no servidor de caixa de correio, os cmdlets do agente de transporte têm um parâmetro _TransportService_ com um valor de "Hub" para o serviço de transporte e "frontend" para o serviço de transporte de front-end.</span><span class="sxs-lookup"><span data-stu-id="0df08-111">To distinguish between agents that extend the Front End Transport service on the Client Access server and the Transport service on the Mailbox server, transport agent cmdlets have a  _TransportService_ parameter with a value of "Hub" for the Transport service and "FrontEnd" for the Front End Transport service.</span></span> 
  
<span data-ttu-id="0df08-112">Você pode ler o arquivo agents. config ou fetagents. config para determinar a presença e as informações de configuração de um ou mais agentes no servidor.</span><span class="sxs-lookup"><span data-stu-id="0df08-112">You can read the agents.config or fetagents.config file to determine the presence of and configuration information for one or more agents on the server.</span></span> <span data-ttu-id="0df08-113">Esta documentação fornece uma referência que você pode usar para ler as informações no arquivo agents. config ou no fetagents. config. O formato de ambos os arquivos é o mesmo.</span><span class="sxs-lookup"><span data-stu-id="0df08-113">This documentation provides a reference that you can use to read the information in either the agents.config file or the fetagents.config. The format for both of these files is the same.</span></span> <span data-ttu-id="0df08-114">Esta documentação não fornece informações sobre como gravar nos arquivos.</span><span class="sxs-lookup"><span data-stu-id="0df08-114">This documentation does not provide information about how to write to the files.</span></span>
  
> [!CAUTION]
> <span data-ttu-id="0df08-115">O uso de métodos sem suporte para gravar no arquivo agents. config ou fetagents. config pode produzir resultados inesperados, incluindo a falha do serviço de transporte ou agentes de transporte, ou ambos.</span><span class="sxs-lookup"><span data-stu-id="0df08-115">Using unsupported methods to write to the agents.config file or fetagents.config can produce unexpected results, including failure of the transport service or transport agents, or both.</span></span> <span data-ttu-id="0df08-116">Não escreva diretamente para nenhum desses arquivos.</span><span class="sxs-lookup"><span data-stu-id="0df08-116">Do not write directly to either of these files.</span></span> <span data-ttu-id="0df08-117">O único método com suporte para gravar nesses arquivos é usando os cmdlets do agente de transporte do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0df08-117">The only supported method for writing to these files is by using the Exchange Management Shell transport agent cmdlets.</span></span> 
  
## <a name="location-of-the-transport-agent-configuration-files"></a><span data-ttu-id="0df08-118">Local dos arquivos de configuração do agente de transporte</span><span class="sxs-lookup"><span data-stu-id="0df08-118">Location of the transport agent configuration files</span></span>
<span data-ttu-id="0df08-119"><a name="bk_ConfigLoc"> </a></span><span class="sxs-lookup"><span data-stu-id="0df08-119"><a name="bk_ConfigLoc"> </a></span></span>

<span data-ttu-id="0df08-120">Quando você instala o Exchange 2013, o instalador cria um arquivo XML chamado Agents. config. Template ou fetagents. config. Template, dependendo da função de servidor instalada, na \<ExchangeInstallFolder\> pasta \TransportRoles\Agents (onde \<ExchangeInstallFolder\> é a pasta na qual você instalou o Exchange 2013).</span><span class="sxs-lookup"><span data-stu-id="0df08-120">When you install Exchange 2013, the installer creates an XML file that is named either agents.config.template or fetagents.config.template, depending on the server role installed, in the \<ExchangeInstallFolder\>\TransportRoles\Agents folder (where \<ExchangeInstallFolder\> is the folder in which you installed Exchange 2013).</span></span> <span data-ttu-id="0df08-121">Se você instalar a função de servidor Acesso para cliente, o Exchange 2013 copiará o arquivo fetagents. config. Template para fetagents. config. Se você instalar a função de servidor caixa de correio, o Exchange 2013 copiará o arquivo agents. config. Template para o Agents. config. O Exchange 2013 lê e grava esse arquivo quando você altera a configuração dos agentes de transporte no servidor.</span><span class="sxs-lookup"><span data-stu-id="0df08-121">If you install the Client Access server role, Exchange 2013 copies the fetagents.config.template file to fetagents.config. If you install the Mailbox server role, Exchange 2013 copies the agents.config.template file to agents.config. Exchange 2013 reads and writes this file when you change the transport agents configuration on the server.</span></span>
  
## <a name="verifying-a-transport-agent-installation"></a><span data-ttu-id="0df08-122">Verificar a instalação de um agente de transporte</span><span class="sxs-lookup"><span data-stu-id="0df08-122">Verifying a transport agent installation</span></span>
<span data-ttu-id="0df08-123"><a name="bk_verifyinstall"> </a></span><span class="sxs-lookup"><span data-stu-id="0df08-123"><a name="bk_verifyinstall"> </a></span></span>

<span data-ttu-id="0df08-124">Você pode usar os recursos de XML que o .NET Framework fornece para ler e validar os agentes. config ou o arquivo XML fetagents. config.</span><span class="sxs-lookup"><span data-stu-id="0df08-124">You can use the XML capabilities that the .NET Framework provides to read and validate the agents.config or the fetagents.config XML file.</span></span> <span data-ttu-id="0df08-125">Para verificar a instalação e a configuração de um agente de transporte, leia o XML no arquivo de configuração e localize o elemento do [agente](agent.md) que corresponde ao agente de transporte.</span><span class="sxs-lookup"><span data-stu-id="0df08-125">To verify the installation and configuration of a transport agent, read the XML in the configuration file and find the [agent](agent.md) element that corresponds to the transport agent.</span></span> <span data-ttu-id="0df08-126">Se não existir um elemento de **agente** para o agente de transporte específico, o agente de transporte não será instalado.</span><span class="sxs-lookup"><span data-stu-id="0df08-126">If an **agent** element for the specific transport agent does not exist, the transport agent is not installed.</span></span> <span data-ttu-id="0df08-127">Se o agente de transporte estiver instalado, você poderá ler os atributos do elemento **Agent** para determinar sua configuração.</span><span class="sxs-lookup"><span data-stu-id="0df08-127">If the transport agent is installed, you can read the attributes of the **agent** element to determine its configuration.</span></span> 
  
## <a name="configuration-file-element-hierarchy"></a><span data-ttu-id="0df08-128">Hierarquia de elemento do arquivo de configuração</span><span class="sxs-lookup"><span data-stu-id="0df08-128">Configuration file element hierarchy</span></span>
<span data-ttu-id="0df08-129"><a name="bk_elementref"> </a></span><span class="sxs-lookup"><span data-stu-id="0df08-129"><a name="bk_elementref"> </a></span></span>

<span data-ttu-id="0df08-130">O código a seguir mostra a hierarquia do elemento no arquivo XML de configuração.</span><span class="sxs-lookup"><span data-stu-id="0df08-130">The following code shows the element hierarchy in the configuration XML file.</span></span>
  
```XML
<configuration>
    <mexRuntime>
        <monitoring>
            <agentExecution/>
            <messageSnapshot/>
        </monitoring>
        <agentList>
            <agent/>
            <agent/>
            <agent />
        </agentList>
    </mexRuntim>
</configuration>
```

## <a name="in-this-section"></a><span data-ttu-id="0df08-131">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="0df08-131">In this section</span></span>
<span data-ttu-id="0df08-132"><a name="bk_elementreflist"> </a></span><span class="sxs-lookup"><span data-stu-id="0df08-132"><a name="bk_elementreflist"> </a></span></span>

- [<span data-ttu-id="0df08-133">Agente</span><span class="sxs-lookup"><span data-stu-id="0df08-133">agent</span></span>](agent.md)
    
- [<span data-ttu-id="0df08-134">agentExecution</span><span class="sxs-lookup"><span data-stu-id="0df08-134">agentExecution</span></span>](agentexecution.md)
    
- [<span data-ttu-id="0df08-135">agentlist</span><span class="sxs-lookup"><span data-stu-id="0df08-135">agentList</span></span>](agentlist.md)
    
- [<span data-ttu-id="0df08-136">configuration</span><span class="sxs-lookup"><span data-stu-id="0df08-136">configuration</span></span>](configuration.md)
    
- [<span data-ttu-id="0df08-137">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="0df08-137">messageSnapshot</span></span>](messagesnapshot.md)
    
- [<span data-ttu-id="0df08-138">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="0df08-138">mexRuntime</span></span>](mexruntime.md)
    
- [<span data-ttu-id="0df08-139">monitoramento</span><span class="sxs-lookup"><span data-stu-id="0df08-139">monitoring</span></span>](monitoring.md)
    
## <a name="see-also"></a><span data-ttu-id="0df08-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="0df08-140">See also</span></span>

- [<span data-ttu-id="0df08-141">Agentes de transporte no Exchange</span><span class="sxs-lookup"><span data-stu-id="0df08-141">Transport agents in Exchange</span></span>](transport-agents-in-exchange-2013.md)
- [<span data-ttu-id="0df08-142">Conceitos de agente de transporte no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0df08-142">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
- [<span data-ttu-id="0df08-143">Referência do agente de transporte para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0df08-143">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
- [<span data-ttu-id="0df08-144">Namespaces do agente de transporte no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0df08-144">Transport agent namespaces in Exchange 2013</span></span>](transport-agent-namespaces-in-exchange-2013.md)
- [<span data-ttu-id="0df08-145">Cmdlets de fluxo de emails</span><span class="sxs-lookup"><span data-stu-id="0df08-145">Mail Flow Cmdlets</span></span>](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)
    

