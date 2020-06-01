---
title: Exemplos de código de agente de transporte para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 626345ec-918f-4d91-932f-e6ce92553ccb
description: Encontre informações sobre os agentes de transporte de amostra disponíveis para o Exchange 2013.
ms.openlocfilehash: c14a4e34102b55014cc6507e375929c186f5f6e9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461797"
---
# <a name="transport-agent-code-samples-for-exchange-2013"></a>Exemplos de código de agente de transporte para o Exchange 2013

Encontre informações sobre os agentes de transporte de amostra disponíveis para o Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013
  
Você pode usar as APIs incluídas no Exchange Server 2013 para desenvolver agentes que estendem a funcionalidade de transporte. Este artigo fornece informações sobre os agentes de amostra que estão disponíveis para ajudá-lo a aprender a estender o comportamento de transporte programaticamente. Os agentes de amostra incluem o código-fonte de cada componente. 
  
A tabela a seguir lista os agentes de amostra do Exchange 2013.
  
**Tabela 1. Amostras de agente de transporte**

|**Nome da amostra**|**Descrição**|
|:-----|:-----|
|[Exchange 2013: criar um agente de transporte antivírus](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-6e544269) <br/> |Este agente responde aos eventos [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) e [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) e envia a mensagem de entrada para um servidor fora de processo que examina de forma assíncrona a mensagem e retorna uma versão modificada.  <br/> |
|[Exchange 2013: criar um agente de transporte de log de largura de banda](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) <br/> |Este agente responde aos eventos [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) e [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) , captura o uso da largura de banda para destinatários específicos e registra as informações de uso da largura de banda em um arquivo de texto.  <br/> |
|[Exchange 2013: criar um agente de transporte de conversão de corpo](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) <br/> |Este agente filtra os scripts fora das mensagens de email determinando o formato da mensagem de entrada e decidindo se a filtragem deve ocorrer. Se a filtragem for necessária, o conteúdo será convertido em HTML, filtrado e convertido novamente no formato de origem.  <br/> |
|[Exchange 2013: criar um agente de transporte de log SMTP](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-fc23dc33) <br/> |Este agente responde ao evento [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) e registra a mensagem de forma assíncrona em um arquivo no disco rígido local.  <br/> |
|[Exchange 2013: criar um agente de transporte que bloqueie os remetentes temporariamente](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-52a767d8) <br/> |Este agente responde aos eventos [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) e [OnRcptCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnRcptCommand.aspx) e determina se o remetente da mensagem enviou mensagens anteriormente para o serviço de transporte de front-end. Se o remetente não tiver enviado uma mensagem para o serviço de transporte de front-end, o remetente será adicionado a uma lista de remetentes, e a mensagem será rejeitada com uma resposta que informa ao cliente para tentar novamente mais tarde (também conhecido como graylisting). Se o remetente estiver na lista de remetentes anteriores, o agente não rejeitará a mensagem.  <br/> |
|[Exchange 2013: criar um agente de transporte de log de servidor de caixa de correio](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-fc8632e5) <br/> |Este agente responde ao evento de pipeline de transporte do [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) e registra a mensagem de forma síncrona em um arquivo no disco rígido local.  <br/> |
|[Exchange 2013: criar um agente de transporte de cabeçalho X](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-32f62f5a) <br/> |Este agente responde ao evento [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) e ler e modificar cabeçalhos X nas mensagens.  <br/> |
   
## <a name="see-also"></a>Também consulte

- [Conceitos de agente de transporte no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Referência do agente de transporte para o Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [Criar um agente de transporte RoutingAgent para o Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)   
- [Criar um agente de transporte SmtpReceiveAgent para o Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)    
- [Criar um agente de transporte DeliveryAgent para o Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    

