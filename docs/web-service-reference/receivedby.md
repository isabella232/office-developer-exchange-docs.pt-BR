---
title: ReceivedBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReceivedBy
api_type:
- schema
ms.assetid: ac84c9c5-d2fe-4b6f-bf4d-0444131d835b
description: O elemento ReceivedBy identifica o representante em um cenário de acesso de representante.
ms.openlocfilehash: 7cee996c15e81f77d71f42e052b14b1d21772ba1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468247"
---
# <a name="receivedby"></a>ReceivedBy

O elemento **ReceivedBy** identifica o representante em um cenário de acesso de representante. 
  
```xml
<ReceivedBy>
   <Mailbox/>
</ReceivedBy>
```

 **SingleRecipientType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixa de Correio](mailbox.md) <br/> |Identifica um objeto de serviço de diretório do Active Directory habilitado para email.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
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
   
## <a name="remarks"></a>Comentários

O elemento **ReceivedRepresenting** é usado em conjunto com os elementos from e **ReceivedBy** nos cenários **de** acesso de representante. A tabela a seguir lista as entidades que esses elementos representam em um cenário de acesso de representante. 
  
**Elementos em um cenário de acesso de representante**

|**Elemento**|**Entidade que o elemento representa**|
|:-----|:-----|
|[De](from.md) <br/> |Terceiros  <br/> |
|[ReceivedBy](receivedby.md) <br/> |Delegar  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |Principal  <br/> |
   
Em um cenário de acesso de representante, se um terceiros envia uma solicitação de reunião para uma entidade que tenha um representante, o representante verá uma nova solicitação de reunião. Esses elementos permitem que os representantes diferenciem mensagens que são enviadas diretamente a elas e mensagens que são enviadas a elas devido a uma regra de encaminhamento de representante.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

