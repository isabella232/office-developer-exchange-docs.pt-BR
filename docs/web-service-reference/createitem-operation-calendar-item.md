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
description: A operação CreateItem cria itens de calendário no repositório do Exchange.
ms.openlocfilehash: 535edf9fe567bc3063a5b853f01d604ea4c7eb95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457498"
---
# <a name="createitem-operation-calendar-item"></a><span data-ttu-id="00832-103">Operação CreateItem (item de calendário)</span><span class="sxs-lookup"><span data-stu-id="00832-103">CreateItem operation (calendar item)</span></span>

<span data-ttu-id="00832-104">A operação CreateItem cria itens de calendário no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="00832-104">The CreateItem operation creates calendar items in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="00832-105">Comentários</span><span class="sxs-lookup"><span data-stu-id="00832-105">Remarks</span></span>

<span data-ttu-id="00832-106">A operação CreateItem cria compromissos, reuniões e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="00832-106">The CreateItem operation creates appointments, meetings, and meeting requests.</span></span> <span data-ttu-id="00832-107">Se um item de calendário for criado sem participantes, ele será considerado um compromisso.</span><span class="sxs-lookup"><span data-stu-id="00832-107">If a calendar item is created without attendees, it is considered an appointment.</span></span> <span data-ttu-id="00832-108">Se os participantes forem especificados, o item de calendário será uma reunião.</span><span class="sxs-lookup"><span data-stu-id="00832-108">If attendees are specified, the calendar item is a meeting.</span></span> <span data-ttu-id="00832-109">Quando uma reunião é criada usando a operação CreateItem, as solicitações de reunião são enviadas automaticamente para os participantes identificados se o atributo SendMeetingInvitations for definido para enviar as solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="00832-109">When a meeting is created by using the CreateItem operation, meeting requests are automatically sent to the identified attendees if the SendMeetingInvitations attribute is set to send the meeting requests.</span></span>
  
## <a name="createitem-calendar-item-request-example"></a><span data-ttu-id="00832-110">Exemplo de solicitação CreateItem (item de calendário)</span><span class="sxs-lookup"><span data-stu-id="00832-110">CreateItem (Calendar Item) request example</span></span>

### <a name="description"></a><span data-ttu-id="00832-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="00832-111">Description</span></span>

<span data-ttu-id="00832-112">O exemplo a seguir de uma solicitação CreateItem mostra como criar uma reunião com dois participantes obrigatórios.</span><span class="sxs-lookup"><span data-stu-id="00832-112">The following example of a CreateItem request shows how to create a meeting with two required attendees.</span></span> <span data-ttu-id="00832-113">Esta solicitação enviará as solicitações de reunião para os dois participantes.</span><span class="sxs-lookup"><span data-stu-id="00832-113">This request will send the meeting requests to the two attendees.</span></span>
  
### <a name="code"></a><span data-ttu-id="00832-114">Código</span><span class="sxs-lookup"><span data-stu-id="00832-114">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                SendMeetingInvitations="SendToAllAndSaveCopy" >
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar"/>
      </SavedItemFolderId>
      <Items>
        <t:CalendarItem xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="00832-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="00832-115">Comments</span></span>

<span data-ttu-id="00832-116">Para obter um exemplo de como responder a uma solicitação de reunião, consulte o tópico [operação CreateItem (solicitação de reunião)](createitem-operation-meeting-request.md) .</span><span class="sxs-lookup"><span data-stu-id="00832-116">For an example of how to respond to a meeting request, see the [CreateItem operation (meeting request)](createitem-operation-meeting-request.md) topic.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="00832-117">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="00832-117">Request elements</span></span>

<span data-ttu-id="00832-118">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="00832-118">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="00832-119">CreateItem</span><span class="sxs-lookup"><span data-stu-id="00832-119">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="00832-120">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="00832-120">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="00832-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="00832-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="00832-122">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="00832-122">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="00832-123">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="00832-123">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="00832-124">Assunto</span><span class="sxs-lookup"><span data-stu-id="00832-124">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="00832-125">Body</span><span class="sxs-lookup"><span data-stu-id="00832-125">Body</span></span>](body.md)
    
- [<span data-ttu-id="00832-126">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="00832-126">ReminderIsSet</span></span>](reminderisset.md)
    
- [<span data-ttu-id="00832-127">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="00832-127">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md)
    
- [<span data-ttu-id="00832-128">Start</span><span class="sxs-lookup"><span data-stu-id="00832-128">Start</span></span>](start.md)
    
- [<span data-ttu-id="00832-129">Ponto</span><span class="sxs-lookup"><span data-stu-id="00832-129">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="00832-130">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="00832-130">IsAllDayEvent</span></span>](isalldayevent.md)
    
- [<span data-ttu-id="00832-131">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="00832-131">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md)
    
- [<span data-ttu-id="00832-132">Localização</span><span class="sxs-lookup"><span data-stu-id="00832-132">Location</span></span>](location.md)
    
- [<span data-ttu-id="00832-133">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="00832-133">RequiredAttendees</span></span>](requiredattendees.md)
    
- [<span data-ttu-id="00832-134">Participante</span><span class="sxs-lookup"><span data-stu-id="00832-134">Attendee</span></span>](attendee.md)
    
- [<span data-ttu-id="00832-135">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="00832-135">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="00832-136">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="00832-136">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
## <a name="successful-createitem-calendar-item-response"></a><span data-ttu-id="00832-137">Resposta de CreateItem (item de calendário) bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="00832-137">Successful CreateItem (Calendar Item) Response</span></span>

### <a name="description"></a><span data-ttu-id="00832-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="00832-138">Description</span></span>

<span data-ttu-id="00832-139">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CreateItem.</span><span class="sxs-lookup"><span data-stu-id="00832-139">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="00832-140">Código</span><span class="sxs-lookup"><span data-stu-id="00832-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="00832-141">Comentários</span><span class="sxs-lookup"><span data-stu-id="00832-141">Comments</span></span>

<span data-ttu-id="00832-142">Os atributos **ID** do elemento [ItemId](itemid.md) e **ChangeKey** foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="00832-142">The [ItemId](itemid.md) element **Id** and **ChangeKey** attributes have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="00832-143">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="00832-143">Successful response elements</span></span>

<span data-ttu-id="00832-144">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="00832-144">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="00832-145">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="00832-145">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="00832-146">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="00832-146">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="00832-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="00832-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="00832-148">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="00832-148">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="00832-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="00832-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="00832-150">Itens</span><span class="sxs-lookup"><span data-stu-id="00832-150">Items</span></span>](items.md)
    
- [<span data-ttu-id="00832-151">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="00832-151">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="00832-152">ItemId</span><span class="sxs-lookup"><span data-stu-id="00832-152">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="00832-153">Também consulte</span><span class="sxs-lookup"><span data-stu-id="00832-153">See also</span></span>



[<span data-ttu-id="00832-154">Operação CreateItem</span><span class="sxs-lookup"><span data-stu-id="00832-154">CreateItem operation</span></span>](createitem-operation.md)

