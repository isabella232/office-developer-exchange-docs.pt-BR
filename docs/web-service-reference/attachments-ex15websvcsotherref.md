---
title: Anexos
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attachments
api_type:
- schema
ms.assetid: b470e614-34bb-44f0-8790-7ddbdcbbd29d
description: O elemento Attachments contém os itens ou arquivos anexados a um item no repositório do Exchange.
ms.openlocfilehash: a9f79cd79f19e6226703c99c53c91efed600f495
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461531"
---
# <a name="attachments"></a>Attachments

O elemento **Attachments** contém os itens ou arquivos anexados a um item no repositório do Exchange. 
  
```xml
<Attachments>
   <ItemAttachment/>
   <FileAttachment/>
</Attachments>
```

 **ArrayOfAttachmentsType** e **NonEmptyArrayOfAttachmentsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemAttachment](itemattachment.md) <br/> |Representa um item do Exchange anexado a outro item do Exchange.  <br/> |
|[FileAttachment](fileattachment.md) <br/> |Representa um arquivo anexado a um item no repositório do Exchange.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateAttachment](createattachment.md) <br/> |Define uma solicitação para criar um anexo a um item no repositório do Exchange.<br/><br/> A seguir está a expressão XPath para este elemento:`/CreateAttachment` <br/> |
|[AcceptItem](acceptitem.md) <br/> | Representa uma resposta de aceitação para uma solicitação de reunião.<br/><br/>A seguir estão algumas das expressões XPath para este elemento:<ul><li>`/CreateItem/Items`</li><li>`/MeetingRequest/ConflictingMeetings` </li><li>`/SetItemField/CalendarItem/ConflictingMeetings`</li><li>`/AppendToItemField/CalendarItem/ConflictingMeetings`</li><li>`/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings`</li><li>`/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li><li>`/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li></ul> |
|[DeclineItem](declineitem.md) <br/> |Representa uma resposta de recusa a uma solicitação de reunião.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Representa uma resposta provisória a uma solicitação de reunião.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Remove um item do repositório do Exchange.  <br/> |
|[Item](item.md) <br/> |Representa um item genérico do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no repositório do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no repositório do Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no repositório do Exchange.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Exchange.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no repositório do Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato do Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação CreateAttachment.  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação GetAttachment.  <br/> |
   
## <a name="remarks"></a>Comentários

Os elementos **Attachments** têm os mesmos elementos filho, mas são baseados em tipos diferentes: **ArrayOfAttachmentsType** e **NonEmptyArrayOfAttachmentsType**. Os tipos definem se um elemento filho é obrigatório. O **ArrayOfAttachmentsType** é usado apenas na mensagem de resposta. Também é importante observar que esses elementos ocorrem nos namespaces de messages e Types. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

