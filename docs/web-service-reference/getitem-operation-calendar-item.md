---
title: Operação GetItem (item de calendário)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8
description: A operação GetItem obtém os itens de calendário do Exchange store.
ms.openlocfilehash: 69bce0f0cc7b5c986f9bf4767c3cd429a309e50d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752530"
---
# <a name="getitem-operation-calendar-item"></a><span data-ttu-id="505f5-103">Operação GetItem (item de calendário)</span><span class="sxs-lookup"><span data-stu-id="505f5-103">GetItem operation (calendar item)</span></span>

<span data-ttu-id="505f5-104">A operação GetItem obtém os itens de calendário do Exchange store.</span><span class="sxs-lookup"><span data-stu-id="505f5-104">The GetItem operation gets calendar items from the Exchange store.</span></span>
  
## <a name="getitem-request-example"></a><span data-ttu-id="505f5-105">Exemplo de solicitação de GetItem</span><span class="sxs-lookup"><span data-stu-id="505f5-105">GetItem request example</span></span>

### <a name="description"></a><span data-ttu-id="505f5-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="505f5-106">Description</span></span>

<span data-ttu-id="505f5-107">O exemplo a seguir de uma solicitação de GetItem mostra como uma solicitação para obter a identidade e o assunto de um item de formulário.</span><span class="sxs-lookup"><span data-stu-id="505f5-107">The following example of a GetItem request shows how to form a request to get the identity and subject of an item.</span></span>
  
### <a name="code"></a><span data-ttu-id="505f5-108">Código</span><span class="sxs-lookup"><span data-stu-id="505f5-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AsdD89=" ChangeKey="Jajs3=="/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="505f5-109">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="505f5-109">Request elements</span></span>

<span data-ttu-id="505f5-110">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="505f5-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="505f5-111">GetItem</span><span class="sxs-lookup"><span data-stu-id="505f5-111">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="505f5-112">ItemShape</span><span class="sxs-lookup"><span data-stu-id="505f5-112">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="505f5-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="505f5-113">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="505f5-114">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="505f5-114">AdditionalProperties</span></span>](additionalproperties.md)
    
- [<span data-ttu-id="505f5-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="505f5-115">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="505f5-116">ItemIds</span><span class="sxs-lookup"><span data-stu-id="505f5-116">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="505f5-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="505f5-117">ItemId</span></span>](itemid.md)
    
> [!NOTE]
> <span data-ttu-id="505f5-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="505f5-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="505f5-119">Para localizar outras opções para a mensagem de solicitação da operação GetItem, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="505f5-119">To find other options for the request message of the GetItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="505f5-120">Inicie o elemento [GetItem](getitem.md) .</span><span class="sxs-lookup"><span data-stu-id="505f5-120">Start at the [GetItem](getitem.md) element.</span></span> 
  
## <a name="successful-getitem-response"></a><span data-ttu-id="505f5-121">Resposta de GetItem bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="505f5-121">Successful GetItem Response</span></span>

### <a name="description"></a><span data-ttu-id="505f5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="505f5-122">Description</span></span>

<span data-ttu-id="505f5-123">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação de GetItem.</span><span class="sxs-lookup"><span data-stu-id="505f5-123">The following example shows a successful response to the GetItem request.</span></span> <span data-ttu-id="505f5-124">A solicitação que criou esta resposta usado o baseshape IdOnly.</span><span class="sxs-lookup"><span data-stu-id="505f5-124">The request that created this response used the IdOnly baseshape.</span></span> <span data-ttu-id="505f5-125">Neste exemplo, a resposta retorna apenas a ID do item.</span><span class="sxs-lookup"><span data-stu-id="505f5-125">In this example, the response returns only the ID of the item.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="505f5-126">A ID de item e a chave de alteração tem sido reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="505f5-126">The item ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="505f5-127">Código</span><span class="sxs-lookup"><span data-stu-id="505f5-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                   xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="ASUAd" ChangeKey="otlIqB=="/>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="description"></a><span data-ttu-id="505f5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="505f5-128">Description</span></span>

