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
# <a name="createitem-operation-calendar-item"></a><span data-ttu-id="62f71-103">Operação CreateItem (item de calendário)</span><span class="sxs-lookup"><span data-stu-id="62f71-103">CreateItem operation (calendar item)</span></span>

<span data-ttu-id="62f71-104">A operação CreateItem cria itens de calendário no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="62f71-104">The CreateItem operation creates calendar items in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="62f71-105">Comentários</span><span class="sxs-lookup"><span data-stu-id="62f71-105">Remarks</span></span>

<span data-ttu-id="62f71-106">A operação CreateItem cria compromissos, reuniões e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="62f71-106">The CreateItem operation creates appointments, meetings, and meeting requests.</span></span> <span data-ttu-id="62f71-107">Se um item de calendário for criado sem participantes, ele será considerado um compromisso.</span><span class="sxs-lookup"><span data-stu-id="62f71-107">If a calendar item is created without attendees, it is considered an appointment.</span></span> <span data-ttu-id="62f71-108">Se os participantes forem especificados, o item de calendário é uma reunião.</span><span class="sxs-lookup"><span data-stu-id="62f71-108">If attendees are specified, the calendar item is a meeting.</span></span> <span data-ttu-id="62f71-109">Quando uma reunião é criada usando a operação CreateItem, solicitações de reunião são enviadas automaticamente para os participantes identificados se o atributo SendMeetingInvitations for definido como enviar as solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="62f71-109">When a meeting is created by using the CreateItem operation, meeting requests are automatically sent to the identified attendees if the SendMeetingInvitations attribute is set to send the meeting requests.</span></span>
  
## <a name="createitem-calendar-item-request-example"></a><span data-ttu-id="62f71-110">Exemplo de solicitação de CreateItem (Item de calendário)</span><span class="sxs-lookup"><span data-stu-id="62f71-110">CreateItem (Calendar Item) request example</span></span>

### <a name="description"></a><span data-ttu-id="62f71-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="62f71-111">Description</span></span>

<span data-ttu-id="62f71-112">O exemplo a seguir de uma solicitação de CreateItem mostra como criar uma reunião com dois participantes necessários.</span><span class="sxs-lookup"><span data-stu-id="62f71-112">The following example of a CreateItem request shows how to create a meeting with two required attendees.</span></span> <span data-ttu-id="62f71-113">Essa solicitação enviará as solicitações de reunião para os dois participantes.</span><span class="sxs-lookup"><span data-stu-id="62f71-113">This request will send the meeting requests to the two attendees.</span></span>
  
### <a name="code"></a><span data-ttu-id="62f71-114">Código</span><span class="sxs-lookup"><span data-stu-id="62f71-114">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="62f71-115">Comments</span><span class="sxs-lookup"><span data-stu-id="62f71-115">Comments</span></span>

<span data-ttu-id="62f71-116">Para obter um exemplo de como responder a uma solicitação de reunião, consulte o tópico de [operação CreateItem (solicitação de reunião)](createitem-operation-meeting-request.md) .</span><span class="sxs-lookup"><span data-stu-id="62f71-116">For an example of how to respond to a meeting request, see the [CreateItem operation (meeting request)](createitem-operation-meeting-request.md) topic.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="62f71-117">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62f71-117">Request elements</span></span>

<span data-ttu-id="62f71-118">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="62f71-118">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="62f71-119">CreateItem</span><span class="sxs-lookup"><span data-stu-id="62f71-119">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="62f71-120">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="62f71-120">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="62f71-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="62f71-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="62f71-122">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="62f71-122">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="62f71-123">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="62f71-123">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="62f71-124">Assunto</span><span class="sxs-lookup"><span data-stu-id="62f71-124">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="62f71-125">Corpo</span><span class="sxs-lookup"><span data-stu-id="62f71-125">Body</span></span>](body.md)
    
- [<span data-ttu-id="62f71-126">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="62f71-126">ReminderIsSet</span></span>](reminderisset.md)
    
- [<span data-ttu-id="62f71-127">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="62f71-127">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md)
    
- [<span data-ttu-id="62f71-128">Start</span><span class="sxs-lookup"><span data-stu-id="62f71-128">Start</span></span>](start.md)
    
- [<span data-ttu-id="62f71-129">End</span><span class="sxs-lookup"><span data-stu-id="62f71-129">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="62f71-130">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="62f71-130">IsAllDayEvent</span></span>](isalldayevent.md)
    
- [<span data-ttu-id="62f71-131">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="62f71-131">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md)
    
- [<span data-ttu-id="62f71-132">Location</span><span class="sxs-lookup"><span data-stu-id="62f71-132">Location</span></span>](location.md)
    
- [<span data-ttu-id="62f71-133">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="62f71-133">RequiredAttendees</span></span>](requiredattendees.md)
    
- [<span data-ttu-id="62f71-134">Attendee</span><span class="sxs-lookup"><span data-stu-id="62f71-134">Attendee</span></span>](attendee.md)
    
- [<span data-ttu-id="62f71-135">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="62f71-135">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="62f71-136">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="62f71-136">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
## <a name="successful-createitem-calendar-item-response"></a><span data-ttu-id="62f71-137">Resposta bem-sucedida CreateItem (Item de calendário)</span><span class="sxs-lookup"><span data-stu-id="62f71-137">Successful CreateItem (Calendar Item) Response</span></span>

### <a name="description"></a><span data-ttu-id="62f71-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="62f71-138">Description</span></span>

<span data-ttu-id="62f71-139">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação de CreateItem.</span><span class="sxs-lookup"><span data-stu-id="62f71-139">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="62f71-140">Código</span><span class="sxs-lookup"><span data-stu-id="62f71-140">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="62f71-141">Comments</span><span class="sxs-lookup"><span data-stu-id="62f71-141">Comments</span></span>

<span data-ttu-id="62f71-142">Os atributos de [ItemId](itemid.md) elemento **Id** e **ChangeKey** foram diminuídos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="62f71-142">The [ItemId](itemid.md) element **Id** and **ChangeKey** attributes have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="62f71-143">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="62f71-143">Successful response elements</span></span>

<span data-ttu-id="62f71-144">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="62f71-144">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="62f71-145">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="62f71-145">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="62f71-146">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="62f71-146">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="62f71-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="62f71-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="62f71-148">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="62f71-148">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="62f71-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="62f71-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="62f71-150">Items</span><span class="sxs-lookup"><span data-stu-id="62f71-150">Items</span></span>](items.md)
    
- [<span data-ttu-id="62f71-151">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="62f71-151">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="62f71-152">ItemId</span><span class="sxs-lookup"><span data-stu-id="62f71-152">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="62f71-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="62f71-153">See also</span></span>



[<span data-ttu-id="62f71-154">Operação CreateItem</span><span class="sxs-lookup"><span data-stu-id="62f71-154">CreateItem operation</span></span>](createitem-operation.md)

