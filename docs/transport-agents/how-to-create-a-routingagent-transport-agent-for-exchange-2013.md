---
title: Criar um agente de transporte RoutingAgent para Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3f0e745f-9289-4f31-8877-926692a8c133
description: Saiba como criar um agente de transporte RoutingAgent personalizado a ser usado com Exchange 2013.
ms.openlocfilehash: 70dbfc3c25e18195bb4b42fd3e750da11b0423d6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534171"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a>Criar um agente de transporte RoutingAgent para Exchange 2013

Saiba como criar um agente de transporte RoutingAgent personalizado a ser usado com Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013
  
Trechos de código relacionados e aplicativos de exemplo:

- [Exchange 2013: criar um agente de transporte de log de largura de banda](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
As [classes RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) e [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) são as classes base para agentes de transporte que foram projetadas para ser executados no serviço de transporte em um servidor de Caixa de Correio Exchange Server 2013. A [classe RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) fornece os eventos listados na tabela a seguir para a qual você pode implementar manipuladores em seu agente de transporte RoutingAgent. 
  
**Tabela 1. Eventos de classe RoutingAgent**

|**Evento**|**Descrição**|
|:-----|:-----|
|[OnCategorizedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |Ocorre depois que o servidor executa a conversão de conteúdo, se necessário.  <br/> |
|[OnResolvedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |Ocorre depois que todos os destinatários da mensagem foram resolvidos e antes que o roteamento seja determinado.  <br/> |
|[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |Ocorre depois que o servidor encaminha a mensagem para o próximo salto e executa a conversão de conteúdo, se necessário. O servidor pode usar mais recursos para processar cada mensagem no evento [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) do que o [evento OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) porque o servidor executará qualquer conversão de conteúdo necessária e determinará o próximo salto na rota da mensagem antes de executar o código no manipulador de eventos [OnRoutedMessage.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)  <br/> |
|[OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |Ocorre depois que a mensagem é retirada da fila de envio. Use o [evento OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) se seu agente de transporte RoutingAgent não exigir conversão de conteúdo, destinatários resolvidos ou dados de roteamento.  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a>Criando um agente de transporte RoutingAgent personalizado

O procedimento a seguir descreve como criar um agente de transporte RoutingAgent personalizado. 
  
### <a name="to-create-the-transport-agent"></a>Para criar o agente de transporte

1. Adicione referências aos namespaces.
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   Você pode encontrar esses namespaces em seu Exchange servidor. Adicionando uma referência a esses namespaces, você terá acesso aos membros [RoutingAgent,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) bem como a outras classes usadas no [Exchange 2013: Criar](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) um exemplo de agente de transporte de log de largura de banda. 
    
2. Implemente a classe derivada para a [classe RoutingAgentFactory.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   Esse código instanciará a classe derivada e substituirá o **método CreateAgent** para criar uma instância do seu novo agente personalizado. Métodos adicionais, como **Close**, também podem ser substituídos nesta classe para executar código personalizado. 
    
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

   Depois de definir sua classe de agente, você pode adicionar sua funcionalidade personalizada. Neste exemplo, os dois eventos [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) e [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)são redirecionados para seus manipuladores de eventos personalizados. 
    
## <a name="see-also"></a>Confira também

- [Conceitos de agente de transporte no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Referência do agente de transporte Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

