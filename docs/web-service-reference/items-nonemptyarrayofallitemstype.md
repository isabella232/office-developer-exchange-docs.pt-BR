---
title: Items (NonEmptyArrayOfAllItemsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Items
api_type:
- schema
ms.assetid: d61ef1cc-ddfc-480a-9625-7b436cb33ae0
description: O elemento Items contém um conjunto de itens a ser criado.
ms.openlocfilehash: a511fa9e81cdfb4d5c84705edb0d37f75eb76049
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524991"
---
# <a name="items-nonemptyarrayofallitemstype"></a>Items (NonEmptyArrayOfAllItemsType)

O **elemento Items** contém um conjunto de itens a ser criado. 
  
```XML
<Items>
   <Item/>
   <Message/>
   <CalendarItem/>
   <Contact/>
   <DistributionList/>
   <MeetingMessage/>
   <MeetingRequest/>
   <MeetingResponse/>
   <MeetingCancellation/>
   <Task/>
   <ReplyToItem/>
   <ForwardItem/>
   <ReplyAllToItem/>
   <AcceptItem/>
   <TentativelyAcceptItem/>
   <DeclineItem/>
   <CancelCalendarItem/>
   <RemoveItem/>
   <PostReplyItem/>
   <SuppressReadReceipt/>
   <AcceptSharingInvitation/>
</Items>
```

 **NonEmptyArrayOfAllItemsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Item](item.md) <br/> |Representa um item no Exchange store.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem Exchange email.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
|[Contato](contact.md) <br/> |Representa um Exchange de contato.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma mensagem de reunião no Exchange store.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no Exchange store.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no Exchange store.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no Exchange store.  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Contém uma resposta ao remetente de um item no Exchange store.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Contém um Exchange de armazenamento para encaminhar aos destinatários.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Contém uma resposta ao remetente e a todos os destinatários identificados de um item no Exchange store.  <br/> |
|[AcceptItem](acceptitem.md) <br/> |Representa uma resposta Aceitar a uma solicitação de reunião.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Representa uma resposta provisória a uma solicitação de reunião.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Representa uma resposta Declinar a uma solicitação de reunião.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Representa o objeto de resposta usado para cancelar uma reunião.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Representa um objeto de resposta usado para remover um item de reunião quando uma mensagem MeetingCancellation é recebida.  <br/> |
|[PostReplyItem](postreplyitem.md) <br/> |Contém uma resposta a um item de postagem.  <br/> |
|[SuppressReadReceipt](suppressreadreceipt.md) <br/> |Usado para suprimir recibos de leitura.  <br/> |
|[AcceptSharingInvitation](acceptsharinginvitation.md) <br/> |Usado para aceitar um convite que permite o acesso aos dados de calendário ou contatos de outro usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateItem](createitem.md) <br/> |Define a solicitação para criar um item no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  `/CreateItem` <br/> |
|[ConversationNode](conversationnode.md) <br/> |Identifica um único nó em uma conversa.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação CreateFolder](createfolder-operation.md)
  
[Operação CreateItem](createitem-operation.md)


[Criando Pastas (Exchange Web Services)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

