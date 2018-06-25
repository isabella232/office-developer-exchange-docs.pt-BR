---
title: Transporte amostras de código do agente do Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 626345ec-918f-4d91-932f-e6ce92553ccb
description: Encontre informações sobre os agentes de transporte de amostra que estão disponíveis para o Exchange 2013.
ms.openlocfilehash: 122a3351748fa6ffd823a51ce65ffb913332cb2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751026"
---
# <a name="transport-agent-code-samples-for-exchange-2013"></a>Transporte amostras de código do agente do Exchange 2013

Encontre informações sobre os agentes de transporte de amostra que estão disponíveis para o Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013
  
Você pode usar as APIs que estão incluídas no Exchange Server 2013 para desenvolver agentes que estendem a funcionalidade de transporte. Este artigo fornece informações sobre os agentes de amostra que estão disponíveis para ajudá-lo a aprender como estender o comportamento de transporte programaticamente. Os agentes de amostra incluem o código-fonte para cada componente. 
  
A tabela a seguir lista os operadores de amostra para o Exchange 2013.
  
**Tabela 1. Exemplos de agente de transporte**

|**Nome da amostra**|**Descrição**|
|:-----|:-----|
|[Exchange 2013: Criar um agente de transporte de antivírus](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-6e544269) <br/> |Este operador responde aos eventos [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) e [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) e envia a mensagem de entrada para um servidor fora do processo que examina a mensagem de forma assíncrona e retorna uma versão modificada.  <br/> |
|[Exchange 2013: Criar um agente de transporte de registro em log de largura de banda](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) <br/> |Este operador responde a eventos [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) e [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) , captura o uso de largura de banda para destinatários especificados e registra as informações de uso de largura de banda em um arquivo de texto.  <br/> |
|[Exchange 2013: Criar um agente de transporte de conversão de corpo](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) <br/> |Este agente filtra scripts sem emails determinando o formato das mensagens de entrada e decidir se a filtragem deverá ocorrer. Se houver necessidade de filtragem, o conteúdo é convertido em HTML, filtrado e depois convertido volta para o formato de fonte.  <br/> |
|[Exchange 2013: Criar um agente de transporte de registro em log do SMTP](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-fc23dc33) <br/> |Este operador responde ao evento [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) e registra assincronamente a mensagem para um arquivo no disco rígido local.  <br/> |
|[Exchange 2013: Criar um agente de transporte que bloqueia remetentes temporariamente](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-52a767d8) <br/> |Este operador responde aos eventos [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) e [OnRcptCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnRcptCommand.aspx) e determina se o remetente da mensagem tem anteriormente mensagens enviadas para o serviço Front End Transport. Se o remetente anteriormente não enviou uma mensagem para o serviço Front End Transport, o remetente é adicionado a uma lista de remetentes confiáveis e a mensagem será rejeitada com uma resposta que informa o cliente tentar novamente mais tarde (também conhecido como graylisting). Se o remetente está na lista de remetentes anteriores, o agente não rejeitar a mensagem.  <br/> |
|[Exchange 2013: Criar um agente de transporte de log do servidor de caixa de correio](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-fc8632e5) <br/> |Este agente responde ao evento do pipeline de transporte [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) e registra de maneira síncrona a mensagem para um arquivo no disco rígido local.  <br/> |
|[Exchange 2013: Criar um agente de transporte de cabeçalho X](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-32f62f5a) <br/> |Este agente responde ao evento [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) e ler e modificar cabeçalhos X nas mensagens.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Transporte conceitos de agente no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Referência de agente de transporte do Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [Criar um agente de transporte RoutingAgent para o Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)   
- [Criar um agente de transporte SmtpReceiveAgent para o Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)    
- [Criar um agente de transporte DeliveryAgent para o Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    

