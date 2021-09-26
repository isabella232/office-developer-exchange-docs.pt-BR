---
title: Exemplos de código do agente de transporte para Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 626345ec-918f-4d91-932f-e6ce92553ccb
description: Encontre informações sobre os agentes de transporte de exemplo disponíveis para Exchange 2013.
ms.openlocfilehash: 56334f661947cffceaf18eb257feeb6504a71ecb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545704"
---
# <a name="transport-agent-code-samples-for-exchange-2013"></a>Exemplos de código do agente de transporte para Exchange 2013

Encontre informações sobre os agentes de transporte de exemplo disponíveis para Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013
  
Você pode usar as APIs incluídas no Exchange Server 2013 para desenvolver agentes que estendem a funcionalidade de transporte. Este artigo fornece informações sobre os agentes de exemplo disponíveis para ajudá-lo a aprender a estender o comportamento de transporte programaticamente. Os agentes de exemplo incluem o código-fonte de cada componente. 
  
A tabela a seguir lista os agentes de exemplo para Exchange 2013.
  
**Tabela 1. Exemplos de agente de transporte**

|**Nome do exemplo**|**Descrição**|
|:-----|:-----|
|[Exchange 2013: criar um agente de transporte antivírus](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-6e544269) <br/> |Esse agente responde aos eventos [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) e [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) e envia a mensagem de entrada para um servidor fora do processo que examina a mensagem de forma assíncrona e retorna uma versão modificada.  <br/> |
|[Exchange 2013: criar um agente de transporte de log de largura de banda](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) <br/> |Esse agente responde aos eventos [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) e [OnRoutedMessage,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) captura o uso de largura de banda para destinatários especificados e registra as informações de uso da largura de banda em um arquivo de texto.  <br/> |
|[Exchange 2013: criar um agente de transporte de conversão de corpo](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) <br/> |Esse agente filtra scripts de mensagens de email determinando o formato da mensagem de entrada e decidindo se a filtragem deve ocorrer. Se a filtragem for necessária, o conteúdo será convertido em HTML, filtrado e convertido novamente no formato de origem.  <br/> |
|[Exchange 2013: criar um agente de transporte de log SMTP](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-fc23dc33) <br/> |Esse agente responde ao [evento OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) e registra a mensagem de forma assíncrona em um arquivo no disco rígido local.  <br/> |
|[Exchange 2013: criar um agente de transporte que bloqueia os envios temporariamente](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-52a767d8) <br/> |Esse agente responde aos eventos [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) e [OnRcptCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnRcptCommand.aspx) e determina se o remetente da mensagem enviou mensagens anteriormente para o serviço de Transporte de Front-End. Se o remetente não tiver enviado uma mensagem anteriormente para o serviço de Transporte de Front-End, o remetente será adicionado a uma lista de remetentes e a mensagem será rejeitada com uma resposta que diz ao cliente para tentar novamente mais tarde (também conhecido como graylisting). Se o remetente estiver na lista de remetentes anteriores, o agente não rejeitará a mensagem.  <br/> |
|[Exchange 2013: criar um agente de transporte de log do servidor de Caixa de Correio](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-fc8632e5) <br/> |Esse agente responde ao evento de pipeline de transporte [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) e registra síncronamente a mensagem em um arquivo no disco rígido local.  <br/> |
|[Exchange 2013: criar um agente de transporte de header X](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-32f62f5a) <br/> |Esse agente responde ao evento [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) e lê e modifica os headers X em mensagens.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Conceitos de agente de transporte no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Referência do agente de transporte Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [Criar um agente de transporte RoutingAgent para Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)   
- [Criar um agente de transporte SmtpReceiveAgent para Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)    
- [Criar um agente de transporte DeliveryAgent para Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    

