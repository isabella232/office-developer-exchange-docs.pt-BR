---
title: ConversationTopic
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationTopic
api_type:
- schema
ms.assetid: 46cacf42-4039-4c8a-9b20-c42cdd9f2760
description: O elemento ConversationTopic representa o tópico de conversa.
ms.openlocfilehash: 3f4f30acad2f5dd7d6fea25dda3ea4e39ddc2492
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457596"
---
# <a name="conversationtopic"></a>ConversationTopic

O elemento **ConversationTopic** representa o tópico de conversa. 
  
```xml
<ConversationTopic/>
```

 **String**
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
|[Message](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no repositório do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no repositório do Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no repositório do Exchange.  <br/> |
|[AcceptItem](acceptitem.md) <br/> |Representa uma resposta de aceitação para uma solicitação de reunião.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Representa uma resposta provisória a uma solicitação de reunião.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Representa uma resposta de recusa a uma solicitação de reunião.  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Contém uma resposta para o criador de um item no repositório do Exchange.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Contém uma resposta a todos os destinatários identificados de um item no repositório do Exchange.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Contém um item de repositório do Exchange para encaminhar aos destinatários.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Representa o objeto Response que é usado para cancelar uma reunião.  <br/> |
|[Item de postagem](postitem.md) <br/> |Representa um item de postagem no repositório do Exchange. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[Conversa (Conversatype)](conversation-conversationtype.md) <br/> |Representa uma única conversa.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o tópico do segmento de conversa.
  
## <a name="remarks"></a>Comentários

O tópico de conversa geralmente é o assunto da primeira mensagem de email em um thread.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindConversation](findconversation-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