<span data-ttu-id="505f5-129">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação de GetItem.</span><span class="sxs-lookup"><span data-stu-id="505f5-129">The following example shows a successful response to the GetItem request.</span></span> <span data-ttu-id="505f5-130">A solicitação que criou esta resposta usado o baseshape padrão.</span><span class="sxs-lookup"><span data-stu-id="505f5-130">The request that created this response used the Default baseshape.</span></span> <span data-ttu-id="505f5-131">Neste exemplo, a resposta retorna a forma padrão de um item do calendário.</span><span class="sxs-lookup"><span data-stu-id="505f5-131">In this example, the response returns the Default shape for a calendar item.</span></span>
  
> [!NOTE]
> <span data-ttu-id="505f5-132">A ID de item e a chave de alteração tem sido reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="505f5-132">The item ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="505f5-133">Código</span><span class="sxs-lookup"><span data-stu-id="505f5-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="ASUAdTB" ChangeKey="otlIqBwrt=="/>
              <t:ResponseObjects>
                <t:ForwardItem/>
              </t:ResponseObjects>
              <t:Start>2006-06-16T00:30:00Z</t:Start>
              <t:End>2006-06-16T01:00:00Z</t:End>
              <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
              <t:CalendarItemType>Single</t:CalendarItemType>
              <t:Organizer>
                <t:Mailbox>
                  <t:Name>Bob</t:Name>
                  <t:EmailAddress>someone@example.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Mailbox>
              </t:Organizer>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="description"></a><span data-ttu-id="505f5-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="505f5-134">Description</span></span>

<span data-ttu-id="505f5-135">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação de GetItem.</span><span class="sxs-lookup"><span data-stu-id="505f5-135">The following example shows a successful response to the GetItem request.</span></span> <span data-ttu-id="505f5-136">A solicitação que criou esta resposta usado o baseshape AllProperties.</span><span class="sxs-lookup"><span data-stu-id="505f5-136">The request that created this response used the AllProperties baseshape.</span></span> <span data-ttu-id="505f5-137">Neste exemplo, a resposta retorna a forma de AllProperties para um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="505f5-137">In this example, the response returns the AllProperties shape for a calendar item.</span></span>
  
### <a name="code"></a><span data-ttu-id="505f5-138">Código</span><span class="sxs-lookup"><span data-stu-id="505f5-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="ASUAdT" ChangeKey="otlIqB=="/>
              <t:ParentFolderId Id="ASUAdT=="/>
              <t:ItemClass>IPM.Appointment</t:ItemClass>
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="Text"/>
              <t:DateTimeReceived>2006-06-16T00:12:41Z</t:DateTimeReceived>
              <t:Size>374</t:Size>
              <t:Importance>Normal</t:Importance>
              <t:IsSubmitted>false</t:IsSubmitted>
              <t:IsDraft>false</t:IsDraft>
              <t:IsFromMe>false</t:IsFromMe>
              <t:IsResend>false</t:IsResend>
              <t:IsUnmodified>false</t:IsUnmodified>
              <t:DateTimeSent>2006-06-16T00:12:41Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-06-16T00:12:41Z</t:DateTimeCreated>
              <t:ResponseObjects>
                <t:ForwardItem/>
              </t:ResponseObjects>
              <t:ReminderDueBy>2006-06-16T00:30:00Z</t:ReminderDueBy>
              <t:ReminderIsSet>true</t:ReminderIsSet>
              <t:ReminderMinutesBeforeStart>15</t:ReminderMinutesBeforeStart>
              <t:DisplayCc/>
              <t:DisplayTo/>
              <t:HasAttachments>false</t:HasAttachments>
              <t:Culture>en-US</t:Culture>
              <t:Start>2006-06-16T00:30:00Z</t:Start>
              <t:End>2006-06-16T01:00:00Z</t:End>
              <t:IsAllDayEvent>false</t:IsAllDayEvent>
              <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
              <t:IsMeeting>false</t:IsMeeting>
              <t:IsCancelled>false</t:IsCancelled>
              <t:IsRecurring>false</t:IsRecurring>
              <t:MeetingRequestWasSent>false</t:MeetingRequestWasSent>
              <t:CalendarItemType>Single</t:CalendarItemType>
              <t:MyResponseType>Organizer</t:MyResponseType>
              <t:Organizer>
                <t:Mailbox>
                  <t:Name>Bob</t:Name>
                  <t:EmailAddress>someone@example.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Mailbox>
              </t:Organizer>
              <t:ConflictingMeetingCount>2</t:ConflictingMeetingCount>
              <t:AdjacentMeetingCount>0</t:AdjacentMeetingCount>
              <t:ConflictingMeetings>
                <t:CalendarItem>
                  <t:ItemId Id="ASUAdTB" ChangeKey="otlIqBwr=="/>
                  <t:Subject/>
                  <t:Start>2006-06-16T00:30:00Z</t:Start>
                  <t:End>2006-06-16T01:00:00Z</t:End>
                  <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
                  <t:Location/>
                </t:CalendarItem>
                <t:CalendarItem>
                  <t:ItemId Id="ASUAd" ChangeKey="otlIqBw=="/>
                  <t:Subject/>
                  <t:Start>2006-06-16T00:30:00Z</t:Start>
                  <t:End>2006-06-16T01:00:00Z</t:End>
                  <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
                  <t:Location/>
                </t:CalendarItem>
              </t:ConflictingMeetings>
              <t:Duration>PT30M</t:Duration>
              <t:TimeZone>Pacific Standard Time</t:TimeZone>
              <t:AppointmentSequenceNumber>0</t:AppointmentSequenceNumber>
              <t:AppointmentState>0</t:AppointmentState>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="505f5-139">Comments</span><span class="sxs-lookup"><span data-stu-id="505f5-139">Comments</span></span>

