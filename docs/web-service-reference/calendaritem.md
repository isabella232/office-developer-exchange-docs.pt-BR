---
title: CalendarItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarItem
api_type:
- schema
ms.assetid: b0c1fd27-b6da-46e5-88b8-88f00c71ba80
description: O elemento CalendarItem representa um item Exchange calendário.
ms.openlocfilehash: b8493a54e42df2789be04b2a426c6aff414ec6f2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518859"
---
# <a name="calendaritem"></a>CalendarItem

O **elemento CalendarItem** representa um item Exchange calendário. 
  
```XML
<CalendarItem>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <Start/>
   <End/>
   <OriginalStart/>
   <IsAllDayEvent/>
   <LegacyFreeBusyStatus/>
   <Location/>
   <When/>
   <IsMeeting/>
   <IsCancelled/>
   <IsRecurring/>
   <MeetingRequestWasSent/>
   <IsResponseRequested/>
   <CalendarItemType/>
   <MyResponseType/>
   <Organizer/>
   <RequiredAttendees/>
   <OptionalAttendees/>
   <Resources/>
   <ConflictingMeetingCount/>
   <AdjacentMeetingCount/>
   <ConflictingMeetings/>
   <AdjacentMeetings/>
   <Duration/>
   <TimeZone/>
   <AppointmentReplyTime/>
   <AppointmentSequenceNumber/>
   <AppointmentState/>
   <Recurrence/>
   <FirstOccurrence/>
   <LastOccurrence/>
   <ModifiedOccurrences/>
   <DeletedOccurrences/>
   <MeetingTimeZone/>
   <StartTimeZone/>
   <EndTimeZone/>
   <ConferenceType/>
   <AllowNewTimeProposal/>
   <IsOnlineMeeting/>
   <MeetingWorkspaceUrl/>
   <NetShowUrl/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</CalendarItem>
```

 **CalendarItemType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Contém o fluxo nativo de Extensões de Email da Internet (MIME) de um objeto representado no formato base64Binary.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador exclusivo e a chave de alteração de um item no Exchange store.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai que contém o item ou pasta.  <br/> |
