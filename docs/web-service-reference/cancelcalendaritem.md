---
title: CancelCalendarItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CancelCalendarItem
api_type:
- schema
ms.assetid: a2046402-a176-44d5-b4b3-adb696581935
description: O elemento CancelCalendarItem representa o objeto de resposta usado para cancelar uma reunião.
ms.openlocfilehash: a0f4c094bba2d78cf1222eefbef7604cf8c33d4e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516010"
---
# <a name="cancelcalendaritem"></a>CancelCalendarItem

O **elemento CancelCalendarItem** representa o objeto de resposta usado para cancelar uma reunião. 
  
```xml
<CancelCalendarItem>
   <Subject/>
   <Body/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ReferenceItemId/>
   <NewBodyContent/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
</CancelCalendarItem>
```

 **CancelCalendarItemType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Assunto](subject.md) <br/> |Representa a propriedade subject de Exchange de armazenamento.  <br/> |
|[Body](body.md) <br/> |Não usado por **CancelCalendarItem**. Use a [propriedade NewBodyContent](newbodycontent.md) para definir o conteúdo do corpo.  <br/> |
|[ToRecipients](torecipients.md) <br/> |Contém um conjunto de destinatários de um item. Esses são os principais destinatários de um item.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Representa uma coleção de destinatários que receberão uma cópia da mensagem.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Representa uma coleção de destinatários para receber uma cópia de carbono cego (Cc) de um email.  <br/> |
|[IsReadReceiptRequested](isreadreceiptrequested.md) <br/> |Indica se o remetente de um item solicita um recibo de leitura.  <br/> |
|[IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |Indica se o remetente de um item solicita um recibo de entrega.  <br/> |
|[ReferenceItemId](referenceitemid.md) <br/> |Identifica o item ao qual o objeto de resposta se refere.  <br/> |
|[NewBodyContent](newbodycontent.md) <br/> |Representa o novo conteúdo de corpo de uma mensagem.  <br/> |
|[ReceivedBy](receivedby.md) <br/> |Identifica o representante em um cenário de acesso de representante. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |Identifica a entidade principal em um cenário de acesso de representante. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> | Descreve todos os itens adjacentes a um horário de reunião.<br/><br/> Veja a seguir algumas das expressões XPath para este elemento:<br/><br/>`/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> | Descreve todos os itens que conflitam com um horário de reunião.<br/><br/>Veja a seguir algumas das expressões XPath para este elemento:<br/><br/>`/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contém uma coleção de todos os objetos de resposta associados a um item no Exchange store.  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contém uma matriz de itens a ser criado na pasta identificada pelo [elemento ParentFolderId (TargetFolderIdType).](parentfolderid-targetfolderidtype.md)  <br/> |
   
## <a name="remarks"></a>Comentários

O **elemento CancelCalendarItem** só é exibido pelo organizador. Ela só se aplica ao item de calendário do organizador. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

