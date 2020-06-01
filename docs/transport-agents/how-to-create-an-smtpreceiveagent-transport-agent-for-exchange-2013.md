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
ms.openlocfilehash: 5ba021d02849ffc7e125029f0fd18ebf14c3f8da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459136"
---
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="4f974-103">Criar um agente de transporte SmtpReceiveAgent para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="4f974-103">Create an SmtpReceiveAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="4f974-104">Descubra como criar um agente de transporte SmtpReceiveAgent personalizado para usar com o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="4f974-104">Find out how to create a custom SmtpReceiveAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="4f974-105">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="4f974-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="4f974-106">Trechos de código relacionados e aplicativos de exemplo:</span><span class="sxs-lookup"><span data-stu-id="4f974-106">Related code snippets and sample apps:</span></span>

- [<span data-ttu-id="4f974-107">Exchange 2013: criar um agente de transporte de conversão de corpo</span><span class="sxs-lookup"><span data-stu-id="4f974-107">Exchange 2013: Build a body conversion transport agent</span></span>](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
<span data-ttu-id="4f974-108">As classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) e [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) permitem que você estenda o comportamento do serviço de transporte de front-end em um servidor de acesso para cliente ou no serviço de transporte em um servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4f974-108">The [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes enable you to extend the behavior of the Front End Transport service on a Client Access Server or the Transport service on a Mailbox server.</span></span> <span data-ttu-id="4f974-109">Você pode usar essas classes para implementar agentes de transporte projetados para responder às mensagens à medida que elas entram na sua organização.</span><span class="sxs-lookup"><span data-stu-id="4f974-109">You can use these classes to implement transport agents that are designed to respond to messages as they come into your organization.</span></span> 
  
