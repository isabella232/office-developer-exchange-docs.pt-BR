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
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a>Criar um agente de transporte SmtpReceiveAgent para o Exchange 2013

Descubra como criar um agente de transporte SmtpReceiveAgent personalizado para usar com o Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013
  
Trechos de código relacionados e aplicativos de exemplo:

- [Exchange 2013: criar um agente de transporte de conversão de corpo](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
As classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) e [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) permitem que você estenda o comportamento do serviço de transporte de front-end em um servidor de acesso para cliente ou no serviço de transporte em um servidor de caixa de correio. Você pode usar essas classes para implementar agentes de transporte projetados para responder às mensagens à medida que elas entram na sua organização. 
  
As classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) e [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) incluem os eventos listados na tabela a seguir. 
  
**Tabela 1. Eventos de classe SmtpReceiveAgent**

|**Evento**|**Descrição**|
|:-----|:-----|
|[OnAuthCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |Use quando o seu agente exigir informações fornecidas apenas no comando de **autenticação** SMTP, como um agente que aceita ou rejeita tentativas de entrega de mensagens com base no tipo de método de autenticação usado.  <br/> |
|[OnConnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |Use quando o seu agente exigir informações fornecidas somente quando uma conexão for aberta via SMTP para o serviço de transporte de front-end, como um agente que executa uma ação com base no endereço ou domínio do servidor SMTP remoto.  <br/> |
|[OnDataCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |Use este evento quando o seu agente exigir informações fornecidas no comando de **dados** SMTP.  <br/> |
|[OnDisconnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |Use quando o seu agente exigir informações disponíveis no momento da desconexão, como a data e hora atuais, para executar cálculos de tempo.  <br/> |
|[OnEhloCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |Use quando o seu agente exigir informações fornecidas no comando **EHLO** do SMTP; por exemplo, se o seu agente aceitar ou rejeitar mensagens com base na identidade fornecida no comando **EHLO** .  <br/> |
|[OnEndOfAuthentication](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |Use quando o seu agente exigir informações disponíveis após o servidor remoto concluir o processo de autenticação; por exemplo, para um agente que executa uma ação em uma mensagem com base nas informações de autenticação fornecidas pelo servidor SMTP ou cliente remoto.  <br/> |
|[OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |Use quando o seu agente deve executar uma ação com base nos dados que estão disponíveis na mensagem. Esse evento não será acionado no serviço de transporte de front-end. Se o seu agente de transporte tiver que usar esse evento, você terá que instalá-lo em um servidor de caixa de correio.  <br/> |
|[OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |Use quando o seu agente deve executar uma ação com base nas informações disponíveis nos cabeçalhos da mensagem enviada.  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a>Criar um agente de transporte SmtpReceiveAgent personalizado

O procedimento a seguir descreve como criar um agente de transporte SmtpReceiveAgent personalizado. 
  
### <a name="to-create-the-transport-agent"></a>Para criar o agente de transporte

1. Adicione referências aos namespaces.
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   Você pode encontrar esses namespaces no seu servidor Exchange 2013. Ao adicionar uma referência a esses namespaces, você terá acesso aos membros do [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) , bem como outras classes usadas no [Exchange 2013: criar uma amostra de agente de transporte de conversão de corpo](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) . 
    
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

   Este código criará uma instância da classe derivada e substituirá o método **CreateAgent** para criar uma instância do seu novo agente personalizado. 
    
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

   Depois de definir sua classe de agente, você pode adicionar sua funcionalidade personalizada. Neste exemplo, o evento [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) é redirecionado para o manipulador de eventos personalizado. 
    
## <a name="see-also"></a>Também consulte

- [Conceitos de agente de transporte no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Referência do agente de transporte para o Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

