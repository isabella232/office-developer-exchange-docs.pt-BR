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
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a>Criar um agente de transporte DeliveryAgent para o Exchange 2013

Descubra como criar um agente de transporte DeliveryAgent personalizado para usar com o Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013
  
As [classes \<Manager\> DeliveryAgentFactory](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) e [DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) são as classes base para agentes de transporte projetados para serem executados no serviço de transporte em um servidor de caixa de correio do Exchange Server 2013. Você pode implementar manipuladores no seu agente de transporte do DeliveryAgent para os eventos fornecidos pela classe [DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) listados na tabela a seguir. 
  
**Tabela 1. Eventos de classe DeliveryAgent**

|**Evento**|**Descrição**|
|:-----|:-----|
|[OnCloseConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx) <br/> |Ocorre depois que o último item de email é entregue e a conexão é fechada.  <br/> |
|[OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx) <br/> |Ocorre quando um item de email está pronto para ser entregue.  <br/> |
|[OnOpenConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx) <br/> |Ocorre quando o agente de entrega é aberto para entrega de email.  <br/> |
   
## <a name="creating-a-custom-deliveryagent-transport-agent"></a>Criar um agente de transporte DeliveryAgent personalizado

O procedimento a seguir descreve como criar um agente de transporte DeliveryAgent personalizado. 
  
### <a name="to-create-the-transport-agent"></a>Para criar o agente de transporte

1. Adicione referências aos namespaces.
    
   ```cs
        using Microsoft.Exchange.Data.Transport;
        using Microsoft.Exchange.Data.Transport.Delivery;
    
   ```

   Você pode encontrar esses namespaces no servidor Exchange. Ao adicionar uma referência a esses namespaces, você terá acesso aos membros do [DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) . 
    
2. Implemente a classe derivada da [classe \<Manager\> DeliveryAgentFactory](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) . 
    
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

   Este código criará uma instância da classe derivada e substituirá o método **CreateAgent** para criar uma instância do seu novo agente personalizado. Métodos adicionais, como **Close**, também podem ser substituídos nessa classe para executar código personalizado. Uma classe [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) é criada para substituir a propriedade [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) e definir o protocolo que seu agente usará. 
    
3. Defina seu agente.
    
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

   Depois de definir sua classe de agente, você pode adicionar a funcionalidade personalizada. Neste exemplo, os três eventos, [OnCloseConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx), [OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)e [OnOpenConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx), são redirecionados para seus manipuladores de eventos personalizados. 
    
## <a name="see-also"></a>Confira também

- [Conceitos de agente de transporte no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)
- [Referência do agente de transporte para o Exchange 2013](transport-agent-reference-for-exchange-2013.md)          

 