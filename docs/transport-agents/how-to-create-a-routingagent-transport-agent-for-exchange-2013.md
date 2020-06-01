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
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a>Criar um agente de transporte RoutingAgent para o Exchange 2013

Descubra como criar um agente de transporte RoutingAgent personalizado para usar com o Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013
  
Trechos de código relacionados e aplicativos de exemplo:

- [Exchange 2013: criar um agente de transporte de log de largura de banda](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
As classes [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) e [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) são as classes base para agentes de transporte projetados para serem executados no serviço de transporte em um servidor de caixa de correio do Exchange Server 2013. A classe [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) fornece os eventos listados na tabela a seguir para o qual você pode implementar manipuladores no seu agente de transporte do RoutingAgent. 
  
**Tabela 1. Eventos de classe RoutingAgent**

|**Evento**|**Descrição**|
|:-----|:-----|
|[OnCategorizedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |Ocorre após o servidor executar a conversão de conteúdo, se for necessário.  <br/> |
|[OnResolvedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |Ocorre depois que todos os destinatários da mensagem foram resolvidos e antes de o roteamento ser determinado.  <br/> |
|[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |Ocorre após o servidor direcionar a mensagem para o próximo salto e realizar a conversão de conteúdo, se necessário. O servidor pode usar mais recursos para processar cada mensagem no evento [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) do que o evento [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) , pois o servidor executará qualquer conversão de conteúdo necessária e determinará o próximo salto na rota da mensagem antes de executar o código no manipulador de eventos [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) .  <br/> |
|[OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |Ocorre depois que a mensagem é retirada da fila de envio. Use o evento [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) se o seu agente de transporte do RoutingAgent não exigir conversão de conteúdo, destinatários resolvidos ou dados de roteamento.  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a>Criar um agente de transporte RoutingAgent personalizado

O procedimento a seguir descreve como criar um agente de transporte RoutingAgent personalizado. 
  
### <a name="to-create-the-transport-agent"></a>Para criar o agente de transporte

1. Adicione referências aos namespaces.
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   Você pode encontrar esses namespaces no servidor Exchange. Ao adicionar uma referência a esses namespaces, você terá acesso aos membros do [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) , bem como outras classes usadas no [Exchange 2013: criar um exemplo de agente de transporte de log de largura de banda](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) . 
    
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

   Este código criará uma instância da classe derivada e substituirá o método **CreateAgent** para criar uma instância do seu novo agente personalizado. Métodos adicionais, como **Close**, também podem ser substituídos nessa classe para executar código personalizado. 
    
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

   Depois de definir sua classe de agente, você pode adicionar a funcionalidade personalizada. Neste exemplo, os dois eventos [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) e [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)são redirecionados para seus manipuladores de eventos personalizados. 
    
## <a name="see-also"></a>Também consulte

- [Conceitos de agente de transporte no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Referência do agente de transporte para o Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

