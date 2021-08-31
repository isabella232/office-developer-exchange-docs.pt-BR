---
title: ResponseObjects
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseObjects
api_type:
- schema
ms.assetid: ad29e064-3f3d-4b7b-aa4c-9ec27326381d
description: O elemento ResponseObjects contém uma coleção de todos os objetos de resposta associados a um item no Exchange store.
ms.openlocfilehash: 9f80fd9703dcd7d9293a3a51eccb6cf2b6903064
ms.sourcegitcommit: 357b882a02e37b380a23b8a45b15f9c006a40b02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58764578"
---
# <a name="responseobjects"></a>ResponseObjects

O **elemento ResponseObjects** contém uma coleção de todos os objetos de resposta associados a um item no Exchange store. 
  
```XML
<ResponseObjects>
   <AcceptItem/>
   <TentativelyAcceptItem/>
   <DeclineItem/>
   <ProposeNewTime>
   <ReplyToItem/>
   <ForwardItem/>
   <ReplyAllToItem/>
   <CancelCalendarItem/>
   <RemoveItem/>
   <PostReplyItem/>
   <SuppressReadReceipt/>
   <AcceptSharingInvitation/>
</ResponseObjects>
```

 **NonEmptyArrayOfResponseObjectsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |Representa uma resposta Aceitar a uma solicitação de reunião.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Representa uma resposta provisória a uma solicitação de reunião.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Representa uma resposta Declinar a uma solicitação de reunião.  <br/> |
|[ProposeNewTime](proposenewtime.md) <br/> |Indica que o participante da reunião pode propor um novo horário de reunião. Esse elemento foi introduzido no Microsoft Exchange Server 2013 Service Pack 1 (SP1).  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Contém uma resposta ao criador de um item no Exchange store.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Contém um Exchange de armazenamento para encaminhar aos destinatários.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Contém uma resposta a todos os destinatários identificados de um item no Exchange store.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Representa o objeto de resposta usado para cancelar uma reunião.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Remove um item do Exchange store.  <br/> |
|[PostReplyItem](postreplyitem.md) <br/> |Contém uma resposta a um item de postagem. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[SuppressReadReceipt](suppressreadreceipt.md) <br/> |Usado para suprimir solicitações de recebimento de leitura.  <br/> |
|[AcceptSharingInvitation](acceptsharinginvitation.md) <br/> |Usado para aceitar um convite que permite o acesso aos dados de calendário ou contatos de outro usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
|[Contato](contact.md) <br/> |Representa um Exchange de contato.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Item](item.md) <br/> |Representa um item no Exchange store.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no Exchange store.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no Exchange store.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no Exchange store.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Representa uma Exchange de email.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Remove um item do Exchange store.  <br/> |
|[Task](task.md) <br/> |Representa uma tarefa no Exchange store.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

