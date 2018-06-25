---
title: Criando os agentes de transporte do Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d291ab78-7cdd-4dbe-a5f4-9dc8e9650a33
description: Encontre informações sobre como criar os agentes de transporte personalizado para o Exchange 2013 e os requisitos de sistema para a criação de um agente personalizado.
ms.openlocfilehash: 6146e37c44441bed1d30d08f71ede255dba26440
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751003"
---
# <a name="creating-transport-agents-for-exchange-2013"></a><span data-ttu-id="0c842-103">Criando os agentes de transporte do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0c842-103">Creating transport agents for Exchange 2013</span></span>

<span data-ttu-id="0c842-104">Encontre informações sobre como criar os agentes de transporte personalizado para o Exchange 2013 e os requisitos de sistema para a criação de um agente personalizado.</span><span class="sxs-lookup"><span data-stu-id="0c842-104">Find information about how to create custom transport agents for Exchange 2013, and the system requirements for creating a custom agent.</span></span>
  
<span data-ttu-id="0c842-105">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="0c842-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="0c842-106">Exchange Server 2013 inclui vários agentes de transporte que podem ser usados para processar mensagens.</span><span class="sxs-lookup"><span data-stu-id="0c842-106">Exchange Server 2013 includes several transport agents that you can use to process messages.</span></span> <span data-ttu-id="0c842-107">Usando os assemblies que vêm com o Exchange, você pode criar seus próprios agentes personalizados para executar tarefas específicas de acordo com as necessidades da sua organização.</span><span class="sxs-lookup"><span data-stu-id="0c842-107">By using the assemblies that come with Exchange, you can create your own custom agents to perform specific tasks according to the needs of your organization.</span></span> <span data-ttu-id="0c842-108">Por exemplo, você pode usar um agente de transporte SmtpReceiveAgent a intercepção mensagens que são recebidos por meio do protocolo SMTP e o processo a mensagem para converter o formato do corpo para conter texto pré-formatado.</span><span class="sxs-lookup"><span data-stu-id="0c842-108">For example, you can use an SmtpReceiveAgent transport agent to intercept messages that are received via the SMTP protocol and process the message to convert the format of the body to contain preformatted text.</span></span> <span data-ttu-id="0c842-109">Você pode usar um agente de transporte RoutingAgent para efetuar as mensagens que passam pelo servidor em rota para outro servidor.</span><span class="sxs-lookup"><span data-stu-id="0c842-109">You can use a RoutingAgent transport agent to log the messages that pass through the server on route to another server.</span></span> <span data-ttu-id="0c842-110">Você também pode criar mais complexos recursos que tornam o usam das mais de um tipo de agente.</span><span class="sxs-lookup"><span data-stu-id="0c842-110">You can also create more complex features that make use of more than one type of agent.</span></span> <span data-ttu-id="0c842-111">Por exemplo, para criar um agente de antivírus, você pode implementar um SmtpReceiveAgent e um agente de RoutingAgent.</span><span class="sxs-lookup"><span data-stu-id="0c842-111">For example, to create an antivirus agent, you can implement an SmtpReceiveAgent and a RoutingAgent agent.</span></span> <span data-ttu-id="0c842-112">Se você tiver um componente da rede que não suporta o protocolo SMTP, você pode usar um agente de transporte DeliveryAgent para lidar com a comunicação entre o seu servidor do Exchange e seu componente externo.</span><span class="sxs-lookup"><span data-stu-id="0c842-112">If you have a component on your network that does not support the SMTP protocol, you can use a DeliveryAgent transport agent to handle the communication between your Exchange server and your external component.</span></span> 
  