<span data-ttu-id="4f974-110">As classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) e [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) incluem os eventos listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="4f974-110">The [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes include the events listed in the following table.</span></span> 
  
<span data-ttu-id="4f974-111">**Tabela 1. Eventos de classe SmtpReceiveAgent**</span><span class="sxs-lookup"><span data-stu-id="4f974-111">**Table 1. SmtpReceiveAgent class events**</span></span>

|<span data-ttu-id="4f974-112">**Evento**</span><span class="sxs-lookup"><span data-stu-id="4f974-112">**Event**</span></span>|<span data-ttu-id="4f974-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4f974-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f974-114">OnAuthCommand</span><span class="sxs-lookup"><span data-stu-id="4f974-114">OnAuthCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |<span data-ttu-id="4f974-115">Use quando o seu agente exigir informações fornecidas apenas no comando de **autenticação** SMTP, como um agente que aceita ou rejeita tentativas de entrega de mensagens com base no tipo de método de autenticação usado.</span><span class="sxs-lookup"><span data-stu-id="4f974-115">Use when your agent requires information that is provided only in the SMTP **AUTH** command, such as an agent that accepts or rejects attempts to deliver a message based on the type of authentication method used.</span></span>  <br/> |
|[<span data-ttu-id="4f974-116">OnConnect</span><span class="sxs-lookup"><span data-stu-id="4f974-116">OnConnect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |<span data-ttu-id="4f974-117">Use quando o seu agente exigir informações fornecidas somente quando uma conexão for aberta via SMTP para o serviço de transporte de front-end, como um agente que executa uma ação com base no endereço ou domínio do servidor SMTP remoto.</span><span class="sxs-lookup"><span data-stu-id="4f974-117">Use when your agent requires information that is provided only when a connection is opened via SMTP to the Front End Transport service, such as an agent that performs an action based on the address or domain of the remote SMTP server.</span></span>  <br/> |
|[<span data-ttu-id="4f974-118">OnDataCommand</span><span class="sxs-lookup"><span data-stu-id="4f974-118">OnDataCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |<span data-ttu-id="4f974-119">Use este evento quando o seu agente exigir informações fornecidas no comando de **dados** SMTP.</span><span class="sxs-lookup"><span data-stu-id="4f974-119">Use this event when your agent requires information that is provided in the SMTP **DATA** command.</span></span>  <br/> |
|[<span data-ttu-id="4f974-120">OnDisconnect</span><span class="sxs-lookup"><span data-stu-id="4f974-120">OnDisconnect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |<span data-ttu-id="4f974-121">Use quando o seu agente exigir informações disponíveis no momento da desconexão, como a data e hora atuais, para executar cálculos de tempo.</span><span class="sxs-lookup"><span data-stu-id="4f974-121">Use when your agent requires information that is available at the time of disconnection, such as the current date and time, in order to perform time calculations.</span></span>  <br/> |
|[<span data-ttu-id="4f974-122">OnEhloCommand</span><span class="sxs-lookup"><span data-stu-id="4f974-122">OnEhloCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |<span data-ttu-id="4f974-123">Use quando o seu agente exigir informações fornecidas no comando **EHLO** do SMTP; por exemplo, se o seu agente aceitar ou rejeitar mensagens com base na identidade fornecida no comando **EHLO** .</span><span class="sxs-lookup"><span data-stu-id="4f974-123">Use when your agent requires information that is provided in the SMTP **EHLO** command; for example, if your agent accepts or rejects messages based on the identity provided in the **EHLO** command.</span></span>  <br/> |
|[<span data-ttu-id="4f974-124">OnEndOfAuthentication</span><span class="sxs-lookup"><span data-stu-id="4f974-124">OnEndOfAuthentication</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |<span data-ttu-id="4f974-125">Use quando o seu agente exigir informações disponíveis após o servidor remoto concluir o processo de autenticação; por exemplo, para um agente que executa uma ação em uma mensagem com base nas informações de autenticação fornecidas pelo servidor SMTP ou cliente remoto.</span><span class="sxs-lookup"><span data-stu-id="4f974-125">Use when your agent requires information that is available after the remote server completes the authentication process; for example, for an agent that performs an action on a message based on the authentication information provided by the remote SMTP server or client.</span></span>  <br/> |
|[<span data-ttu-id="4f974-126">OnEndOfData</span><span class="sxs-lookup"><span data-stu-id="4f974-126">OnEndOfData</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |<span data-ttu-id="4f974-127">Use quando o seu agente deve executar uma ação com base nos dados que estão disponíveis na mensagem.</span><span class="sxs-lookup"><span data-stu-id="4f974-127">Use when your agent must perform an action based on data that is available in the message.</span></span> <span data-ttu-id="4f974-128">Esse evento não será acionado no serviço de transporte de front-end.</span><span class="sxs-lookup"><span data-stu-id="4f974-128">This event will not fire on the Front End Transport service.</span></span> <span data-ttu-id="4f974-129">Se o seu agente de transporte tiver que usar esse evento, você terá que instalá-lo em um servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4f974-129">If your transport agent has to use this event, you have to install it on a Mailbox server.</span></span>  <br/> |
|[<span data-ttu-id="4f974-130">OnEndOfHeaders</span><span class="sxs-lookup"><span data-stu-id="4f974-130">OnEndOfHeaders</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |<span data-ttu-id="4f974-131">Use quando o seu agente deve executar uma ação com base nas informações disponíveis nos cabeçalhos da mensagem enviada.</span><span class="sxs-lookup"><span data-stu-id="4f974-131">Use when your agent must perform an action based on information that is available in the headers of the submitted message.</span></span>  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a><span data-ttu-id="4f974-132">Criar um agente de transporte SmtpReceiveAgent personalizado</span><span class="sxs-lookup"><span data-stu-id="4f974-132">Creating a custom SmtpReceiveAgent transport agent</span></span>

<span data-ttu-id="4f974-133">O procedimento a seguir descreve como criar um agente de transporte SmtpReceiveAgent personalizado.</span><span class="sxs-lookup"><span data-stu-id="4f974-133">The following procedure describes how to create a custom SmtpReceiveAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="4f974-134">Para criar o agente de transporte</span><span class="sxs-lookup"><span data-stu-id="4f974-134">To create the transport agent</span></span>

1. <span data-ttu-id="4f974-135">Adicione referências aos namespaces.</span><span class="sxs-lookup"><span data-stu-id="4f974-135">Add references to the namespaces.</span></span>
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   <span data-ttu-id="4f974-136">Você pode encontrar esses namespaces no seu servidor Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="4f974-136">You can find these namespaces on your Exchange 2013 server.</span></span> <span data-ttu-id="4f974-137">Ao adicionar uma referência a esses namespaces, você terá acesso aos membros do [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) , bem como outras classes usadas no [Exchange 2013: criar uma amostra de agente de transporte de conversão de corpo](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) .</span><span class="sxs-lookup"><span data-stu-id="4f974-137">When you add a reference to these namespaces, you will have access to the [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) members as well as other classes used in the [Exchange 2013: Build a body conversion transport agent](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) sample.</span></span> 
    
2. <span data-ttu-id="4f974-138">Implemente a classe derivada da classe [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4f974-138">Implement the derived class for the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) class.</span></span> 
    
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

   <span data-ttu-id="4f974-139">Este código criará uma instância da classe derivada e substituirá o método **CreateAgent** para criar uma instância do seu novo agente personalizado.</span><span class="sxs-lookup"><span data-stu-id="4f974-139">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> 
    
3. <span data-ttu-id="4f974-140">Defina seu agente.</span><span class="sxs-lookup"><span data-stu-id="4f974-140">Define your agent.</span></span>
    
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

   <span data-ttu-id="4f974-141">Depois de definir sua classe de agente, você pode adicionar sua funcionalidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="4f974-141">After you define your agent class, you can add your custom functionality.</span></span> <span data-ttu-id="4f974-142">Neste exemplo, o evento [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) é redirecionado para o manipulador de eventos personalizado.</span><span class="sxs-lookup"><span data-stu-id="4f974-142">In this example, the [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) event is redirected to your custom event handler.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="4f974-143">Também consulte</span><span class="sxs-lookup"><span data-stu-id="4f974-143">See also</span></span>

- [<span data-ttu-id="4f974-144">Conceitos de agente de transporte no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="4f974-144">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)    
- [<span data-ttu-id="4f974-145">Referência do agente de transporte para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="4f974-145">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="4f974-146">SmtpReceiveAgentFactory</span><span class="sxs-lookup"><span data-stu-id="4f974-146">SmtpReceiveAgentFactory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [<span data-ttu-id="4f974-147">SmtpReceiveAgent</span><span class="sxs-lookup"><span data-stu-id="4f974-147">SmtpReceiveAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

