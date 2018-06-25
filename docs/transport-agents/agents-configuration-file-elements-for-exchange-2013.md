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
description: Encontre informações sobre os elementos XML no arquivo de configuração Agents e fetagents.config no Exchange 2013.
ms.openlocfilehash: dd58c4bc21a968db2ca5b13e0c53f7058b29f233
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751004"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a><span data-ttu-id="8c2c0-103">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8c2c0-103">Agents configuration file elements for Exchange 2013</span></span>

<span data-ttu-id="8c2c0-104">Encontre informações sobre os elementos XML no arquivo de configuração Agents e fetagents.config no Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-104">Find information about the XML elements in the agents.config and fetagents.config configuration file in Exchange 2013.</span></span>
  
<span data-ttu-id="8c2c0-105">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="8c2c0-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="8c2c0-106">Quando você instala o acesso para cliente ou a função de servidor de caixa de correio em um servidor Exchange, o instalador cria um arquivo XML que contém informações de configuração sobre os operadores que estão instalados no servidor.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-106">When you install the Client Access or the Mailbox server role on an Exchange server, the installer creates an XML file that contains configuration information about agents that are installed on the server.</span></span> <span data-ttu-id="8c2c0-107">Você não pode gravar diretamente esse arquivo.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-107">You cannot write directly to this file.</span></span> 
  
<span data-ttu-id="8c2c0-108">O serviço Front End Transport é executado em servidores de acesso para cliente e grava um arquivo chamado fetagents.config. O serviço de transporte e o serviço de transporte de caixa de correio executados nos servidores de caixa de correio e gravar em um arquivo denominado Agents. Um computador que possui a função de servidor acesso para cliente e a função de servidor de caixa de correio terá um fetagents.config e um arquivo Agents.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-108">The Front End Transport service runs on Client Access servers and writes to a file named fetagents.config. The Transport service and the Mailbox Transport service run on Mailbox servers, and write to a file named agents.config. A computer that has both the Client Access server role and the Mailbox server role will have both a fetagents.config and an agents.config file.</span></span> 
  
