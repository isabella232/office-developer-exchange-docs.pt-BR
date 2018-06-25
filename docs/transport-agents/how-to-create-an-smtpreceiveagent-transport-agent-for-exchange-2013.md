---
title: Criar um agente de transporte SmtpReceiveAgent para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cdc7c462-74a7-49d6-95b2-155d783840e9
description: Descubra como criar um agente de transporte SmtpReceiveAgent personalizado para usar com o Exchange 2013.
ms.openlocfilehash: a74d5baae6334c5e17acb6335206964b48f320e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751125"
---
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="45627-103">Criar um agente de transporte SmtpReceiveAgent para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="45627-103">Create an SmtpReceiveAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="45627-104">Descubra como criar um agente de transporte SmtpReceiveAgent personalizado para usar com o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="45627-104">Find out how to create a custom SmtpReceiveAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="45627-105">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="45627-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="45627-106">Relacionadas a aplicativos de exemplo e trechos de código:</span><span class="sxs-lookup"><span data-stu-id="45627-106">Related code snippets and sample apps:</span></span>

- [<span data-ttu-id="45627-107">Exchange 2013: Criar um agente de transporte de conversão de corpo</span><span class="sxs-lookup"><span data-stu-id="45627-107">Exchange 2013: Build a body conversion transport agent</span></span>](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
<span data-ttu-id="45627-108">As classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) e [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) permitem estender o comportamento do serviço Front End Transport em um servidor de acesso para cliente ou o serviço de transporte em um servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="45627-108">The [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes enable you to extend the behavior of the Front End Transport service on a Client Access Server or the Transport service on a Mailbox server.</span></span> <span data-ttu-id="45627-109">Você pode usar essas classes para implementar os agentes de transporte que foram projetados para responder às mensagens como eles entram em sua organização.</span><span class="sxs-lookup"><span data-stu-id="45627-109">You can use these classes to implement transport agents that are designed to respond to messages as they come into your organization.</span></span> 
  
<span data-ttu-id="45627-110">As classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) e [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) incluem os eventos listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="45627-110">The [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes include the events listed in the following table.</span></span> 
  
<span data-ttu-id="45627-111">**Tabela 1. Eventos de classe SmtpReceiveAgent**</span><span class="sxs-lookup"><span data-stu-id="45627-111">**Table 1. SmtpReceiveAgent class events**</span></span>

|<span data-ttu-id="45627-112">**Event**</span><span class="sxs-lookup"><span data-stu-id="45627-112">**Event**</span></span>|<span data-ttu-id="45627-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="45627-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45627-114">OnAuthCommand</span><span class="sxs-lookup"><span data-stu-id="45627-114">OnAuthCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |<span data-ttu-id="45627-115">Quando seu agente exige informações que são fornecidas apenas no comando SMTP **AUTH** , como um operador que aceita ou rejeita tenta enviar uma mensagem com base no tipo de método de autenticação usado para uso.</span><span class="sxs-lookup"><span data-stu-id="45627-115">Use when your agent requires information that is provided only in the SMTP **AUTH** command, such as an agent that accepts or rejects attempts to deliver a message based on the type of authentication method used.</span></span>  <br/> |
|[<span data-ttu-id="45627-116">OnConnect</span><span class="sxs-lookup"><span data-stu-id="45627-116">OnConnect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |<span data-ttu-id="45627-117">Use quando seu agente exige informações que são fornecidas apenas quando uma conexão é aberta por meio de SMTP para o serviço de Front End Transport, como um operador que está executando uma ação com base no endereço ou no domínio do servidor SMTP remoto.</span><span class="sxs-lookup"><span data-stu-id="45627-117">Use when your agent requires information that is provided only when a connection is opened via SMTP to the Front End Transport service, such as an agent that performs an action based on the address or domain of the remote SMTP server.</span></span>  <br/> |
|[<span data-ttu-id="45627-118">OnDataCommand</span><span class="sxs-lookup"><span data-stu-id="45627-118">OnDataCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |<span data-ttu-id="45627-119">Use este evento quando seu agente requer as informações fornecidas no comando SMTP **dados** .</span><span class="sxs-lookup"><span data-stu-id="45627-119">Use this event when your agent requires information that is provided in the SMTP **DATA** command.</span></span>  <br/> |
|[<span data-ttu-id="45627-120">OnDisconnect</span><span class="sxs-lookup"><span data-stu-id="45627-120">OnDisconnect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |<span data-ttu-id="45627-121">Use quando seu agente exige informações que está disponíveis no momento da desconexão, como a data e hora atuais, para executar cálculos de tempo.</span><span class="sxs-lookup"><span data-stu-id="45627-121">Use when your agent requires information that is available at the time of disconnection, such as the current date and time, in order to perform time calculations.</span></span>  <br/> |
|[<span data-ttu-id="45627-122">OnEhloCommand</span><span class="sxs-lookup"><span data-stu-id="45627-122">OnEhloCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |<span data-ttu-id="45627-123">Uso quando seu agente requer as informações fornecidas no comando SMTP **EHLO** ; Por exemplo, se seu operador a aceita ou rejeita mensagens com base na identidade fornecida no comando **EHLO** .</span><span class="sxs-lookup"><span data-stu-id="45627-123">Use when your agent requires information that is provided in the SMTP **EHLO** command; for example, if your agent accepts or rejects messages based on the identity provided in the **EHLO** command.</span></span>  <br/> |
|[<span data-ttu-id="45627-124">OnEndOfAuthentication</span><span class="sxs-lookup"><span data-stu-id="45627-124">OnEndOfAuthentication</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |<span data-ttu-id="45627-125">Use quando seu agente exige informações que está disponíveis depois que o servidor remoto conclui o processo de autenticação; Por exemplo, para um operador que está executando uma ação em uma mensagem com base nas informações de autenticação fornecidas pelo cliente ou servidor SMTP remoto.</span><span class="sxs-lookup"><span data-stu-id="45627-125">Use when your agent requires information that is available after the remote server completes the authentication process; for example, for an agent that performs an action on a message based on the authentication information provided by the remote SMTP server or client.</span></span>  <br/> |
|[<span data-ttu-id="45627-126">OnEndOfData</span><span class="sxs-lookup"><span data-stu-id="45627-126">OnEndOfData</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |<span data-ttu-id="45627-127">Use quando seu agente deve executar uma ação com base nos dados que está disponíveis na mensagem.</span><span class="sxs-lookup"><span data-stu-id="45627-127">Use when your agent must perform an action based on data that is available in the message.</span></span> <span data-ttu-id="45627-128">Esse evento não será acionado no serviço Front End Transport.</span><span class="sxs-lookup"><span data-stu-id="45627-128">This event will not fire on the Front End Transport service.</span></span> <span data-ttu-id="45627-129">Se o agente de transporte precisa usar esse evento, você precisa instalá-lo em um servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="45627-129">If your transport agent has to use this event, you have to install it on a Mailbox server.</span></span>  <br/> |
|[<span data-ttu-id="45627-130">OnEndOfHeaders</span><span class="sxs-lookup"><span data-stu-id="45627-130">OnEndOfHeaders</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |<span data-ttu-id="45627-131">Use quando seu agente deve executar uma ação com base nas informações que está disponíveis nos cabeçalhos da mensagem enviada.</span><span class="sxs-lookup"><span data-stu-id="45627-131">Use when your agent must perform an action based on information that is available in the headers of the submitted message.</span></span>  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a><span data-ttu-id="45627-132">Criando um agente de transporte SmtpReceiveAgent personalizado</span><span class="sxs-lookup"><span data-stu-id="45627-132">Creating a custom SmtpReceiveAgent transport agent</span></span>

<span data-ttu-id="45627-133">O procedimento a seguir descreve como criar um agente de transporte SmtpReceiveAgent personalizado.</span><span class="sxs-lookup"><span data-stu-id="45627-133">The following procedure describes how to create a custom SmtpReceiveAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="45627-134">Para criar o agente de transporte</span><span class="sxs-lookup"><span data-stu-id="45627-134">To create the transport agent</span></span>

1. <span data-ttu-id="45627-135">Adicione referências para os namespaces.</span><span class="sxs-lookup"><span data-stu-id="45627-135">Add references to the namespaces.</span></span>
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   <span data-ttu-id="45627-136">Você pode encontrar esses espaços para nome no seu servidor Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="45627-136">You can find these namespaces on your Exchange 2013 server.</span></span> <span data-ttu-id="45627-137">Quando você adiciona uma referência a esses espaços para nome, você terá acesso aos membros [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) bem como outros classes usadas no [Exchange 2013: criar um agente de transporte de conversão de corpo](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) amostra.</span><span class="sxs-lookup"><span data-stu-id="45627-137">When you add a reference to these namespaces, you will have access to the [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) members as well as other classes used in the [Exchange 2013: Build a body conversion transport agent](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) sample.</span></span> 
    
2. <span data-ttu-id="45627-138">Implemente a classe derivada da classe [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="45627-138">Implement the derived class for the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) class.</span></span> 
    
   ```cs
      public class BodyConversionFactory : SmtpReceiveAgentFactory
      {
          /// <summary>
          /// Create a new BodyConversion
          /// </summary>
          /// <param name="server">Exchange server</param>
          /// <returns>A new BodyConversion</returns>
          public override SmtpReceiveAgent CreateAgent(SmtpServer server)
          {
              return new BodyConversion();
          }
      }
  
   ```

   <span data-ttu-id="45627-139">Este código será instanciar a classe derivada e substitua o método **CreateAgent** para criar uma instância do seu novo agente personalizado.</span><span class="sxs-lookup"><span data-stu-id="45627-139">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> 
    
3. <span data-ttu-id="45627-140">Defina seu agente.</span><span class="sxs-lookup"><span data-stu-id="45627-140">Define your agent.</span></span>
    
   ```cs
     public class BodyConversion : SmtpReceiveAgent
      {
          // Your custom code goes here
          /// <summary>
          /// The constructor registers an end of data event handler.
          /// </summary>
          public BodyConversion()
          {
              Debug.WriteLine("[BodyConversion] Agent constructor");
              this.OnEndOfData += new EndOfDataEventHandler(this.OnEndOfDataHandler);
          }
      }
  
   ```

   <span data-ttu-id="45627-141">Depois de definir seu classe de agente, você pode adicionar sua funcionalidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="45627-141">After you define your agent class, you can add your custom functionality.</span></span> <span data-ttu-id="45627-142">Neste exemplo, o evento [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) é redirecionado para o manipulador de eventos personalizados.</span><span class="sxs-lookup"><span data-stu-id="45627-142">In this example, the [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) event is redirected to your custom event handler.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="45627-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="45627-143">See also</span></span>

- [<span data-ttu-id="45627-144">Transporte conceitos de agente no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="45627-144">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)    
- [<span data-ttu-id="45627-145">Referência de agente de transporte do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="45627-145">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="45627-146">SmtpReceiveAgentFactory</span><span class="sxs-lookup"><span data-stu-id="45627-146">SmtpReceiveAgentFactory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [<span data-ttu-id="45627-147">SmtpReceiveAgent</span><span class="sxs-lookup"><span data-stu-id="45627-147">SmtpReceiveAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

