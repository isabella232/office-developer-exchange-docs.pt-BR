---
title: Criar um agente de transporte DeliveryAgent para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4af904d7-b315-4849-92b1-66018f76ffdf
description: Descubra como criar um agente de transporte DeliveryAgent personalizado para usar com o Exchange 2013.
ms.openlocfilehash: b349f0b6d835ba3d6195b43e80d1dcd21750bf82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527569"
---
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="b72ed-103">Criar um agente de transporte DeliveryAgent para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b72ed-103">Create a DeliveryAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="b72ed-104">Descubra como criar um agente de transporte DeliveryAgent personalizado para usar com o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="b72ed-104">Find out how to create a custom DeliveryAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="b72ed-105">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="b72ed-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="b72ed-106">As [classes \<Manager\> DeliveryAgentFactory](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) e [DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) são as classes base para agentes de transporte projetados para serem executados no serviço de transporte em um servidor de caixa de correio do Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b72ed-106">The [DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) and [DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) classes are the base classes for transport agents that are designed to run on the Transport service on an Exchange Server 2013 Mailbox server.</span></span> <span data-ttu-id="b72ed-107">Você pode implementar manipuladores no seu agente de transporte do DeliveryAgent para os eventos fornecidos pela classe [DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="b72ed-107">You might implement handlers in your DeliveryAgent transport agent for the events provided by the [DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) class that are listed in the following table.</span></span> 
  
<span data-ttu-id="b72ed-108">**Tabela 1. Eventos de classe DeliveryAgent**</span><span class="sxs-lookup"><span data-stu-id="b72ed-108">**Table 1. DeliveryAgent class events**</span></span>

|<span data-ttu-id="b72ed-109">**Evento**</span><span class="sxs-lookup"><span data-stu-id="b72ed-109">**Event**</span></span>|<span data-ttu-id="b72ed-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b72ed-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b72ed-111">[OnCloseConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx)</span><span class="sxs-lookup"><span data-stu-id="b72ed-111">[OnCloseConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx)</span></span> <br/> |<span data-ttu-id="b72ed-112">Ocorre depois que o último item de email é entregue e a conexão é fechada.</span><span class="sxs-lookup"><span data-stu-id="b72ed-112">Occurs after the last mail item has been delivered and the connection is closed.</span></span>  <br/> |
|<span data-ttu-id="b72ed-113">[OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)</span><span class="sxs-lookup"><span data-stu-id="b72ed-113">[OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)</span></span> <br/> |<span data-ttu-id="b72ed-114">Ocorre quando um item de email está pronto para ser entregue.</span><span class="sxs-lookup"><span data-stu-id="b72ed-114">Occurs when a mail item is ready to be delivered.</span></span>  <br/> |
|<span data-ttu-id="b72ed-115">[OnOpenConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx)</span><span class="sxs-lookup"><span data-stu-id="b72ed-115">[OnOpenConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx)</span></span> <br/> |<span data-ttu-id="b72ed-116">Ocorre quando o agente de entrega é aberto para entrega de email.</span><span class="sxs-lookup"><span data-stu-id="b72ed-116">Occurs when the delivery agent is opened for mail delivery.</span></span>  <br/> |
   
## <a name="creating-a-custom-deliveryagent-transport-agent"></a><span data-ttu-id="b72ed-117">Criar um agente de transporte DeliveryAgent personalizado</span><span class="sxs-lookup"><span data-stu-id="b72ed-117">Creating a custom DeliveryAgent transport agent</span></span>

<span data-ttu-id="b72ed-118">O procedimento a seguir descreve como criar um agente de transporte DeliveryAgent personalizado.</span><span class="sxs-lookup"><span data-stu-id="b72ed-118">The following procedure describes how to create a custom DeliveryAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="b72ed-119">Para criar o agente de transporte</span><span class="sxs-lookup"><span data-stu-id="b72ed-119">To create the transport agent</span></span>

