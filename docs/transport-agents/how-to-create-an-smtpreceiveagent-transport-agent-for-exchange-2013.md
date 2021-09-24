---
title: Criar um agente de transporte SmtpReceiveAgent para Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: cdc7c462-74a7-49d6-95b2-155d783840e9
description: Saiba como criar um agente de transporte SmtpReceiveAgent personalizado a ser usado com Exchange 2013.
ms.openlocfilehash: a441f93113798c10421e9073e266c28fd87bca8d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513028"
---
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a>Criar um agente de transporte SmtpReceiveAgent para Exchange 2013

Saiba como criar um agente de transporte SmtpReceiveAgent personalizado a ser usado com Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013
  
Trechos de código relacionados e aplicativos de exemplo:

- [Exchange 2013: criar um agente de transporte de conversão de corpo](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
As classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) e [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) permitem estender o comportamento do serviço de Transporte de Front-End em um Servidor de Acesso para Cliente ou o serviço de Transporte em um servidor de Caixa de Correio. Você pode usar essas classes para implementar agentes de transporte projetados para responder a mensagens à medida que elas chegam à sua organização. 
  
As [classes SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) e [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) incluem os eventos listados na tabela a seguir. 
  
**Tabela 1. Eventos de classe SmtpReceiveAgent**

|**Evento**|**Descrição**|
|:-----|:-----|
|[OnAuthCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |Use quando seu agente exigir informações fornecidas apenas no comando **AUTH** SMTP, como um agente que aceita ou rejeita tentativas de entregar uma mensagem com base no tipo de método de autenticação usado.  <br/> |
|[OnConnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |Use quando seu agente exigir informações fornecidas somente quando uma conexão é aberta via SMTP para o serviço de Transporte de Front-End, como um agente que executa uma ação com base no endereço ou domínio do servidor SMTP remoto.  <br/> |
|[OnDataCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |Use esse evento quando seu agente exigir informações  fornecidas no comando DATA SMTP.  <br/> |
|[OnDisconnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |Use quando seu agente exigir informações que estão disponíveis no momento da desconexão, como a data e hora atuais, para realizar cálculos de hora.  <br/> |
|[OnEhloCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |Use quando seu agente exigir informações fornecidas no comando **EHLO** SMTP; por exemplo, se seu agente aceitar ou rejeitar mensagens com base na identidade fornecida no **comando EHLO.**  <br/> |
|[OnEndOfAuthentication](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |Use quando seu agente exigir informações disponíveis depois que o servidor remoto concluir o processo de autenticação; por exemplo, para um agente que executa uma ação em uma mensagem com base nas informações de autenticação fornecidas pelo servidor ou cliente SMTP remoto.  <br/> |
|[OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |Use quando seu agente deve executar uma ação com base nos dados disponíveis na mensagem. Esse evento não disparará no serviço de Transporte de Front-End. Se o agente de transporte tiver que usar esse evento, você terá que instalá-lo em um servidor de Caixa de Correio.  <br/> |
|[OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |Use quando seu agente deve executar uma ação com base nas informações disponíveis nos headers da mensagem enviada.  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a>Criando um agente de transporte SmtpReceiveAgent personalizado

O procedimento a seguir descreve como criar um agente de transporte SmtpReceiveAgent personalizado. 
  
### <a name="to-create-the-transport-agent"></a>Para criar o agente de transporte

1. Adicione referências aos namespaces.
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   Você pode encontrar esses namespaces no servidor Exchange 2013. Ao adicionar uma referência a esses namespaces, você terá acesso aos membros [SmtpReceiveAgent,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) bem como a outras classes usadas no [Exchange 2013: Criar](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) um exemplo de agente de transporte de conversão de corpo. 
    
2. Implemente a classe derivada para a [classe SmtpReceiveAgentFactory.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) 
    
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

   Esse código instanciará a classe derivada e substituirá o **método CreateAgent** para criar uma instância do seu novo agente personalizado. 
    
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

   Depois de definir sua classe de agente, você pode adicionar sua funcionalidade personalizada. Neste exemplo, o [evento OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) é redirecionado para o manipulador de eventos personalizado. 
    
## <a name="see-also"></a>Confira também

- [Conceitos de agente de transporte no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Referência do agente de transporte Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