<span data-ttu-id="505f5-140">Para localizar outras opções para a mensagem de resposta da operação GetItem, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="505f5-140">To find other options for the response message of the GetItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="505f5-141">Inicie o elemento [GetItemResponse](getitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="505f5-141">Start at the [GetItemResponse](getitemresponse.md) element.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="505f5-142">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="505f5-142">Successful response elements</span></span>

<span data-ttu-id="505f5-143">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="505f5-143">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="505f5-144">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="505f5-144">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="505f5-145">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="505f5-145">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="505f5-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="505f5-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="505f5-147">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="505f5-147">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="505f5-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="505f5-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="505f5-149">Items</span><span class="sxs-lookup"><span data-stu-id="505f5-149">Items</span></span>](items.md)
    
- [<span data-ttu-id="505f5-150">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="505f5-150">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="505f5-151">ItemId</span><span class="sxs-lookup"><span data-stu-id="505f5-151">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="505f5-152">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="505f5-152">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="505f5-153">ItemClass</span><span class="sxs-lookup"><span data-stu-id="505f5-153">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="505f5-154">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="505f5-154">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="505f5-155">Corpo</span><span class="sxs-lookup"><span data-stu-id="505f5-155">Body</span></span>](body.md)
    
- [<span data-ttu-id="505f5-156">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="505f5-156">DateTimeReceived</span></span>](datetimereceived.md)
    
- [<span data-ttu-id="505f5-157">Size</span><span class="sxs-lookup"><span data-stu-id="505f5-157">Size</span></span>](size.md)
    
- [<span data-ttu-id="505f5-158">Importância</span><span class="sxs-lookup"><span data-stu-id="505f5-158">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="505f5-159">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="505f5-159">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="505f5-160">IsDraft</span><span class="sxs-lookup"><span data-stu-id="505f5-160">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="505f5-161">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="505f5-161">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="505f5-162">IsResend</span><span class="sxs-lookup"><span data-stu-id="505f5-162">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="505f5-163">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="505f5-163">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="505f5-164">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="505f5-164">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="505f5-165">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="505f5-165">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="505f5-166">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="505f5-166">ResponseObjects</span></span>](responseobjects.md)
    
- [<span data-ttu-id="505f5-167">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="505f5-167">ForwardItem</span></span>](forwarditem.md)
    
