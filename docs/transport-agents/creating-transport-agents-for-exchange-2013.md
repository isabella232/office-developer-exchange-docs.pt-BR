---
title: Criando agentes de transporte para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d291ab78-7cdd-4dbe-a5f4-9dc8e9650a33
description: Encontre informações sobre como criar agentes de transporte personalizados para o Exchange 2013 e os requisitos de sistema para a criação de um agente personalizado.
ms.openlocfilehash: cb1cd180817524fe29a100a48d90444c75a77510
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462371"
---
# <a name="creating-transport-agents-for-exchange-2013"></a><span data-ttu-id="e8834-103">Criando agentes de transporte para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e8834-103">Creating transport agents for Exchange 2013</span></span>

<span data-ttu-id="e8834-104">Encontre informações sobre como criar agentes de transporte personalizados para o Exchange 2013 e os requisitos de sistema para a criação de um agente personalizado.</span><span class="sxs-lookup"><span data-stu-id="e8834-104">Find information about how to create custom transport agents for Exchange 2013, and the system requirements for creating a custom agent.</span></span>
  
<span data-ttu-id="e8834-105">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="e8834-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="e8834-106">O Exchange Server 2013 inclui vários agentes de transporte que você pode usar para processar mensagens.</span><span class="sxs-lookup"><span data-stu-id="e8834-106">Exchange Server 2013 includes several transport agents that you can use to process messages.</span></span> <span data-ttu-id="e8834-107">Usando os assemblies que acompanham o Exchange, você pode criar seus próprios agentes personalizados para executar tarefas específicas de acordo com as necessidades da sua organização.</span><span class="sxs-lookup"><span data-stu-id="e8834-107">By using the assemblies that come with Exchange, you can create your own custom agents to perform specific tasks according to the needs of your organization.</span></span> <span data-ttu-id="e8834-108">Por exemplo, você pode usar um agente de transporte SmtpReceiveAgent para interceptar mensagens recebidas por meio do protocolo SMTP e processar a mensagem para converter o formato do corpo para conter texto pré-formatado.</span><span class="sxs-lookup"><span data-stu-id="e8834-108">For example, you can use an SmtpReceiveAgent transport agent to intercept messages that are received via the SMTP protocol and process the message to convert the format of the body to contain preformatted text.</span></span> <span data-ttu-id="e8834-109">Você pode usar um agente de transporte RoutingAgent para registrar as mensagens que passam pelo servidor na rota para outro servidor.</span><span class="sxs-lookup"><span data-stu-id="e8834-109">You can use a RoutingAgent transport agent to log the messages that pass through the server on route to another server.</span></span> <span data-ttu-id="e8834-110">Você também pode criar recursos mais complexos que fazem uso de mais de um tipo de agente.</span><span class="sxs-lookup"><span data-stu-id="e8834-110">You can also create more complex features that make use of more than one type of agent.</span></span> <span data-ttu-id="e8834-111">Por exemplo, para criar um agente antivírus, é possível implementar um SmtpReceiveAgent e um agente do RoutingAgent.</span><span class="sxs-lookup"><span data-stu-id="e8834-111">For example, to create an antivirus agent, you can implement an SmtpReceiveAgent and a RoutingAgent agent.</span></span> <span data-ttu-id="e8834-112">Se você tiver um componente em sua rede que não ofereça suporte ao protocolo SMTP, poderá usar um agente de transporte do DeliveryAgent para lidar com a comunicação entre o servidor do Exchange e o componente externo.</span><span class="sxs-lookup"><span data-stu-id="e8834-112">If you have a component on your network that does not support the SMTP protocol, you can use a DeliveryAgent transport agent to handle the communication between your Exchange server and your external component.</span></span> 
  