<span data-ttu-id="8c2c0-109">A única maneira com suporte para gravar esses arquivos é usando os cmdlets do agente de transporte no Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-109">The only supported way to write to these files is by using the transport agent cmdlets in the Exchange Management Shell.</span></span> <span data-ttu-id="8c2c0-110">Para obter informações sobre os cmdlets do agente de transporte, consulte [Cmdlets de fluxo de email](http://technet.microsoft.com/en-us/library/aa998553%28v=exchg.150%29.aspx) no TechNet.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-110">For information about the transport agent cmdlets, see [Mail Flow Cmdlets](http://technet.microsoft.com/en-us/library/aa998553%28v=exchg.150%29.aspx) on TechNet.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="8c2c0-111">Para distinguir entre os agentes que estendem o serviço Front End Transport no servidor de acesso para cliente e o serviço de transporte no servidor de caixa de correio, os cmdlets de agente de transporte tem um parâmetro _TransportService_ com um valor de "Hub" para o transporte serviço e "FrontEnd" para o serviço Front End Transport.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-111">To distinguish between agents that extend the Front End Transport service on the Client Access server and the Transport service on the Mailbox server, transport agent cmdlets have a  _TransportService_ parameter with a value of "Hub" for the Transport service and "FrontEnd" for the Front End Transport service.</span></span> 
  
<span data-ttu-id="8c2c0-112">Você pode ler a Agents ou arquivo fetagents.config para determinar a presença de e informações de configuração de um ou mais operadores no servidor.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-112">You can read the agents.config or fetagents.config file to determine the presence of and configuration information for one or more agents on the server.</span></span> <span data-ttu-id="8c2c0-113">Esta documentação fornece uma referência que você pode usar para ler as informações do arquivo Agents exe ou o fetagents.config. O formato para ambos os arquivos é o mesmo.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-113">This documentation provides a reference that you can use to read the information in either the agents.config file or the fetagents.config. The format for both of these files is the same.</span></span> <span data-ttu-id="8c2c0-114">Esta documentação não fornece informações sobre como escrever para os arquivos.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-114">This documentation does not provide information about how to write to the files.</span></span>
  
> [!CAUTION]
> <span data-ttu-id="8c2c0-115">Usando métodos não suportados para gravar no arquivo Agents ou fetagents.config pode gerar resultados inesperados, inclusive falha de serviço de transporte ou agentes de transporte ou ambos.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-115">Using unsupported methods to write to the agents.config file or fetagents.config can produce unexpected results, including failure of the transport service or transport agents, or both.</span></span> <span data-ttu-id="8c2c0-116">Não escreva diretamente a qualquer um desses arquivos.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-116">Do not write directly to either of these files.</span></span> <span data-ttu-id="8c2c0-117">O único método suportado para gravar nesses arquivos é usando os cmdlets de agente de transporte do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-117">The only supported method for writing to these files is by using the Exchange Management Shell transport agent cmdlets.</span></span> 
  
## <a name="location-of-the-transport-agent-configuration-files"></a><span data-ttu-id="8c2c0-118">Local dos arquivos de configuração do agente de transporte</span><span class="sxs-lookup"><span data-stu-id="8c2c0-118">Location of the transport agent configuration files</span></span>
<span data-ttu-id="8c2c0-119"><a name="bk_ConfigLoc"> </a></span><span class="sxs-lookup"><span data-stu-id="8c2c0-119"></span></span>

<span data-ttu-id="8c2c0-120">Quando você instala o Exchange 2013, o instalador cria um arquivo XML que é chamado agents.config.template ou fetagents.config.template, dependendo da função de servidor instalada, o \<ExchangeInstallFolder\>\TransportRoles\Agents pasta (onde \<ExchangeInstallFolder\> é a pasta na qual você instalou o Exchange 2013).</span><span class="sxs-lookup"><span data-stu-id="8c2c0-120">When you install Exchange 2013, the installer creates an XML file that is named either agents.config.template or fetagents.config.template, depending on the server role installed, in the \<ExchangeInstallFolder\>\TransportRoles\Agents folder (where \<ExchangeInstallFolder\> is the folder in which you installed Exchange 2013).</span></span> <span data-ttu-id="8c2c0-121">Se você instalar a função de servidor acesso para cliente, o Exchange 2013 copia o arquivo fetagents.config.template para fetagents.config. Se você instalar a função de servidor de caixa de correio, o Exchange 2013 copia o arquivo agents.config.template para Agents. Exchange 2013 leituras e gravações esse arquivo, quando você altera a configuração de agentes de transporte no servidor.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-121">If you install the Client Access server role, Exchange 2013 copies the fetagents.config.template file to fetagents.config. If you install the Mailbox server role, Exchange 2013 copies the agents.config.template file to agents.config. Exchange 2013 reads and writes this file when you change the transport agents configuration on the server.</span></span>
  
## <a name="verifying-a-transport-agent-installation"></a><span data-ttu-id="8c2c0-122">Verificando uma instalação do agente de transporte</span><span class="sxs-lookup"><span data-stu-id="8c2c0-122">Verifying a transport agent installation</span></span>
<span data-ttu-id="8c2c0-123"><a name="bk_verifyinstall"> </a></span><span class="sxs-lookup"><span data-stu-id="8c2c0-123"></span></span>

<span data-ttu-id="8c2c0-124">Você pode usar os recursos XML que o .NET Framework fornece para ler e validar o Agents ou o arquivo XML de fetagents.config.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-124">You can use the XML capabilities that the .NET Framework provides to read and validate the agents.config or the fetagents.config XML file.</span></span> <span data-ttu-id="8c2c0-125">Para verificar a instalação e configuração de um agente de transporte, leia o XML no arquivo de configuração e localize o elemento de [agente](agent.md) que corresponde ao agente de transporte.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-125">To verify the installation and configuration of a transport agent, read the XML in the configuration file and find the [agent](agent.md) element that corresponds to the transport agent.</span></span> <span data-ttu-id="8c2c0-126">Se não existir um elemento de **agente** para o agente de transporte específica, o agente de transporte não está instalado.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-126">If an **agent** element for the specific transport agent does not exist, the transport agent is not installed.</span></span> <span data-ttu-id="8c2c0-127">Se o agente de transporte estiver instalado, você pode ler os atributos do elemento **agente** para determinar sua configuração.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-127">If the transport agent is installed, you can read the attributes of the **agent** element to determine its configuration.</span></span> 
  
## <a name="configuration-file-element-hierarchy"></a><span data-ttu-id="8c2c0-128">Hierarquia de elemento do arquivo de configuração</span><span class="sxs-lookup"><span data-stu-id="8c2c0-128">Configuration file element hierarchy</span></span>
<span data-ttu-id="8c2c0-129"><a name="bk_elementref"> </a></span><span class="sxs-lookup"><span data-stu-id="8c2c0-129"></span></span>

<span data-ttu-id="8c2c0-130">O código a seguir mostra a hierarquia de elemento no arquivo XML de configuração.</span><span class="sxs-lookup"><span data-stu-id="8c2c0-130">The following code shows the element hierarchy in the configuration XML file.</span></span>
  
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

## <a name="in-this-section"></a><span data-ttu-id="8c2c0-131">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="8c2c0-131">In this section</span></span>
<span data-ttu-id="8c2c0-132"><a name="bk_elementreflist"> </a></span><span class="sxs-lookup"><span data-stu-id="8c2c0-132"></span></span>

- [<span data-ttu-id="8c2c0-133">agente</span><span class="sxs-lookup"><span data-stu-id="8c2c0-133">agent</span></span>](agent.md)
    
- [<span data-ttu-id="8c2c0-134">agentExecution</span><span class="sxs-lookup"><span data-stu-id="8c2c0-134">agentExecution</span></span>](agentexecution.md)
    
- [<span data-ttu-id="8c2c0-135">agentList</span><span class="sxs-lookup"><span data-stu-id="8c2c0-135">agentList</span></span>](agentlist.md)
    
- [<span data-ttu-id="8c2c0-136">configuração</span><span class="sxs-lookup"><span data-stu-id="8c2c0-136">configuration</span></span>](configuration.md)
    
- [<span data-ttu-id="8c2c0-137">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="8c2c0-137">messageSnapshot</span></span>](messagesnapshot.md)
    
- [<span data-ttu-id="8c2c0-138">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="8c2c0-138">mexRuntime</span></span>](mexruntime.md)
    
- [<span data-ttu-id="8c2c0-139">monitoramento</span><span class="sxs-lookup"><span data-stu-id="8c2c0-139">monitoring</span></span>](monitoring.md)
    
## <a name="see-also"></a><span data-ttu-id="8c2c0-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="8c2c0-140">See also</span></span>

- [<span data-ttu-id="8c2c0-141">Agentes de transporte no Exchange</span><span class="sxs-lookup"><span data-stu-id="8c2c0-141">Transport agents in Exchange</span></span>](transport-agents-in-exchange-2013.md)
- [<span data-ttu-id="8c2c0-142">Transporte conceitos de agente no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8c2c0-142">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
- [<span data-ttu-id="8c2c0-143">Referência de agente de transporte do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8c2c0-143">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
- [<span data-ttu-id="8c2c0-144">Transporte namespaces de agente no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8c2c0-144">Transport agent namespaces in Exchange 2013</span></span>](transport-agent-namespaces-in-exchange-2013.md)
- [<span data-ttu-id="8c2c0-145">Cmdlets de fluxo de email</span><span class="sxs-lookup"><span data-stu-id="8c2c0-145">Mail Flow Cmdlets</span></span>](https://docs.microsoft.com/en-us/powershell/exchange/?view=exchange-ps)
    

