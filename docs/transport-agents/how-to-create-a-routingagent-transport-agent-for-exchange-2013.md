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
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a>Criar um agente de transporte RoutingAgent para o Exchange 2013

Descubra como criar um agente de transporte RoutingAgent personalizado para usar com o Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013
  
Relacionadas a aplicativos de exemplo e trechos de código:

- [Exchange 2013: Criar um agente de transporte de registro em log de largura de banda](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
As classes [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) e [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) são as classes base para os agentes de transporte que são projetados para executar o serviço de transporte em um servidor de caixa de correio do Exchange Server 2013. A classe [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) fornece os eventos listados na tabela a seguir para o qual você pode implementar manipuladores em seu agente de transporte RoutingAgent. 
  
**Tabela 1. Eventos de classe RoutingAgent**

|**Event**|**Descrição**|
|:-----|:-----|
|[OnCategorizedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |Ocorre depois que o servidor executa a conversão de conteúdo, se for necessário.  <br/> |
|[OnResolvedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |Ocorre após todos os destinatários da mensagem foram resolvidos e antes de roteamento é determinado.  <br/> |
|[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |Ocorre depois que o servidor encaminha a mensagem para o próximo salto e executa a conversão de conteúdo, se necessário. O servidor pode usar mais recursos para processar cada mensagem no evento [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) do evento [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) porque o servidor executar nenhuma conversão de conteúdo necessário e determinar o próximo salto na rota da mensagem antes de executar o código no manipulador de eventos [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) .  <br/> |
|[OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |Ocorre depois que a mensagem for retirada a fila de envio. Use o evento [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) se o agente de transporte RoutingAgent não exigir dados de roteamento, resolvidos destinatários ou conversão de conteúdo.  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a>Criando um agente de transporte RoutingAgent personalizado

O procedimento a seguir descreve como criar um agente de transporte RoutingAgent personalizado. 
  
### <a name="to-create-the-transport-agent"></a>Para criar o agente de transporte

1. Adicione referências para os namespaces.
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   Você pode encontrar esses namespaces em seu servidor Exchange. Adicionando uma referência a esses espaços para nome, você terá acesso aos membros [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) bem como outros classes usadas no [Exchange 2013: criar um agente de transporte do log de largura de banda](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) amostra. 
    
2. Implemente a classe derivada da classe [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) . 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   Este código será instanciar a classe derivada e substitua o método **CreateAgent** para criar uma instância do seu novo agente personalizado. Métodos adicionais, como **Fechar**, também podem ser substituídos nesta classe para executar código personalizado. 
    
3. Defina seu agente.
    
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

   Depois de definir seu classe de agente, você pode adicionar a você uma funcionalidade personalizada. Neste exemplo, os dois eventos [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) e [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)serão redirecionados para seus manipuladores de eventos personalizados. 
    
## <a name="see-also"></a>Confira também

- [Transporte conceitos de agente no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Referência de agente de transporte do Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

