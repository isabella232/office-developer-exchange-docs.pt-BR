---
title: InternetMessageId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- InternetMessageId
api_type:
- schema
ms.assetid: a5a9563f-e761-4658-9957-0e13566f6a35
description: O elemento InternetMessageId representa o identificador de mensagem da Internet de um item.
ms.openlocfilehash: a357b33f32ae622609df7a3acfe3549d7171bce2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514575"
---
# <a name="internetmessageid"></a>InternetMessageId

O **elemento InternetMessageId** representa o identificador de mensagem da Internet de um item. 
  
```xml
<InternetMessageId/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RemoveItem](removeitem.md) <br/> |Remove um item do Exchange store.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma Exchange de email.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no Exchange store.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no Exchange store.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no Exchange store.  <br/> |
|[AcceptItem](acceptitem.md) <br/> |Representa uma resposta Aceitar a uma solicitação de reunião.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Representa uma resposta provisória a uma solicitação de reunião.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Representa uma resposta Declinar a uma solicitação de reunião.  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Contém uma resposta ao criador de um item no Exchange store.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Contém uma resposta a todos os destinatários identificados de um item no Exchange store.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Contém um Exchange de armazenamento para encaminhar aos destinatários.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Representa o objeto de resposta usado para cancelar uma reunião.  <br/> |
|[Item de postagem](postitem.md) <br/> |Representa um item post no Exchange store. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o identificador de mensagem da Internet.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

