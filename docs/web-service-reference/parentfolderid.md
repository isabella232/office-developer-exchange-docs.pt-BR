---
title: ParentFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 258f4b1f-367e-4c7d-9c29-eb775a2398c7
description: O elemento ParentFolderId representa o identificador da pasta pai que contém o item ou a pasta.
ms.openlocfilehash: 3f60e8adb62fbf464a58af4169fbcd83910877cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824687"
---
# <a name="parentfolderid"></a>ParentFolderId

O elemento **ParentFolderId** representa o identificador da pasta pai que contém o item ou a pasta. 
  
```XML
<ParentFolderId Id="" ChangeKey=""/>
```

**FolderIdType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**ID de** <br/> |Contém uma cadeia de caracteres que identifica uma pasta no repositório do Exchange. Este atributo é necessário.  <br/> |
|**ChangeKey** <br/> |Contém uma cadeia de caracteres que identifica uma versão de uma pasta que é identificada pelo atributo **Id** . Este atributo é opcional. Use este atributo para certificar-se de que a versão correta de uma pasta é usada.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Representa uma pasta de calendário em uma caixa de correio.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário em uma caixa de correio.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato em uma caixa de correio.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Representa uma pasta de contatos em uma caixa de correio.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Representa um evento no qual uma pasta ou um item é copiada.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Representa um evento no qual uma pasta ou um item é criada.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Representa um evento no qual uma pasta ou um item é excluída.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição particular em uma caixa de correio.  <br/> |
|[Folder](folder.md) <br/> |Representa uma pasta em uma caixa de correio.  <br/> |
|[1.1](item.md) <br/> |Representa um item genérico do Exchange.  <br/> |
|[Item (UploadItemType)](item-uploaditemtype.md) <br/> |Representa um único item para carregar em uma caixa de correio.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa o cancelamento da reunião em uma caixa de correio.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma mensagem de reunião em uma caixa de correio.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião em uma caixa de correio.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião em uma caixa de correio.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email em uma caixa de correio.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Representa um evento no qual um item ou pasta é modificada.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Representa um evento na qual um item ou pasta é movida de uma pasta pai para outra pasta pai.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Representa um evento que é disparado por um novo item de email em uma caixa de correio.  <br/> |
|[AcceptItem](acceptitem.md) <br/> |Representa uma resposta de aceitar a uma solicitação de reunião.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Representa um provisório responde a uma solicitação de reunião.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Representa uma resposta recusar a uma solicitação de reunião.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Remove um item de armazenamento do Exchange.  <br/> |
|[Task](task.md) <br/> |Representa um item de tarefa em uma caixa de correio.  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Contém uma resposta para o criador de um item no armazenamento do Exchange.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Contém uma resposta a todos os destinatários identificados de um item no armazenamento do Exchange.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Contém um item de armazenamento do Exchange para encaminhar para destinatários.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Representa o objeto de resposta é usado para cancelar uma reunião.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Representa uma pasta de tarefa em uma caixa de correio.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Representa uma pasta de pesquisa em uma caixa de correio.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