<span data-ttu-id="e8834-113">Este artigo fornece informações sobre os pré-requisitos e as tarefas envolvidas na criação de seu próprio agente de transporte.</span><span class="sxs-lookup"><span data-stu-id="e8834-113">This article provides information about the prerequisites for and tasks involved in creating your own transport agent.</span></span> <span data-ttu-id="e8834-114">Para obter informações sobre como criar agentes de transporte específicos, consulte [criar um agente de transporte RoutingAgent para o exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [criar um agente de transporte SmtpReceiveAgent para o Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)e [criar um agente de transporte DeliveryAgent para o Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="e8834-114">For information about creating specific transport agents, see [Create a RoutingAgent transport agent for Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [Create an SmtpReceiveAgent transport agent for Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md), and [Create a DeliveryAgent transport agent for Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).</span></span>
  
## <a name="prerequisites-for-creating-a-transport-agent"></a><span data-ttu-id="e8834-115">Pré-requisitos para a criação de um agente de transporte</span><span class="sxs-lookup"><span data-stu-id="e8834-115">Prerequisites for creating a transport agent</span></span>
<span data-ttu-id="e8834-116"><a name="bk_prerequisites"> </a></span><span class="sxs-lookup"><span data-stu-id="e8834-116"><a name="bk_prerequisites"> </a></span></span>

<span data-ttu-id="e8834-117">Estes são os pré-requisitos de que você precisa para implementar um agente de transporte:</span><span class="sxs-lookup"><span data-stu-id="e8834-117">The following are the prerequisites that you need in order to implement a transport agent:</span></span>
  
- <span data-ttu-id="e8834-118">Um computador executando o Exchange 2013 que está executando o serviço de transporte de front end em um servidor de transporte de borda ou acesso para cliente, ou o serviço de transporte em um servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e8834-118">A computer running Exchange 2013 that is running the Front End Transport service on a Client Access or Edge Transport server, or the Transport service on a Mailbox server.</span></span> <span data-ttu-id="e8834-119">Para obter informações sobre a arquitetura de função de servidor no Exchange 2013, consulte [Transport Agent Concepts in exchange 2013](transport-agent-concepts-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="e8834-119">For information about the server role architecture in Exchange 2013, see [Transport agent concepts in Exchange 2013](transport-agent-concepts-in-exchange-2013.md).</span></span>
    
- <span data-ttu-id="e8834-120">Os seguintes assemblies para as classes de agente de transporte:</span><span class="sxs-lookup"><span data-stu-id="e8834-120">The following assemblies for the transport agent classes:</span></span>
    
  - <span data-ttu-id="e8834-121">Microsoft. Exchange. Data. dll</span><span class="sxs-lookup"><span data-stu-id="e8834-121">Microsoft.Exchange.Data.dll</span></span>
    
  - <span data-ttu-id="e8834-122">Microsoft. Exchange. Data. Common. dll</span><span class="sxs-lookup"><span data-stu-id="e8834-122">Microsoft.Exchange.Data.Common.dll</span></span>
    
  - <span data-ttu-id="e8834-123">Microsoft. Exchange. Transport. dll</span><span class="sxs-lookup"><span data-stu-id="e8834-123">Microsoft.Exchange.Transport.dll</span></span>
    
- <span data-ttu-id="e8834-124">O .NET Framework 4,5</span><span class="sxs-lookup"><span data-stu-id="e8834-124">The .NET Framework 4.5</span></span>
    
<span data-ttu-id="e8834-125">Também é recomendável instalar o Visual Studio 2012.</span><span class="sxs-lookup"><span data-stu-id="e8834-125">We also recommend that you install Visual Studio 2012.</span></span> <span data-ttu-id="e8834-126">Você pode implementar agentes de transporte usando o Visual Basic .NET ou C#.</span><span class="sxs-lookup"><span data-stu-id="e8834-126">You can implement transport agents by using either Visual Basic .NET or C#.</span></span>
  
## <a name="referencing-the-assemblies"></a><span data-ttu-id="e8834-127">Fazendo referência aos assemblies</span><span class="sxs-lookup"><span data-stu-id="e8834-127">Referencing the assemblies</span></span>
<span data-ttu-id="e8834-128"><a name="bk_ReferenceAssemblies"> </a></span><span class="sxs-lookup"><span data-stu-id="e8834-128"><a name="bk_ReferenceAssemblies"> </a></span></span>

<span data-ttu-id="e8834-129">O Exchange 2013 fornece uma biblioteca de classes que dão suporte à extensão do comportamento de transporte do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8834-129">Exchange 2013 provides a library of classes that support the extension of Exchange transport behavior.</span></span> <span data-ttu-id="e8834-130">Essas classes exigem o .NET Framework 4,5.</span><span class="sxs-lookup"><span data-stu-id="e8834-130">These classes require the .NET Framework 4.5.</span></span> <span data-ttu-id="e8834-131">Você pode implementar agentes de transporte com base nessas classes usando o Visual Studio 2012.</span><span class="sxs-lookup"><span data-stu-id="e8834-131">You can implement transport agents based on these classes by using Visual Studio 2012.</span></span>
  
<span data-ttu-id="e8834-132">O instalador do Exchange 2013 instala assemblies que são usados para o desenvolvimento do agente de transporte e os registra no cache de assembly global (GAC).</span><span class="sxs-lookup"><span data-stu-id="e8834-132">The Exchange 2013 installer installs assemblies that are used for transport agent development and registers them in the global assembly cache (GAC).</span></span> <span data-ttu-id="e8834-133">Para começar a implementar um agente de transporte, crie uma referência ao assembly Microsoft. Exchange. Data. Transport em um projeto de biblioteca de classes.</span><span class="sxs-lookup"><span data-stu-id="e8834-133">To begin implementing a transport agent, create a reference to the Microsoft.Exchange.Data.Transport assembly in a class library project.</span></span>
  
## <a name="implementing-a-transport-agent"></a><span data-ttu-id="e8834-134">Implementar um agente de transporte</span><span class="sxs-lookup"><span data-stu-id="e8834-134">Implementing a transport agent</span></span>
<span data-ttu-id="e8834-135"><a name="bk_implementationExample"> </a></span><span class="sxs-lookup"><span data-stu-id="e8834-135"><a name="bk_implementationExample"> </a></span></span>

<span data-ttu-id="e8834-136">O exemplo a seguir mostra uma implementação mínima de classes que derivam das classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) e [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e8834-136">The following example shows a minimal implementation of classes that derive from the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes.</span></span> 
  
> [!CAUTION]
> <span data-ttu-id="e8834-137">Se vários agentes de transporte estiverem instalados e registrados para o mesmo evento, todos os agentes serão invocados, mesmo que um agente remova todos os destinatários de um item de email.</span><span class="sxs-lookup"><span data-stu-id="e8834-137">If multiple transport agents are installed and registered for the same event, all agents will be invoked, even if one agent removes all the recipients from a mail item.</span></span> <span data-ttu-id="e8834-138">> para evitar erros não tratados ou comportamento imprevisível, seu agente de transporte deve lidar com casos em que a contagem de destinatários em um item de email é igual a zero.</span><span class="sxs-lookup"><span data-stu-id="e8834-138">> To avoid unhandled errors or unpredictable behavior, your transport agent should handle cases in which the recipient count on a mail item is equal to zero.</span></span> 
  
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

## <a name="installing-and-enabling-an-agent"></a><span data-ttu-id="e8834-139">Instalando e habilitando um agente</span><span class="sxs-lookup"><span data-stu-id="e8834-139">Installing and enabling an agent</span></span>
<span data-ttu-id="e8834-140"><a name="bk_InstallEnable"> </a></span><span class="sxs-lookup"><span data-stu-id="e8834-140"><a name="bk_InstallEnable"> </a></span></span>

<span data-ttu-id="e8834-141">Depois de compilar o seu agente para uma DLL, você deve instalar e habilitar o agente no seu servidor do Exchange de desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="e8834-141">After you compile your agent to a DLL, you must install and enable the agent on your development Exchange server.</span></span> <span data-ttu-id="e8834-142">No Shell de gerenciamento do Exchange, use o cmdlet [Install-TransportAgent](https://technet.microsoft.com/library/aa997998.aspx) para instalar o seu agente e o cmdlet [Enable-TransportAgent](https://technet.microsoft.com/library/bb124921.aspx) para habilitar o seu agente.</span><span class="sxs-lookup"><span data-stu-id="e8834-142">In the Exchange Management Shell, use the [Install-TransportAgent](https://technet.microsoft.com/library/aa997998.aspx) cmdlet to install your agent, and the [Enable-TransportAgent](https://technet.microsoft.com/library/bb124921.aspx) cmdlet to enable your agent.</span></span> <span data-ttu-id="e8834-143">Para obter informações sobre como usar o Shell de gerenciamento do Exchange, consulte [Exchange Server PowerShell (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="e8834-143">For information about how to use the Exchange Management Shell, see [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).</span></span>
  
> [!CAUTION]
> <span data-ttu-id="e8834-144">Os agentes de transporte têm acesso total a todas as mensagens de email que encontrarem.</span><span class="sxs-lookup"><span data-stu-id="e8834-144">Transport agents have full access to all email messages that they encounter.</span></span> <span data-ttu-id="e8834-145">O Exchange 2013 não restringe o comportamento de um agente de transporte.</span><span class="sxs-lookup"><span data-stu-id="e8834-145">Exchange 2013 does not restrict the behavior of a transport agent.</span></span> <span data-ttu-id="e8834-146">Os agentes de transporte instáveis ou que contêm falhas de segurança podem afetar a estabilidade e a segurança do Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="e8834-146">Transport agents that are unstable or that contain security flaws might affect the stability and security of Exchange 2013.</span></span> <span data-ttu-id="e8834-147">Portanto, você deve instalar somente agentes de transporte com confiança total e que foram totalmente testados.</span><span class="sxs-lookup"><span data-stu-id="e8834-147">Therefore, you should only install transport agents that you fully trust and that have been fully tested.</span></span> 
  
<span data-ttu-id="e8834-148">Quando você usa o cmdlet **Install-TransportAgent** para instalar um agente, o Shell de gerenciamento do Exchange mantém um bloqueio no assembly.</span><span class="sxs-lookup"><span data-stu-id="e8834-148">When you use the **Install-TransportAgent** cmdlet to install an agent, the Exchange Management Shell keeps a lock on the assembly.</span></span> <span data-ttu-id="e8834-149">Para liberar o bloqueio no assembly, você deve fechar a instância do Shell de gerenciamento do Exchange que você usou para instalar o agente.</span><span class="sxs-lookup"><span data-stu-id="e8834-149">To release the lock on the assembly, you must close the instance of the Exchange Management Shell that you used to install the agent.</span></span> <span data-ttu-id="e8834-150">Você não poderá atualizar o assembly até que você libere o bloqueio.</span><span class="sxs-lookup"><span data-stu-id="e8834-150">You will be unable to update the assembly until you release the lock.</span></span> 
  
<span data-ttu-id="e8834-151">O exemplo a seguir mostra como usar o Shell de gerenciamento do Exchange para instalar e habilitar um agente chamado myagent usando uma classe derivada de [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) chamada myagents. MyAgentFactory.</span><span class="sxs-lookup"><span data-stu-id="e8834-151">The following example shows how to use the Exchange Management Shell to install and enable an agent named MyAgent by using a class derived from [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) named MyAgents.MyAgentFactory.</span></span> 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
<span data-ttu-id="e8834-152">Este exemplo nomeia o agente MyCustomAgent no servidor no qual o agente está instalado.</span><span class="sxs-lookup"><span data-stu-id="e8834-152">This example names the agent MyCustomAgent on the server on which the agent is installed.</span></span> <span data-ttu-id="e8834-153">O exemplo a seguir mostra como habilitar o agente chamado MyCustomAgent.</span><span class="sxs-lookup"><span data-stu-id="e8834-153">The following example shows how to enable the agent named MyCustomAgent.</span></span>
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
<span data-ttu-id="e8834-154">Para gerenciar um agente de transporte no serviço de transporte de front-end em um servidor de acesso para cliente, adicione o seguinte valor ao comando: `-TransportService FrontEnd` .</span><span class="sxs-lookup"><span data-stu-id="e8834-154">To manage a transport agent in the Front End Transport service on a Client Access server, add the following value to the command:  `-TransportService FrontEnd`.</span></span> <span data-ttu-id="e8834-155">Por exemplo, para exibir os agentes de transporte no serviço de transporte de front-end, execute o comando a seguir.</span><span class="sxs-lookup"><span data-stu-id="e8834-155">For example, to view the transport agents in the Front End Transport service, run the following command.</span></span>
  
 `Get-TransportAgent -TransportService FrontEnd`
  
<span data-ttu-id="e8834-156">Para obter mais informações sobre como instalar, habilitar e gerenciar o seu agente, consulte [Manage Transport Agents](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="e8834-156">For more information about installing, enabling, and managing your agent, see [Manage Transport Agents](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="e8834-157">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="e8834-157">In this section</span></span>
<span data-ttu-id="e8834-158"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="e8834-158"><a name="bk_inthissection"> </a></span></span>

- [<span data-ttu-id="e8834-159">Criar um agente de transporte RoutingAgent para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e8834-159">Create a RoutingAgent transport agent for Exchange 2013</span></span>](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [<span data-ttu-id="e8834-160">Criar um agente de transporte SmtpReceiveAgent para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e8834-160">Create an SmtpReceiveAgent transport agent for Exchange 2013</span></span>](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [<span data-ttu-id="e8834-161">Criar um agente de transporte DeliveryAgent para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e8834-161">Create a DeliveryAgent transport agent for Exchange 2013</span></span>](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="e8834-162">Também consulte</span><span class="sxs-lookup"><span data-stu-id="e8834-162">See also</span></span>

- [<span data-ttu-id="e8834-163">Conceitos de agente de transporte no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e8834-163">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)   
- [<span data-ttu-id="e8834-164">Referência do agente de transporte para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e8834-164">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
    

