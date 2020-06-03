---
title: ConversationIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationIndex
api_type:
- schema
ms.assetid: fdf47e22-8d93-4ae4-883b-0c9f07f48724
description: O elemento ConversationIndex contém uma ID binária que representa o thread ao qual esta mensagem pertence.
ms.openlocfilehash: 03874c6462be6380e34c999bc2354c376a462882
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461433"
---
# <a name="conversationindex"></a>ConversationIndex

O elemento **ConversationIndex** contém uma ID binária que representa o thread ao qual esta mensagem pertence. 
  
```xml
<ConversationIndex/>
```

 **Base64Binary**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RemoveItem](removeitem.md) <br/> |Remove um item do repositório do Exchange.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no repositório do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no repositório do Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no repositório do Exchange.  <br/> |
|[AcceptItem](acceptitem.md) <br/> |Representa uma resposta de aceitação para uma solicitação de reunião.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Representa uma resposta provisoriamente aceita a uma solicitação de reunião.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Representa uma resposta de recusa a uma solicitação de reunião.  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Contém uma resposta para o criador de um item no repositório do Exchange.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Contém uma resposta a todos os destinatários identificados de um item no repositório do Exchange.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Contém um item de repositório do Exchange para encaminhar aos destinatários.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Representa o objeto Response que é usado para cancelar uma reunião.  <br/> |
|[Item de postagem](postitem.md) <br/> |Representa um item de postagem no repositório do Exchange. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa um identificador binário no formato **Base64Binary** . 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do servidor Exchange que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

