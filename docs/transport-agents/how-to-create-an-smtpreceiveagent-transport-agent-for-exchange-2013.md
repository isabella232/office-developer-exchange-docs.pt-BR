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
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a>Criar um agente de transporte SmtpReceiveAgent para o Exchange 2013

Descubra como criar um agente de transporte SmtpReceiveAgent personalizado para usar com o Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013
  
Relacionadas a aplicativos de exemplo e trechos de código:

- [Exchange 2013: Criar um agente de transporte de conversão de corpo](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
As classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) e [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) permitem estender o comportamento do serviço Front End Transport em um servidor de acesso para cliente ou o serviço de transporte em um servidor de caixa de correio. Você pode usar essas classes para implementar os agentes de transporte que foram projetados para responder às mensagens como eles entram em sua organização. 
  
As classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) e [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) incluem os eventos listados na tabela a seguir. 
  
**Tabela 1. Eventos de classe SmtpReceiveAgent**

|**Event**|**Descrição**|
|:-----|:-----|
|[OnAuthCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |Quando seu agente exige informações que são fornecidas apenas no comando SMTP **AUTH** , como um operador que aceita ou rejeita tenta enviar uma mensagem com base no tipo de método de autenticação usado para uso.  <br/> |
|[OnConnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |Use quando seu agente exige informações que são fornecidas apenas quando uma conexão é aberta por meio de SMTP para o serviço de Front End Transport, como um operador que está executando uma ação com base no endereço ou no domínio do servidor SMTP remoto.  <br/> |
|[OnDataCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |Use este evento quando seu agente requer as informações fornecidas no comando SMTP **dados** .  <br/> |
|[OnDisconnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |Use quando seu agente exige informações que está disponíveis no momento da desconexão, como a data e hora atuais, para executar cálculos de tempo.  <br/> |
|[OnEhloCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |Uso quando seu agente requer as informações fornecidas no comando SMTP **EHLO** ; Por exemplo, se seu operador a aceita ou rejeita mensagens com base na identidade fornecida no comando **EHLO** .  <br/> |
|[OnEndOfAuthentication](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |Use quando seu agente exige informações que está disponíveis depois que o servidor remoto conclui o processo de autenticação; Por exemplo, para um operador que está executando uma ação em uma mensagem com base nas informações de autenticação fornecidas pelo cliente ou servidor SMTP remoto.  <br/> |
|[OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |Use quando seu agente deve executar uma ação com base nos dados que está disponíveis na mensagem. Esse evento não será acionado no serviço Front End Transport. Se o agente de transporte precisa usar esse evento, você precisa instalá-lo em um servidor de caixa de correio.  <br/> |
|[OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |Use quando seu agente deve executar uma ação com base nas informações que está disponíveis nos cabeçalhos da mensagem enviada.  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a>Criando um agente de transporte SmtpReceiveAgent personalizado

O procedimento a seguir descreve como criar um agente de transporte SmtpReceiveAgent personalizado. 
  
### <a name="to-create-the-transport-agent"></a>Para criar o agente de transporte

1. Adicione referências para os namespaces.
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   Você pode encontrar esses espaços para nome no seu servidor Exchange 2013. Quando você adiciona uma referência a esses espaços para nome, você terá acesso aos membros [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) bem como outros classes usadas no [Exchange 2013: criar um agente de transporte de conversão de corpo](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) amostra. 
    
2. Implemente a classe derivada da classe [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) . 
    
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

   Este código será instanciar a classe derivada e substitua o método **CreateAgent** para criar uma instância do seu novo agente personalizado. 
    
3. Defina seu agente.
    
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

   Depois de definir seu classe de agente, você pode adicionar sua funcionalidade personalizada. Neste exemplo, o evento [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) é redirecionado para o manipulador de eventos personalizados. 
    
## <a name="see-also"></a>Confira também

- [Transporte conceitos de agente no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Referência de agente de transporte do Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

