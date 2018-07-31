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
ms.openlocfilehash: bc36c7b5e0fb8006c5927d423d7767dcc7382ce0
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353305"
---
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a>Criar um agente de transporte DeliveryAgent para o Exchange 2013

Descubra como criar um agente de transporte DeliveryAgent personalizado para usar com o Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013
  
O [DeliveryAgentFactory\<Manager\> ](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx) e classes de [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) são as classes base para os agentes de transporte que são projetados para executar o serviço de transporte em um servidor de caixa de correio do Exchange Server 2013. Você pode implementar manipuladores em seu agente de transporte DeliveryAgent para os eventos fornecido pela classe [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) que estão listados na tabela a seguir. 
  
**Tabela 1. Eventos de classe DeliveryAgent**

|**Event**|**Descrição**|
|:-----|:-----|
|[OnCloseConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx) <br/> |Ocorre após o último item de email foi entregue e a conexão é fechada.  <br/> |
|[OnDeliverMailItem](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx) <br/> |Ocorre quando um item de email está pronto para ser entregue.  <br/> |
|[OnOpenConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx) <br/> |Ocorre quando o agente de entrega é aberto para entrega de email.  <br/> |
   
## <a name="creating-a-custom-deliveryagent-transport-agent"></a>Criando um agente de transporte DeliveryAgent personalizado

O procedimento a seguir descreve como criar um agente de transporte DeliveryAgent personalizado. 
  
### <a name="to-create-the-transport-agent"></a>Para criar o agente de transporte

1. Adicione referências para os namespaces.
    
   ```cs
        using Microsoft.Exchange.Data.Transport;
        using Microsoft.Exchange.Data.Transport.Delivery;
    
   ```

   Você pode encontrar esses namespaces em seu servidor Exchange. Adicionando uma referência a esses espaços para nome, você terá acesso aos membros [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) . 
    
2. Implementar a classe derivada para o [DeliveryAgentFactory\<Manager\> ](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx) classe. 
    
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

   Este código será instanciar a classe derivada e substitua o método **CreateAgent** para criar uma instância do seu novo agente personalizado. Métodos adicionais, como **Fechar**, também podem ser substituídos nesta classe para executar código personalizado. Uma classe de [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) é criada para substituir a propriedade [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) e defina o protocolo que seu agente usará. 
    
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

   Depois de definir seu classe de agente, você pode adicionar a você uma funcionalidade personalizada. Neste exemplo, os três eventos, [OnCloseConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx), [OnDeliverMailItem](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)e [OnOpenConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx), serão redirecionadas para seus manipuladores de eventos personalizados. 
    
## <a name="see-also"></a>Confira também

- [Transporte conceitos de agente no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)
- [Referência de agente de transporte do Exchange 2013](transport-agent-reference-for-exchange-2013.md)          

 