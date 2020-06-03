---
title: Operação GetItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- GetItem
api_type:
- schema
ms.assetid: e3590b8b-c2a7-4dad-a014-6360197b68e4
description: Encontre informações sobre a operação do EWS do GetItem.
localization_priority: Priority
ms.openlocfilehash: 8871dde183974454fc27dbddda489e6b0a70f3aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463325"
---
# <a name="getitem-operation"></a>Operação GetItem

Encontre informações sobre a operação do EWS do **GetItem** . 
  
A operação **GetItem** Obtém itens do repositório do Exchange. 
  
## <a name="using-the-getitem-operation"></a>Usando a operação GetItem

A operação **GetItem** retorna muitas propriedades de item. As propriedades que são retornadas em uma resposta **GetItem** variam de acordo com a forma solicitada, as propriedades adicionais solicitadas e o tipo de item retornado. 
  
Os elementos da [mensagem](message-ex15websvcsotherref.md) representam mensagens de email e todos os outros itens que não são digitados com rigidez pelo esquema dos serviços Web do Exchange (EWS). Itens como IPM. O compartilhamento e o IPM. InfoPath são retornados como elementos de [mensagem](message-ex15websvcsotherref.md) . O Exchange não retorna o elemento de [Item](item.md) base em respostas. 
  
A operação **GetItem** não retorna anexos. Ele retorna metadados sobre um item ou arquivo anexado. Para retornar um anexo, use a [operação GetAttachment](getattachment-operation.md).
  
## <a name="getitem-operation-soap-headers"></a>Cabeçalhos SOAP de operação GetItem

A operação **GetItem** pode usar os cabeçalhos SOAP listados na tabela a seguir. 
  
|Header * * * *|****Element****|****Descrição****|
|:-----|:-----|:-----|
|**DateTimePrecision** <br/> |[DateTimePrecision](datetimeprecision.md) <br/> |Especifica a resolução de valores de data/hora em respostas do servidor, em segundos ou em milissegundos.  <br/> |
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação.  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Identifica o fuso horário a ser usado para todas as respostas do servidor.  <br/> |
   
## <a name="in-this-section"></a>Nesta seção

[Operação GetItem (mensagem de email)](getitem-operation-email-message.md)
  
[Operação GetItem (item de calendário)](getitem-operation-calendar-item.md)
  
[Operação GetItem (tarefa)](getitem-operation-task.md)
  
[Operação GetItem (contato)](getitem-operation-contact.md)
  
## <a name="see-also"></a>Confira também



[Referência do EWS para Exchange](ews-reference-for-exchange.md)

