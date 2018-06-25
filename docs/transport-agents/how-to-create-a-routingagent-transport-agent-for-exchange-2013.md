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
ms.openlocfilehash: d07f68494acd26940a4837bbbfc7a0505114bd20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751009"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="22267-103">Criar um agente de transporte RoutingAgent para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="22267-103">Create a RoutingAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="22267-104">Descubra como criar um agente de transporte RoutingAgent personalizado para usar com o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="22267-104">Find out how to create a custom RoutingAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="22267-105">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="22267-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="22267-106">Relacionadas a aplicativos de exemplo e trechos de código:</span><span class="sxs-lookup"><span data-stu-id="22267-106">Related code snippets and sample apps:</span></span>

- [<span data-ttu-id="22267-107">Exchange 2013: Criar um agente de transporte de registro em log de largura de banda</span><span class="sxs-lookup"><span data-stu-id="22267-107">Exchange 2013: Build a bandwidth logging transport agent</span></span>](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
<span data-ttu-id="22267-108">As classes [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) e [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) são as classes base para os agentes de transporte que são projetados para executar o serviço de transporte em um servidor de caixa de correio do Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="22267-108">The [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) and [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) classes are the base classes for transport agents that are designed to run on the transport service on an Exchange Server 2013 Mailbox server.</span></span> <span data-ttu-id="22267-109">A classe [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) fornece os eventos listados na tabela a seguir para o qual você pode implementar manipuladores em seu agente de transporte RoutingAgent.</span><span class="sxs-lookup"><span data-stu-id="22267-109">The [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) class provides the events listed in the following table for which you might implement handlers in your RoutingAgent transport agent.</span></span> 
  
<span data-ttu-id="22267-110">**Tabela 1. Eventos de classe RoutingAgent**</span><span class="sxs-lookup"><span data-stu-id="22267-110">**Table 1. RoutingAgent class events**</span></span>

|<span data-ttu-id="22267-111">**Event**</span><span class="sxs-lookup"><span data-stu-id="22267-111">**Event**</span></span>|<span data-ttu-id="22267-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="22267-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22267-113">OnCategorizedMessage</span><span class="sxs-lookup"><span data-stu-id="22267-113">OnCategorizedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |<span data-ttu-id="22267-114">Ocorre depois que o servidor executa a conversão de conteúdo, se for necessário.</span><span class="sxs-lookup"><span data-stu-id="22267-114">Occurs after the server performs content conversion, if it is required.</span></span>  <br/> |
|[<span data-ttu-id="22267-115">OnResolvedMessage</span><span class="sxs-lookup"><span data-stu-id="22267-115">OnResolvedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |<span data-ttu-id="22267-116">Ocorre após todos os destinatários da mensagem foram resolvidos e antes de roteamento é determinado.</span><span class="sxs-lookup"><span data-stu-id="22267-116">Occurs after all the recipients of the message have been resolved and before routing is determined.</span></span>  <br/> |
|[<span data-ttu-id="22267-117">OnRoutedMessage</span><span class="sxs-lookup"><span data-stu-id="22267-117">OnRoutedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |<span data-ttu-id="22267-118">Ocorre depois que o servidor encaminha a mensagem para o próximo salto e executa a conversão de conteúdo, se necessário.</span><span class="sxs-lookup"><span data-stu-id="22267-118">Occurs after the server routes the message to the next hop and performs content conversion, if required.</span></span> <span data-ttu-id="22267-119">O servidor pode usar mais recursos para processar cada mensagem no evento [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) do evento [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) porque o servidor executar nenhuma conversão de conteúdo necessário e determinar o próximo salto na rota da mensagem antes de executar o código no manipulador de eventos [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) .</span><span class="sxs-lookup"><span data-stu-id="22267-119">The server might use more resources to process each message in the [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) event than the [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) event because the server will perform any necessary content conversion and determine the next hop in the route for the message before it executes the code in the [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) event handler.</span></span>  <br/> |
|[<span data-ttu-id="22267-120">OnSubmittedMessage</span><span class="sxs-lookup"><span data-stu-id="22267-120">OnSubmittedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |<span data-ttu-id="22267-121">Ocorre depois que a mensagem for retirada a fila de envio.</span><span class="sxs-lookup"><span data-stu-id="22267-121">Occurs after the message is taken off the submit queue.</span></span> <span data-ttu-id="22267-122">Use o evento [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) se o agente de transporte RoutingAgent não exigir dados de roteamento, resolvidos destinatários ou conversão de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="22267-122">Use the [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) event if your RoutingAgent transport agent does not require content conversion, resolved recipients, or routing data.</span></span>  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a><span data-ttu-id="22267-123">Criando um agente de transporte RoutingAgent personalizado</span><span class="sxs-lookup"><span data-stu-id="22267-123">Creating a custom RoutingAgent transport agent</span></span>

<span data-ttu-id="22267-124">O procedimento a seguir descreve como criar um agente de transporte RoutingAgent personalizado.</span><span class="sxs-lookup"><span data-stu-id="22267-124">The following procedure describes how to create a custom RoutingAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="22267-125">Para criar o agente de transporte</span><span class="sxs-lookup"><span data-stu-id="22267-125">To create the transport agent</span></span>

1. <span data-ttu-id="22267-126">Adicione referências para os namespaces.</span><span class="sxs-lookup"><span data-stu-id="22267-126">Add references to the namespaces.</span></span>
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   <span data-ttu-id="22267-127">Você pode encontrar esses namespaces em seu servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="22267-127">You can find these namespaces on your Exchange server.</span></span> <span data-ttu-id="22267-128">Adicionando uma referência a esses espaços para nome, você terá acesso aos membros [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) bem como outros classes usadas no [Exchange 2013: criar um agente de transporte do log de largura de banda](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) amostra.</span><span class="sxs-lookup"><span data-stu-id="22267-128">By adding a reference to these namespaces, you will have access to the [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) members as well as other classes used in the [Exchange 2013: Build a bandwidth logging transport agent](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) sample.</span></span> 
    
2. <span data-ttu-id="22267-129">Implemente a classe derivada da classe [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="22267-129">Implement the derived class for the [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) class.</span></span> 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   <span data-ttu-id="22267-130">Este código será instanciar a classe derivada e substitua o método **CreateAgent** para criar uma instância do seu novo agente personalizado.</span><span class="sxs-lookup"><span data-stu-id="22267-130">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> <span data-ttu-id="22267-131">Métodos adicionais, como **Fechar**, também podem ser substituídos nesta classe para executar código personalizado.</span><span class="sxs-lookup"><span data-stu-id="22267-131">Additional methods, such as **Close**, can also be overridden in this class to execute custom code.</span></span> 
    
3. <span data-ttu-id="22267-132">Defina seu agente.</span><span class="sxs-lookup"><span data-stu-id="22267-132">Define your agent.</span></span>
    
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

   <span data-ttu-id="22267-133">Depois de definir seu classe de agente, você pode adicionar a você uma funcionalidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="22267-133">After you define your agent class, you can add you custom functionality.</span></span> <span data-ttu-id="22267-134">Neste exemplo, os dois eventos [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) e [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)serão redirecionados para seus manipuladores de eventos personalizados.</span><span class="sxs-lookup"><span data-stu-id="22267-134">In this example, the two events [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) and [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)are redirected to your custom event handlers.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="22267-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="22267-135">See also</span></span>

- [<span data-ttu-id="22267-136">Transporte conceitos de agente no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="22267-136">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)    
- [<span data-ttu-id="22267-137">Referência de agente de transporte do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="22267-137">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="22267-138">RoutingAgentFactory</span><span class="sxs-lookup"><span data-stu-id="22267-138">RoutingAgentFactory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [<span data-ttu-id="22267-139">RoutingAgent</span><span class="sxs-lookup"><span data-stu-id="22267-139">RoutingAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

