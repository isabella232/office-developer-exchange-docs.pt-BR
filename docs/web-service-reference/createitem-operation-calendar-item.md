---
title: Operação CreateItem (item de calendário)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: aa4a7c94-f668-4bd2-8079-c855f6ab17e1
description: A operação CreateItem cria itens de calendário no armazenamento do Exchange.
ms.openlocfilehash: c2174dd806b922e640ef7afcab32b98c67c65b41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751601"
---
# <a name="createitem-operation-calendar-item"></a>Operação CreateItem (item de calendário)

A operação CreateItem cria itens de calendário no armazenamento do Exchange.
  
## <a name="remarks"></a>Comentários

A operação CreateItem cria compromissos, reuniões e solicitações de reunião. Se um item de calendário for criado sem participantes, ele será considerado um compromisso. Se os participantes forem especificados, o item de calendário é uma reunião. Quando uma reunião é criada usando a operação CreateItem, solicitações de reunião são enviadas automaticamente para os participantes identificados se o atributo SendMeetingInvitations for definido como enviar as solicitações de reunião.
  
## <a name="createitem-calendar-item-request-example"></a>Exemplo de solicitação de CreateItem (Item de calendário)

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de CreateItem mostra como criar uma reunião com dois participantes necessários. Essa solicitação enviará as solicitações de reunião para os dois participantes.
  
### <a name="code"></a>Código

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                SendMeetingInvitations="SendToAllAndSaveCopy" >
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar"/>
      </SavedItemFolderId>
      <Items>
        <t:CalendarItem xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Planning Meeting</Subject>
          <Body BodyType="Text">Plan the agenda for next week's meeting.</Body>
          <ReminderIsSet>true</ReminderIsSet>
          <ReminderMinutesBeforeStart>60</ReminderMinutesBeforeStart>
          <Start>2006-11-02T14:00:00</Start>
          <End>2006-11-02T15:00:00</End>
          <IsAllDayEvent>false</IsAllDayEvent>
          <LegacyFreeBusyStatus>Busy</LegacyFreeBusyStatus>
          <Location>Conference Room 721</Location>
          <RequiredAttendees>
            <Attendee>
              <Mailbox>
                <EmailAddress>User1@example.com</EmailAddress>
              </Mailbox>
            </Attendee>
            <Attendee>
              <Mailbox>
                <EmailAddress>User2@example.com</EmailAddress>
              </Mailbox>
            </Attendee>
          </RequiredAttendees>
        </t:CalendarItem>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

Para obter um exemplo de como responder a uma solicitação de reunião, consulte o tópico de [operação CreateItem (solicitação de reunião)](createitem-operation-meeting-request.md) . 
  
### <a name="request-elements"></a>Elementos de solicitação

Os seguintes elementos são usados na solicitação:
  
- [CreateItem](createitem.md)
    
- [SavedItemFolderId](saveditemfolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [Itens (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [CalendarItem](calendaritem.md)
    
- [Assunto](subject.md)
    
- [Corpo](body.md)
    
- [ReminderIsSet](reminderisset.md)
    
- [ReminderMinutesBeforeStart](reminderminutesbeforestart.md)
    
- [Start](start.md)
    
- [End](end-ex15websvcsotherref.md)
    
- [IsAllDayEvent](isalldayevent.md)
    
- [LegacyFreeBusyStatus](legacyfreebusystatus.md)
    
- [Location](location.md)
    
- [RequiredAttendees](requiredattendees.md)
    
- [Attendee](attendee.md)
    
- [Caixa de correio](mailbox.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
## <a name="successful-createitem-calendar-item-response"></a>Resposta bem-sucedida CreateItem (Item de calendário)

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida à solicitação de CreateItem.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAAlAFV" ChangeKey="DwAAABYA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

Os atributos de [ItemId](itemid.md) elemento **Id** e **ChangeKey** foram diminuídos para preservar a legibilidade. 
  
### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedida

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
- [CalendarItem](calendaritem.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>Confira também



[Operação CreateItem](createitem-operation.md)