<span data-ttu-id="0c842-113">Este artigo fornece informações sobre os pré-requisitos para e as tarefas envolvidas na criação de seu próprio agente de transporte.</span><span class="sxs-lookup"><span data-stu-id="0c842-113">This article provides information about the prerequisites for and tasks involved in creating your own transport agent.</span></span> <span data-ttu-id="0c842-114">Para obter informações sobre a criação de agentes de transporte específica, consulte [criar um agente de transporte do Exchange 2013 RoutingAgent](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [criar um agente de transporte SmtpReceiveAgent para o Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)e [criar um agente de transporte DeliveryAgent para Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="0c842-114">For information about creating specific transport agents, see [Create a RoutingAgent transport agent for Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [Create an SmtpReceiveAgent transport agent for Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md), and [Create a DeliveryAgent transport agent for Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).</span></span>
  
## <a name="prerequisites-for-creating-a-transport-agent"></a><span data-ttu-id="0c842-115">Pré-requisitos para a criação de um agente de transporte</span><span class="sxs-lookup"><span data-stu-id="0c842-115">Prerequisites for creating a transport agent</span></span>
<span data-ttu-id="0c842-116"><a name="bk_prerequisites"> </a></span><span class="sxs-lookup"><span data-stu-id="0c842-116"></span></span>

<span data-ttu-id="0c842-117">Estes são os pré-requisitos necessários para implementar um agente de transporte:</span><span class="sxs-lookup"><span data-stu-id="0c842-117">The following are the prerequisites that you need in order to implement a transport agent:</span></span>
  
- <span data-ttu-id="0c842-118">Um computador executando o Exchange 2013 que está executando o serviço Front End Transport em um servidor de acesso para cliente ou de transporte de borda, ou o serviço de transporte em um servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0c842-118">A computer running Exchange 2013 that is running the Front End Transport service on a Client Access or Edge Transport server, or the Transport service on a Mailbox server.</span></span> <span data-ttu-id="0c842-119">Para obter informações sobre a arquitetura da função de servidor no Exchange 2013, consulte [Transporte conceitos de agente no Exchange 2013](transport-agent-concepts-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="0c842-119">For information about the server role architecture in Exchange 2013, see [Transport agent concepts in Exchange 2013](transport-agent-concepts-in-exchange-2013.md).</span></span>
    
- <span data-ttu-id="0c842-120">Os assemblies a seguir para as classes de agente de transporte:</span><span class="sxs-lookup"><span data-stu-id="0c842-120">The following assemblies for the transport agent classes:</span></span>
    
  - <span data-ttu-id="0c842-121">Microsoft.Exchange.Data.dll</span><span class="sxs-lookup"><span data-stu-id="0c842-121">Microsoft.Exchange.Data.dll</span></span>
    
  - <span data-ttu-id="0c842-122">Microsoft.Exchange.Data.Common.dll</span><span class="sxs-lookup"><span data-stu-id="0c842-122">Microsoft.Exchange.Data.Common.dll</span></span>
    
  - <span data-ttu-id="0c842-123">Microsoft.Exchange.Transport.dll</span><span class="sxs-lookup"><span data-stu-id="0c842-123">Microsoft.Exchange.Transport.dll</span></span>
    
- <span data-ttu-id="0c842-124">O .NET Framework 4.5</span><span class="sxs-lookup"><span data-stu-id="0c842-124">The .NET Framework 4.5</span></span>
    
<span data-ttu-id="0c842-125">Também recomendamos que você instale o Visual Studio 2012.</span><span class="sxs-lookup"><span data-stu-id="0c842-125">We also recommend that you install Visual Studio 2012.</span></span> <span data-ttu-id="0c842-126">Você pode implementar agentes de transporte usando o Visual Basic .NET ou c#.</span><span class="sxs-lookup"><span data-stu-id="0c842-126">You can implement transport agents by using either Visual Basic .NET or C#.</span></span>
  
## <a name="referencing-the-assemblies"></a><span data-ttu-id="0c842-127">Referenciando os assemblies</span><span class="sxs-lookup"><span data-stu-id="0c842-127">Referencing the assemblies</span></span>
<span data-ttu-id="0c842-128"><a name="bk_ReferenceAssemblies"> </a></span><span class="sxs-lookup"><span data-stu-id="0c842-128"></span></span>

<span data-ttu-id="0c842-129">Exchange 2013 fornece uma biblioteca de classes que oferecem suporte a extensão de comportamento de transporte do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c842-129">Exchange 2013 provides a library of classes that support the extension of Exchange transport behavior.</span></span> <span data-ttu-id="0c842-130">Essas classes exigem o .NET Framework 4.5.</span><span class="sxs-lookup"><span data-stu-id="0c842-130">These classes require the .NET Framework 4.5.</span></span> <span data-ttu-id="0c842-131">Você pode implementar os agentes de transporte com base nessas classes usando o Visual Studio 2012.</span><span class="sxs-lookup"><span data-stu-id="0c842-131">You can implement transport agents based on these classes by using Visual Studio 2012.</span></span>
  
<span data-ttu-id="0c842-132">O instalador do Exchange 2013 instala os assemblies que são usados para desenvolvimento do agente de transporte e registra-los no cache de assembly global (GAC).</span><span class="sxs-lookup"><span data-stu-id="0c842-132">The Exchange 2013 installer installs assemblies that are used for transport agent development and registers them in the global assembly cache (GAC).</span></span> <span data-ttu-id="0c842-133">Para começar a implementar um agente de transporte, crie uma referência para o assembly Microsoft.Exchange.Data.Transport em um projeto de biblioteca de classe.</span><span class="sxs-lookup"><span data-stu-id="0c842-133">To begin implementing a transport agent, create a reference to the Microsoft.Exchange.Data.Transport assembly in a class library project.</span></span>
  
## <a name="implementing-a-transport-agent"></a><span data-ttu-id="0c842-134">Implementando um agente de transporte</span><span class="sxs-lookup"><span data-stu-id="0c842-134">Implementing a transport agent</span></span>
<span data-ttu-id="0c842-135"><a name="bk_implementationExample"> </a></span><span class="sxs-lookup"><span data-stu-id="0c842-135"></span></span>

<span data-ttu-id="0c842-136">O exemplo a seguir mostra um mínimo de implementação das classes que derivam das classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) e [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0c842-136">The following example shows a minimal implementation of classes that derive from the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes.</span></span> 
  
> [!CAUTION]
> <span data-ttu-id="0c842-137">Se vários agentes de transporte são instalados e registrados para o mesmo evento, todos os operadores serão chamados, mesmo se um agente remove todos os destinatários de um item de email.</span><span class="sxs-lookup"><span data-stu-id="0c842-137">If multiple transport agents are installed and registered for the same event, all agents will be invoked, even if one agent removes all the recipients from a mail item.</span></span> <span data-ttu-id="0c842-138">> Para evitar erros não tratados ou comportamento imprevisível, o agente de transporte deve lidar com casos em que a contagem de destinatários em um item de email é igual a zero.</span><span class="sxs-lookup"><span data-stu-id="0c842-138">> To avoid unhandled errors or unpredictable behavior, your transport agent should handle cases in which the recipient count on a mail item is equal to zero.</span></span> 
  
```cs
using System;
using System.Collections.Generic;
using System.Text;
using Microsoft.Exchange.Data.Transport;
using Microsoft.Exchange.Data.Transport.Smtp;
namespace MyAgents
{
    public sealed class MyAgentFactory : SmtpReceiveAgentFactory
    {
        public override SmtpReceiveAgent CreateAgent(SmtpServer server)
        {
            return new MyAgent();
        }
    }
    public class MyAgent : SmtpReceiveAgent
    {
        public MyAgent()
        {
            this.OnEndOfData += new EndOfDataEventHandler(MyEndOfDataHandler);
        }
        private void MyEndOfDataHandler (ReceiveMessageEventSource source, EndOfDataEventArgs e)
        {
            // The following line appends text to the subject of the message that caused the event.
            e.MailItem.Message.Subject += " - this text appended by MyAgent";
        }
    }
}
```

```vb
Imports System
Imports System.Collections.Generic
Imports System.Text
Imports Microsoft.Exchange.Data.Transport
Imports Microsoft.Exchange.Data.Transport.Smtp
Namespace MyAgents
    NotInheritable Class MyAgentFactory
        Inherits SmtpReceiveAgentFactory
        Public Overrides Function CreateAgent(ByVal server as SmtpServer) As SmtpReceiveAgent
            Return New MyAgent
        End Function
    End Class
    Public Class MyAgent
        Inherits SmtpReceiveAgent
        Private Sub MyEndOfDataHandler(ByVal source As ReceiveMessageEventSource, ByVal e As EndOfDataEventArgs) Handles Me.OnEndOfData
            ' The following line appends text to the subject of the message that caused the event.
            e.MailItem.Message.Subject &amp;= e.MailItem.Message.Subject + " - this text appended by MyAgent"
        End Sub
    End Class
End Namespace
```

## <a name="installing-and-enabling-an-agent"></a><span data-ttu-id="0c842-139">Instalar e ativar um operador</span><span class="sxs-lookup"><span data-stu-id="0c842-139">Installing and enabling an agent</span></span>
<span data-ttu-id="0c842-140"><a name="bk_InstallEnable"> </a></span><span class="sxs-lookup"><span data-stu-id="0c842-140"></span></span>

<span data-ttu-id="0c842-141">Depois que você compila seu agente para uma DLL, você deve instalar e habilitar o agente em seu servidor do Exchange de desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="0c842-141">After you compile your agent to a DLL, you must install and enable the agent on your development Exchange server.</span></span> <span data-ttu-id="0c842-142">No Shell de gerenciamento do Exchange, use o cmdlet [Install-TransportAgent](http://technet.microsoft.com/en-us/library/aa997998.aspx) para instalar o agente e o cmdlet [Enable-TransportAgent](http://technet.microsoft.com/en-us/library/bb124921.aspx) para habilitar o agente.</span><span class="sxs-lookup"><span data-stu-id="0c842-142">In the Exchange Management Shell, use the [Install-TransportAgent](http://technet.microsoft.com/en-us/library/aa997998.aspx) cmdlet to install your agent, and the [Enable-TransportAgent](http://technet.microsoft.com/en-us/library/bb124921.aspx) cmdlet to enable your agent.</span></span> <span data-ttu-id="0c842-143">Para obter informações sobre como usar o Shell de gerenciamento do Exchange, consulte [Exchange Server PowerShell (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="0c842-143">For information about how to use the Exchange Management Shell, see [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).</span></span>
  
> [!CAUTION]
> <span data-ttu-id="0c842-144">Agentes de transporte têm acesso total a todas as mensagens de email que eles encontrem.</span><span class="sxs-lookup"><span data-stu-id="0c842-144">Transport agents have full access to all email messages that they encounter.</span></span> <span data-ttu-id="0c842-145">Exchange 2013 não restringe o comportamento de um agente de transporte.</span><span class="sxs-lookup"><span data-stu-id="0c842-145">Exchange 2013 does not restrict the behavior of a transport agent.</span></span> <span data-ttu-id="0c842-146">Agentes de transporte que estão instáveis ou que contenham falhas de segurança podem afetar a estabilidade e a segurança do Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="0c842-146">Transport agents that are unstable or that contain security flaws might affect the stability and security of Exchange 2013.</span></span> <span data-ttu-id="0c842-147">Portanto, você deve instalar somente os agentes de transporte que você confia totalmente e que foram testados totalmente.</span><span class="sxs-lookup"><span data-stu-id="0c842-147">Therefore, you should only install transport agents that you fully trust and that have been fully tested.</span></span> 
  
<span data-ttu-id="0c842-148">Quando você usa o cmdlet **Install-TransportAgent** para instalar um operador, o Shell de gerenciamento do Exchange mantém um bloqueio no assembly.</span><span class="sxs-lookup"><span data-stu-id="0c842-148">When you use the **Install-TransportAgent** cmdlet to install an agent, the Exchange Management Shell keeps a lock on the assembly.</span></span> <span data-ttu-id="0c842-149">Para liberar o bloqueio do assembly, você deve fechar a instância do Shell de gerenciamento do Exchange que você usou para instalar o agente.</span><span class="sxs-lookup"><span data-stu-id="0c842-149">To release the lock on the assembly, you must close the instance of the Exchange Management Shell that you used to install the agent.</span></span> <span data-ttu-id="0c842-150">Não será possível atualizar o assembly até que você libere o bloqueio.</span><span class="sxs-lookup"><span data-stu-id="0c842-150">You will be unable to update the assembly until you release the lock.</span></span> 
  
<span data-ttu-id="0c842-151">O exemplo a seguir mostra como usar o Shell de gerenciamento do Exchange para instalar e habilitar um agente chamado MyAgent usando uma classe derivada de [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) chamado MyAgents.MyAgentFactory.</span><span class="sxs-lookup"><span data-stu-id="0c842-151">The following example shows how to use the Exchange Management Shell to install and enable an agent named MyAgent by using a class derived from [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) named MyAgents.MyAgentFactory.</span></span> 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
<span data-ttu-id="0c842-152">Este exemplo chama o agente MyCustomAgent no servidor em que o agente está instalado.</span><span class="sxs-lookup"><span data-stu-id="0c842-152">This example names the agent MyCustomAgent on the server on which the agent is installed.</span></span> <span data-ttu-id="0c842-153">O exemplo a seguir mostra como habilitar o agente denominado MyCustomAgent.</span><span class="sxs-lookup"><span data-stu-id="0c842-153">The following example shows how to enable the agent named MyCustomAgent.</span></span>
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
<span data-ttu-id="0c842-154">Para gerenciar um agente de transporte no serviço Front End Transport em um servidor de acesso para cliente, adicione o seguinte valor ao comando: `-TransportService FrontEnd`.</span><span class="sxs-lookup"><span data-stu-id="0c842-154">To manage a transport agent in the Front End Transport service on a Client Access server, add the following value to the command:  `-TransportService FrontEnd`.</span></span> <span data-ttu-id="0c842-155">Por exemplo, para exibir os agentes de transporte no serviço Front End Transport, execute o seguinte comando.</span><span class="sxs-lookup"><span data-stu-id="0c842-155">For example, to view the transport agents in the Front End Transport service, run the following command.</span></span>
  
 `Get-TransportAgent -TransportService FrontEnd`
  
<span data-ttu-id="0c842-156">Para obter mais informações sobre como instalar, habilitando e gerenciando seu agente, consulte [Gerenciar agentes de transporte](http://technet.microsoft.com/en-us/library/bb125175%28v=exchg.150%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="0c842-156">For more information about installing, enabling, and managing your agent, see [Manage Transport Agents](http://technet.microsoft.com/en-us/library/bb125175%28v=exchg.150%29.aspx).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="0c842-157">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="0c842-157">In this section</span></span>
<span data-ttu-id="0c842-158"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="0c842-158"></span></span>

- [<span data-ttu-id="0c842-159">Criar um agente de transporte RoutingAgent para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0c842-159">Create a RoutingAgent transport agent for Exchange 2013</span></span>](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [<span data-ttu-id="0c842-160">Criar um agente de transporte SmtpReceiveAgent para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0c842-160">Create an SmtpReceiveAgent transport agent for Exchange 2013</span></span>](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [<span data-ttu-id="0c842-161">Criar um agente de transporte DeliveryAgent para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0c842-161">Create a DeliveryAgent transport agent for Exchange 2013</span></span>](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="0c842-162">Confira também</span><span class="sxs-lookup"><span data-stu-id="0c842-162">See also</span></span>

- [<span data-ttu-id="0c842-163">Transporte conceitos de agente no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0c842-163">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)   
- [<span data-ttu-id="0c842-164">Referência de agente de transporte do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0c842-164">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
    

