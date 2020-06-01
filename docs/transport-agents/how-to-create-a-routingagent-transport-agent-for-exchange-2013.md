---
title: Criar um agente de transporte RoutingAgent para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f0e745f-9289-4f31-8877-926692a8c133
description: Descubra como criar um agente de transporte RoutingAgent personalizado para usar com o Exchange 2013.
ms.openlocfilehash: 9acf30be0dd795098f757effaa34b2e72183b000
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463696"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="9f454-103">Criar um agente de transporte RoutingAgent para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="9f454-103">Create a RoutingAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="9f454-104">Descubra como criar um agente de transporte RoutingAgent personalizado para usar com o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="9f454-104">Find out how to create a custom RoutingAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="9f454-105">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="9f454-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="9f454-106">Trechos de código relacionados e aplicativos de exemplo:</span><span class="sxs-lookup"><span data-stu-id="9f454-106">Related code snippets and sample apps:</span></span>

- [<span data-ttu-id="9f454-107">Exchange 2013: criar um agente de transporte de log de largura de banda</span><span class="sxs-lookup"><span data-stu-id="9f454-107">Exchange 2013: Build a bandwidth logging transport agent</span></span>](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
<span data-ttu-id="9f454-108">As classes [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) e [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) são as classes base para agentes de transporte projetados para serem executados no serviço de transporte em um servidor de caixa de correio do Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9f454-108">The [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) and [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) classes are the base classes for transport agents that are designed to run on the transport service on an Exchange Server 2013 Mailbox server.</span></span> <span data-ttu-id="9f454-109">A classe [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) fornece os eventos listados na tabela a seguir para o qual você pode implementar manipuladores no seu agente de transporte do RoutingAgent.</span><span class="sxs-lookup"><span data-stu-id="9f454-109">The [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) class provides the events listed in the following table for which you might implement handlers in your RoutingAgent transport agent.</span></span> 
  
<span data-ttu-id="9f454-110">**Tabela 1. Eventos de classe RoutingAgent**</span><span class="sxs-lookup"><span data-stu-id="9f454-110">**Table 1. RoutingAgent class events**</span></span>

|<span data-ttu-id="9f454-111">**Evento**</span><span class="sxs-lookup"><span data-stu-id="9f454-111">**Event**</span></span>|<span data-ttu-id="9f454-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9f454-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f454-113">OnCategorizedMessage</span><span class="sxs-lookup"><span data-stu-id="9f454-113">OnCategorizedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |<span data-ttu-id="9f454-114">Ocorre após o servidor executar a conversão de conteúdo, se for necessário.</span><span class="sxs-lookup"><span data-stu-id="9f454-114">Occurs after the server performs content conversion, if it is required.</span></span>  <br/> |
|[<span data-ttu-id="9f454-115">OnResolvedMessage</span><span class="sxs-lookup"><span data-stu-id="9f454-115">OnResolvedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |<span data-ttu-id="9f454-116">Ocorre depois que todos os destinatários da mensagem foram resolvidos e antes de o roteamento ser determinado.</span><span class="sxs-lookup"><span data-stu-id="9f454-116">Occurs after all the recipients of the message have been resolved and before routing is determined.</span></span>  <br/> |
|[<span data-ttu-id="9f454-117">OnRoutedMessage</span><span class="sxs-lookup"><span data-stu-id="9f454-117">OnRoutedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |<span data-ttu-id="9f454-118">Ocorre após o servidor direcionar a mensagem para o próximo salto e realizar a conversão de conteúdo, se necessário.</span><span class="sxs-lookup"><span data-stu-id="9f454-118">Occurs after the server routes the message to the next hop and performs content conversion, if required.</span></span> <span data-ttu-id="9f454-119">O servidor pode usar mais recursos para processar cada mensagem no evento [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) do que o evento [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) , pois o servidor executará qualquer conversão de conteúdo necessária e determinará o próximo salto na rota da mensagem antes de executar o código no manipulador de eventos [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) .</span><span class="sxs-lookup"><span data-stu-id="9f454-119">The server might use more resources to process each message in the [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) event than the [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) event because the server will perform any necessary content conversion and determine the next hop in the route for the message before it executes the code in the [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) event handler.</span></span>  <br/> |
|[<span data-ttu-id="9f454-120">OnSubmittedMessage</span><span class="sxs-lookup"><span data-stu-id="9f454-120">OnSubmittedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |<span data-ttu-id="9f454-121">Ocorre depois que a mensagem é retirada da fila de envio.</span><span class="sxs-lookup"><span data-stu-id="9f454-121">Occurs after the message is taken off the submit queue.</span></span> <span data-ttu-id="9f454-122">Use o evento [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) se o seu agente de transporte do RoutingAgent não exigir conversão de conteúdo, destinatários resolvidos ou dados de roteamento.</span><span class="sxs-lookup"><span data-stu-id="9f454-122">Use the [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) event if your RoutingAgent transport agent does not require content conversion, resolved recipients, or routing data.</span></span>  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a><span data-ttu-id="9f454-123">Criar um agente de transporte RoutingAgent personalizado</span><span class="sxs-lookup"><span data-stu-id="9f454-123">Creating a custom RoutingAgent transport agent</span></span>

<span data-ttu-id="9f454-124">O procedimento a seguir descreve como criar um agente de transporte RoutingAgent personalizado.</span><span class="sxs-lookup"><span data-stu-id="9f454-124">The following procedure describes how to create a custom RoutingAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="9f454-125">Para criar o agente de transporte</span><span class="sxs-lookup"><span data-stu-id="9f454-125">To create the transport agent</span></span>

1. <span data-ttu-id="9f454-126">Adicione referências aos namespaces.</span><span class="sxs-lookup"><span data-stu-id="9f454-126">Add references to the namespaces.</span></span>
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   <span data-ttu-id="9f454-127">Você pode encontrar esses namespaces no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f454-127">You can find these namespaces on your Exchange server.</span></span> <span data-ttu-id="9f454-128">Ao adicionar uma referência a esses namespaces, você terá acesso aos membros do [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) , bem como outras classes usadas no [Exchange 2013: criar um exemplo de agente de transporte de log de largura de banda](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) .</span><span class="sxs-lookup"><span data-stu-id="9f454-128">By adding a reference to these namespaces, you will have access to the [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) members as well as other classes used in the [Exchange 2013: Build a bandwidth logging transport agent](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) sample.</span></span> 
    
2. <span data-ttu-id="9f454-129">Implemente a classe derivada da classe [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="9f454-129">Implement the derived class for the [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) class.</span></span> 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   <span data-ttu-id="9f454-130">Este código criará uma instância da classe derivada e substituirá o método **CreateAgent** para criar uma instância do seu novo agente personalizado.</span><span class="sxs-lookup"><span data-stu-id="9f454-130">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> <span data-ttu-id="9f454-131">Métodos adicionais, como **Close**, também podem ser substituídos nessa classe para executar código personalizado.</span><span class="sxs-lookup"><span data-stu-id="9f454-131">Additional methods, such as **Close**, can also be overridden in this class to execute custom code.</span></span> 
    
3. <span data-ttu-id="9f454-132">Defina seu agente.</span><span class="sxs-lookup"><span data-stu-id="9f454-132">Define your agent.</span></span>
    
   ```cs
      public class BandwidthLogger : RoutingAgent
      {
          // Your custom code goes here
          public BandwidthLogger(SmtpServer server)
          {
              Debug.WriteLine(logPrefix + "Agent constructor");
              this.server = server;
              this.OnSubmittedMessage += SubmittedMessage;
              this.OnRoutedMessage += RoutedMessage;
          }
      }
  
   ```

   <span data-ttu-id="9f454-133">Depois de definir sua classe de agente, você pode adicionar a funcionalidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="9f454-133">After you define your agent class, you can add you custom functionality.</span></span> <span data-ttu-id="9f454-134">Neste exemplo, os dois eventos [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) e [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)são redirecionados para seus manipuladores de eventos personalizados.</span><span class="sxs-lookup"><span data-stu-id="9f454-134">In this example, the two events [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) and [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)are redirected to your custom event handlers.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="9f454-135">Também consulte</span><span class="sxs-lookup"><span data-stu-id="9f454-135">See also</span></span>

- [<span data-ttu-id="9f454-136">Conceitos de agente de transporte no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="9f454-136">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)    
- [<span data-ttu-id="9f454-137">Referência do agente de transporte para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="9f454-137">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="9f454-138">RoutingAgentFactory</span><span class="sxs-lookup"><span data-stu-id="9f454-138">RoutingAgentFactory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [<span data-ttu-id="9f454-139">RoutingAgent</span><span class="sxs-lookup"><span data-stu-id="9f454-139">RoutingAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

