---
title: Operação GetItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: e3590b8b-c2a7-4dad-a014-6360197b68e4
description: Encontre informações sobre o EWS GetItem operação.
ms.openlocfilehash: 9b63032b2eaa3bf26027a42e38bfa06bedcbac86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752544"
---
# <a name="getitem-operation"></a>Operação GetItem

Encontre informações sobre a operação de EWS **GetItem** . 
  
A operação **GetItem** obtém os itens do armazenamento do Exchange. 
  
## <a name="using-the-getitem-operation"></a>Usando a operação GetItem

A operação de **GetItem** retorna propriedades de item de muitos. As propriedades que são retornadas em uma resposta **GetItem** variam com base na forma solicitada, propriedades adicionais solicitadas e o tipo de item os dados retornados. 
  
Elementos de [mensagem](message-ex15websvcsotherref.md) representam as mensagens de email e outros itens que não são fortemente tipados pelo esquema dos serviços Web do Exchange (EWS). Itens como IPM. Compartilhamento e IPM.InfoPath são retornados como elementos da [mensagem](message-ex15websvcsotherref.md) . Exchange não retorna o elemento do [Item](item.md) base nas respostas. 
  
A operação **GetItem** não retorna anexos. Ela retornar metadados sobre um item anexado ou o arquivo. Para retornar um anexo, use a [operação GetAttachment](getattachment-operation.md).
  
## <a name="getitem-operation-soap-headers"></a>Cabeçalhos SOAP GetItem operação

A operação **GetItem** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir. 
  
|Cabeçalho * * *|****Element****|****Descrição****|
|:-----|:-----|:-----|
|**DateTimePrecision** <br/> |[DateTimePrecision](datetimeprecision.md) <br/> |Especifica a resolução dos valores de data/hora nas respostas do servidor, em segundos ou em milissegundos.  <br/> |
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação.  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Identifica o fuso horário a ser usado para todas as respostas do servidor.  <br/> |
   
## <a name="in-this-section"></a>Nesta Seção

[Operação GetItem (mensagem de email)](getitem-operation-email-message.md)
  
[Operação GetItem (item de calendário)](getitem-operation-calendar-item.md)
  
[Operação GetItem (tarefa)](getitem-operation-task.md)
  
[Operação GetItem (contato)](getitem-operation-contact.md)
  
## <a name="see-also"></a>Confira também



[Referência do EWS para Exchange](ews-reference-for-exchange.md)