|[ItemClass](itemclass.md) <br/> |Representa a classe de mensagem de um item.  <br/> |
|[Assunto](subject.md) <br/> |Representa o assunto para Exchange itens de armazenamento e objetos de resposta.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Indica o nível de sensibilidade de um item.  <br/> |
|[Body](body.md) <br/> |Representa o conteúdo real do corpo de uma mensagem.  <br/> |
|[Anexos](attachments-ex15websvcsotherref.md) <br/> |Contém os itens ou arquivos anexados a um item no Exchange store.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Representa a data e a hora em que um item em uma caixa de correio foi recebido.  <br/> |
|[Tamanho](size.md) <br/> |Representa o tamanho em bytes de um item. Essa propriedade é somente leitura.  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |Representa uma coleção de cadeias de caracteres que identificam as categorias às quais um item na caixa de correio pertence.  <br/> |
|[Importance](importance.md) <br/> |Descreve a importância de um item.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Representa o identificador do item ao qual este item é uma resposta.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Indica se um item foi enviado para a pasta padrão da Caixa de Saída.  <br/> |
|[IsDraft](isdraft.md) <br/> |Indica se um item ainda não foi enviado.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Indica se um usuário enviou um item para ele ou para si mesmo.  <br/> |
|[IsResend](isresend.md) <br/> |Indica se o item foi enviado anteriormente.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Indica se o item foi modificado.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Representa a coleção de todos os headers de mensagens da Internet que estão contidos em um item em uma caixa de correio.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Representa a data e a hora em que um item em uma caixa de correio foi enviado.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Representa a data e a hora em que um determinado item na caixa de correio foi criado.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contém uma coleção de todos os objetos de resposta associados a um item no Exchange store.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Representa a data e a hora em que o evento ocorre. Isso é usado pelo [elemento ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Indica se um lembrete foi definido para um item no Exchange store.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Representa o número de minutos antes de um evento quando um lembrete é exibido.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Representa a cadeia de caracteres de exibição usada para o conteúdo da linha Cc. Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatário Cc.  <br/> |
|[DisplayTo](displayto.md) <br/> |Representa a cadeia de caracteres de exibição usada para o conteúdo da linha Para. Esta é a cadeia de caracteres concatenada de todos os nomes de exibição do destinatário Para.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Representa uma propriedade definida como **true se** um item tiver pelo menos um anexo visível. Essa propriedade é somente leitura.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifica propriedades estendidas em pastas e itens.  <br/> |
|[Cultura](culture.md) <br/> |Representa a cultura de um determinado item em uma caixa de correio.  <br/> |
|[UID](uid.md) <br/> |Identifica um item de calendário.  <br/> |
|[RecurrenceId](recurrenceid.md) <br/> |Usado para identificar uma instância específica de um item de calendário recorrente.  <br/> |
|[DateTimeStamp](datetimestamp.md) <br/> |Indica a data e a hora em que uma instância de um objeto iCalendar foi criada.  <br/> |
|[Start](start.md) <br/> |Representa o início de um item de calendário. Esse elemento só se aplica a uma única ocorrência de um item de calendário.  <br/> |
|[End ](end-ex15websvcsotherref.md) <br/> |Representa o fim de uma duração. Esse elemento só se aplica a uma única ocorrência de um item de calendário.  <br/> |
|[OriginalStart](originalstart.md) <br/> |Representa a hora de início original de um item de calendário.  <br/> |
|[IsAllDayEvent](isalldayevent.md) <br/> |Indica se um item de calendário ou uma solicitação de reunião representa um evento de todo o dia.  <br/> |
|[LegacyFreeBusyStatus](legacyfreebusystatus.md) <br/> |Representa o status de ocupado/livre do item de calendário.  <br/> |
|[Location](location.md) <br/> |Representa o local de uma reunião ou compromisso.  <br/> |
|[When](when.md) <br/> |Fornece informações sobre quando um item de calendário ocorre.  <br/> |
|[IsMeeting](ismeeting.md) <br/> |Indica se o item de calendário é uma reunião ou compromisso.  <br/> |
|[IsCancelled](iscancelled.md) <br/> |Indica se um compromisso ou reunião foi cancelado.  <br/> |
|[IsRecurring](isrecurring.md) <br/> |Indica se um item de calendário faz parte de um item recorrente. Esse elemento é somente leitura.  <br/> |
|[MeetingRequestWasSent](meetingrequestwassent.md) <br/> |Indica se uma solicitação de reunião foi enviada aos participantes solicitados.  <br/> |
|[IsResponseRequested](isresponserequested.md) <br/> |Indica se uma resposta a um item é necessária.  <br/> |
|[CalendarItemType](calendaritemtype.md) <br/> |Representa o tipo de ocorrência de um item de calendário.  <br/> |
|[MyResponseType](myresponsetype.md) <br/> |Contém o status ou a resposta a um item de calendário.  <br/> |
|[Organizador](organizer.md) <br/> |Representa o organizador de uma reunião.  <br/> |
|[RequiredAttendees](requiredattendees.md) <br/> |Representa os participantes que são necessários para participar de uma reunião.  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |Representa participantes que não são necessários para participar de uma reunião.  <br/> |
|[Recursos](resources.md) <br/> |Representa um recurso agendado para uma reunião.  <br/> |
|[ConflictingMeetingCount](conflictingmeetingcount.md) <br/> |Representa o número de reuniões que conflitam com o item de calendário.  <br/> |
|[AdjacentMeetingCount](adjacentmeetingcount.md) <br/> |Representa o número total de itens de calendário adjacentes a um horário de reunião.  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Identifica todos os itens que conflitam com um horário de reunião.  <br/> |
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Descreve todos os itens de calendário adjacentes a um horário de reunião.  <br/> |
|[Duration (Items)](duration-items.md) <br/> |Representa a duração de um item de calendário.  <br/> |
|[TimeZone (Item)](timezone-item.md) <br/> |Fornece uma descrição de texto de um fuso horário.  <br/> |
|[AppointmentReplyTime](appointmentreplytime.md) <br/> |Representa a data e a hora em que um participante respondeu a uma solicitação de reunião.  <br/> |
|[AppointmentSequenceNumber](appointmentsequencenumber.md) <br/> |Especifica o número da sequência de uma versão de um compromisso.  <br/> |
|[AppointmentState](appointmentstate.md) <br/> |Especifica o status do compromisso.  <br/> |
|[Recurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Contém o padrão de recorrência para itens de calendário e solicitações de reunião.  <br/> Esse elemento será válido se [CalendarItemType](calendaritemtype.md) tiver o valor RecurringMaster.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Representa a primeira ocorrência de um item de calendário recorrente.  <br/> Esse elemento será válido se [CalendarItemType](calendaritemtype.md) tiver o valor RecurringMaster.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Representa a última ocorrência de um item de calendário recorrente.  <br/> Esse elemento será válido se [CalendarItemType](calendaritemtype.md) tiver o valor RecurringMaster.  <br/> |
|[ModifiedOccurrences](modifiedoccurrences.md) <br/> |Contém uma matriz de ocorrências de item de calendário recorrentes que foram modificadas para que eles diferem do item mestre de recorrência.  <br/> Esse elemento será válido se [CalendarItemType](calendaritemtype.md) tiver o valor RecurringMaster.  <br/> |
|[DeletedOccurrences](deletedoccurrences.md) <br/> |Contém uma matriz de ocorrências excluídas de um item de calendário recorrente.  <br/> Esse elemento será válido se [CalendarItemType](calendaritemtype.md) tiver o valor RecurringMaster.  <br/> |
|[MeetingTimeZone](meetingtimezone.md) <br/> |Representa o fuso horário do local onde a reunião está hospedada.  <br/> |
|[StartTimeZone](starttimezone.md) <br/> |Representa o fuso horário de início do item de calendário.  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |Representa o fuso horário final do item de calendário.  <br/> |
|[ConferenceType](conferencetype.md) <br/> |Descreve o tipo de conferência que é realizada com um item de calendário.  <br/> |
|[AllowNewTimeProposal](allownewtimeproposal.md) <br/> |Indica se um novo horário de reunião pode ser proposto para uma reunião por um participante.  <br/> |
|[IsOnlineMeeting](isonlinemeeting.md) <br/> |Indica se a reunião está online.  <br/> |
|[MeetingWorkspaceUrl](meetingworkspaceurl.md) <br/> |Contém a URL do espaço de trabalho de reunião que está vinculado pelo item de calendário.  <br/> |
|[NetShowUrl](netshowurl.md) <br/> |Especifica a URL de uma reunião online do Microsoft NetShow.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contém os direitos do cliente com base nas configurações de permissão do item ou pasta. Esse elemento é somente leitura.  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |Contém o nome de exibição do último usuário para modificar um item.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Indica quando um item foi modificado pela última vez.  <br/> |
|[IsAssociated](isassociated.md) <br/> |Indica se o item está associado a uma pasta.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Representa uma URL para concatenar ao ponto de extremidade Microsoft Office Outlook Web App para ler um item em Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Representa uma URL para concatenar ao ponto de extremidade Microsoft Office Outlook Web App para editar um item no Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Contém o identificador de um item ou conversa.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Representa um fragmento HTML ou texto simples que representa o corpo exclusivo dessa conversa.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Descreve todos os itens de calendário adjacentes a um horário de reunião.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifica dados a ser anexados a uma única propriedade de um item ou pasta durante uma [operação UpdateItem.](updateitem-operation.md)  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Identifica todos os itens que conflitam com um horário de reunião.  <br/> |
|[Create (ItemSync)](create-itemsync.md) <br/> |Identifica uma única pasta a ser criado no armazenamento do cliente local.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Representa um Exchange que está anexado a outro Exchange item.  <br/> |
|[Itens](items.md) <br/> |Contém uma matriz de itens.  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contém uma matriz de itens a ser criado na pasta identificada pelo elemento [ParentFolderId (TargetFolderIdType).](parentfolderid-targetfolderidtype.md)  <br/> |
|[SetItemField](setitemfield.md) <br/> |Representa uma atualização para uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |Identifica um único item a ser atualizado no armazenamento cliente local.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

Quando um único item de calendário é atualizado para se tornar um item de calendário mestre recorrente, o [elemento MeetingTimeZone](meetingtimezone.md) deve ser especificado para preservar o fuso horário original do item de calendário. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
  
[Referência do EWS para Exchange](ews-reference-for-exchange.md)