- [<span data-ttu-id="505f5-168">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="505f5-168">ReminderDueBy</span></span>](reminderdueby.md)
    
- [<span data-ttu-id="505f5-169">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="505f5-169">ReminderIsSet</span></span>](reminderisset.md)
    
- [<span data-ttu-id="505f5-170">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="505f5-170">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md)
    
- [<span data-ttu-id="505f5-171">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="505f5-171">DisplayCc</span></span>](displaycc.md)
    
- [<span data-ttu-id="505f5-172">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="505f5-172">DisplayTo</span></span>](displayto.md)
    
- [<span data-ttu-id="505f5-173">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="505f5-173">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="505f5-174">Cultura</span><span class="sxs-lookup"><span data-stu-id="505f5-174">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="505f5-175">Start</span><span class="sxs-lookup"><span data-stu-id="505f5-175">Start</span></span>](start.md)
    
- [<span data-ttu-id="505f5-176">End</span><span class="sxs-lookup"><span data-stu-id="505f5-176">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="505f5-177">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="505f5-177">IsAllDayEvent</span></span>](isalldayevent.md)
    
- [<span data-ttu-id="505f5-178">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="505f5-178">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md)
    
- [<span data-ttu-id="505f5-179">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="505f5-179">IsMeeting</span></span>](ismeeting.md)
    
- [<span data-ttu-id="505f5-180">IsCancelled</span><span class="sxs-lookup"><span data-stu-id="505f5-180">IsCancelled</span></span>](iscancelled.md)
    
- [<span data-ttu-id="505f5-181">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="505f5-181">IsRecurring</span></span>](isrecurring.md)
    
- [<span data-ttu-id="505f5-182">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="505f5-182">MeetingRequestWasSent</span></span>](meetingrequestwassent.md)
    
- [<span data-ttu-id="505f5-183">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="505f5-183">CalendarItemType</span></span>](calendaritemtype.md)
    
- [<span data-ttu-id="505f5-184">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="505f5-184">MyResponseType</span></span>](myresponsetype.md)
    
- [<span data-ttu-id="505f5-185">Organizer</span><span class="sxs-lookup"><span data-stu-id="505f5-185">Organizer</span></span>](organizer.md)
    
- [<span data-ttu-id="505f5-186">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="505f5-186">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="505f5-187">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="505f5-187">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="505f5-188">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="505f5-188">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="505f5-189">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="505f5-189">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="505f5-190">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="505f5-190">ConflictingMeetingCount</span></span>](conflictingmeetingcount.md)
    
- [<span data-ttu-id="505f5-191">AdjacentMeetingCount</span><span class="sxs-lookup"><span data-stu-id="505f5-191">AdjacentMeetingCount</span></span>](adjacentmeetingcount.md)
    
- [<span data-ttu-id="505f5-192">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="505f5-192">ConflictingMeetings</span></span>](conflictingmeetings.md)
    
- [<span data-ttu-id="505f5-193">Location</span><span class="sxs-lookup"><span data-stu-id="505f5-193">Location</span></span>](location.md)
    
- [<span data-ttu-id="505f5-194">Duração (itens)</span><span class="sxs-lookup"><span data-stu-id="505f5-194">Duration (Items)</span></span>](duration-items.md)
    
- [<span data-ttu-id="505f5-195">Fuso horário (Item)</span><span class="sxs-lookup"><span data-stu-id="505f5-195">TimeZone (Item)</span></span>](timezone-item.md)
    
- [<span data-ttu-id="505f5-196">AppointmentSequenceNumber</span><span class="sxs-lookup"><span data-stu-id="505f5-196">AppointmentSequenceNumber</span></span>](appointmentsequencenumber.md)
    
- [<span data-ttu-id="505f5-197">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="505f5-197">AppointmentState</span></span>](appointmentstate.md)
    
## <a name="see-also"></a><span data-ttu-id="505f5-198">Confira também</span><span class="sxs-lookup"><span data-stu-id="505f5-198">See also</span></span>



[<span data-ttu-id="505f5-199">Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="505f5-199">GetItem operation</span></span>](getitem-operation.md)