1. <span data-ttu-id="b72ed-120">Adicione referências aos namespaces.</span><span class="sxs-lookup"><span data-stu-id="b72ed-120">Add references to the namespaces.</span></span>
    
   ```cs
        using Microsoft.Exchange.Data.Transport;
        using Microsoft.Exchange.Data.Transport.Delivery;
    
   ```

   <span data-ttu-id="b72ed-121">Você pode encontrar esses namespaces no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="b72ed-121">You can find these namespaces on your Exchange server.</span></span> <span data-ttu-id="b72ed-122">Ao adicionar uma referência a esses namespaces, você terá acesso aos membros do [DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) .</span><span class="sxs-lookup"><span data-stu-id="b72ed-122">By adding a reference to these namespaces, you will have access to the [DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) members.</span></span> 
    
2. <span data-ttu-id="b72ed-123">Implemente a classe derivada da [classe \<Manager\> DeliveryAgentFactory](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) .</span><span class="sxs-lookup"><span data-stu-id="b72ed-123">Implement the derived class for the [DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) class.</span></span> 
    
   ```cs
      public class MyDeliveryAgentFactory : DeliveryAgentFactory<MyDeliveryAgentFactory.MyDeliveryAgentManager>
      {
          static MyDeliveryAgentFactory()
          {
          }
          public override DeliveryAgent CreateAgent(SmtpServer server)
          {
              return new MyDeliveryAgent(server);
          }
          public sealed class MyDeliveryAgentManager : DeliveryAgentManager
          {
              /// <summary>
              /// Gets the supported delivery protocol.
              /// </summary>
              public override string SupportedDeliveryProtocol
              {
                  get { return "MyProtocol"; }
              }
          }
      }
  
   ```

   <span data-ttu-id="b72ed-124">Este código criará uma instância da classe derivada e substituirá o método **CreateAgent** para criar uma instância do seu novo agente personalizado.</span><span class="sxs-lookup"><span data-stu-id="b72ed-124">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> <span data-ttu-id="b72ed-125">Métodos adicionais, como **Close**, também podem ser substituídos nessa classe para executar código personalizado.</span><span class="sxs-lookup"><span data-stu-id="b72ed-125">Additional methods, such as **Close**, can also be overridden in this class to execute custom code.</span></span> <span data-ttu-id="b72ed-126">Uma classe [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) é criada para substituir a propriedade [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) e definir o protocolo que seu agente usará.</span><span class="sxs-lookup"><span data-stu-id="b72ed-126">A [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) class is created to override the [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) property and set the protocol your agent will use.</span></span> 
    
3. <span data-ttu-id="b72ed-127">Defina seu agente.</span><span class="sxs-lookup"><span data-stu-id="b72ed-127">Define your agent.</span></span>
    
   ```cs
      public class MyDeliveryAgent : DeliveryAgent
      {
          public MyDeliveryAgent(SmtpServer server)
          {
              this.OnCloseConnection += CloseConnection;
              this.OnDeliverMailItem += DeliverMailItem;
              this.OnOpenConnection += OpenConnection;
          }
      }
  
   ```

   <span data-ttu-id="b72ed-128">Depois de definir sua classe de agente, você pode adicionar a funcionalidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="b72ed-128">After you define your agent class, you can add you custom functionality.</span></span> <span data-ttu-id="b72ed-129">Neste exemplo, os três eventos, [OnCloseConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx), [OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)e [OnOpenConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx), são redirecionados para seus manipuladores de eventos personalizados.</span><span class="sxs-lookup"><span data-stu-id="b72ed-129">In this example, the three events, [OnCloseConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx), [OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx), and [OnOpenConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx), are redirected to your custom event handlers.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="b72ed-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="b72ed-130">See also</span></span>

- [<span data-ttu-id="b72ed-131">Conceitos de agente de transporte no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b72ed-131">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
- [<span data-ttu-id="b72ed-132">Referência do agente de transporte para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b72ed-132">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)          

 