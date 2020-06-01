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
description: A operação GetItem Obtém itens de calendário do repositório do Exchange.
ms.openlocfilehash: 09fe92af12f03ce4cebd1e98f4e01c087ace64f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460614"
---
# <a name="getitem-operation-calendar-item"></a><span data-ttu-id="0a24e-103">Operação GetItem (item de calendário)</span><span class="sxs-lookup"><span data-stu-id="0a24e-103">GetItem operation (calendar item)</span></span>

<span data-ttu-id="0a24e-104">A operação GetItem Obtém itens de calendário do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0a24e-104">The GetItem operation gets calendar items from the Exchange store.</span></span>
  
## <a name="getitem-request-example"></a><span data-ttu-id="0a24e-105">Exemplo de solicitação GetItem</span><span class="sxs-lookup"><span data-stu-id="0a24e-105">GetItem request example</span></span>

### <a name="description"></a><span data-ttu-id="0a24e-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a24e-106">Description</span></span>

<span data-ttu-id="0a24e-107">O exemplo a seguir de uma solicitação GetItem mostra como formar uma solicitação para obter a identidade e o assunto de um item.</span><span class="sxs-lookup"><span data-stu-id="0a24e-107">The following example of a GetItem request shows how to form a request to get the identity and subject of an item.</span></span>
  
### <a name="code"></a><span data-ttu-id="0a24e-108">Código</span><span class="sxs-lookup"><span data-stu-id="0a24e-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="request-elements"></a><span data-ttu-id="0a24e-109">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="0a24e-109">Request elements</span></span>

<span data-ttu-id="0a24e-110">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="0a24e-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="0a24e-111">GetItem</span><span class="sxs-lookup"><span data-stu-id="0a24e-111">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="0a24e-112">Shape</span><span class="sxs-lookup"><span data-stu-id="0a24e-112">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="0a24e-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="0a24e-113">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="0a24e-114">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="0a24e-114">AdditionalProperties</span></span>](additionalproperties.md)
    
- [<span data-ttu-id="0a24e-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="0a24e-115">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="0a24e-116">ItemIds</span><span class="sxs-lookup"><span data-stu-id="0a24e-116">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="0a24e-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="0a24e-117">ItemId</span></span>](itemid.md)
    
> [!NOTE]
> <span data-ttu-id="0a24e-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="0a24e-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="0a24e-119">Para encontrar outras opções para a mensagem de solicitação da operação GetItem, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="0a24e-119">To find other options for the request message of the GetItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="0a24e-120">Inicie no elemento [GetItem](getitem.md) .</span><span class="sxs-lookup"><span data-stu-id="0a24e-120">Start at the [GetItem](getitem.md) element.</span></span> 
  
## <a name="successful-getitem-response"></a><span data-ttu-id="0a24e-121">Resposta GetItem bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="0a24e-121">Successful GetItem Response</span></span>

### <a name="description"></a><span data-ttu-id="0a24e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a24e-122">Description</span></span>

<span data-ttu-id="0a24e-123">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação GetItem.</span><span class="sxs-lookup"><span data-stu-id="0a24e-123">The following example shows a successful response to the GetItem request.</span></span> <span data-ttu-id="0a24e-124">A solicitação que criou essa resposta utilizou o IdOnly BaseShape.</span><span class="sxs-lookup"><span data-stu-id="0a24e-124">The request that created this response used the IdOnly baseshape.</span></span> <span data-ttu-id="0a24e-125">Neste exemplo, a resposta retorna apenas a ID do item.</span><span class="sxs-lookup"><span data-stu-id="0a24e-125">In this example, the response returns only the ID of the item.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0a24e-126">A ID do item e a chave de alteração foram reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0a24e-126">The item ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0a24e-127">Código</span><span class="sxs-lookup"><span data-stu-id="0a24e-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                   xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="description"></a><span data-ttu-id="0a24e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a24e-128">Description</span></span>

<span data-ttu-id="0a24e-129">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação GetItem.</span><span class="sxs-lookup"><span data-stu-id="0a24e-129">The following example shows a successful response to the GetItem request.</span></span> <span data-ttu-id="0a24e-130">A solicitação que criou essa resposta utilizou o BaseShape padrão.</span><span class="sxs-lookup"><span data-stu-id="0a24e-130">The request that created this response used the Default baseshape.</span></span> <span data-ttu-id="0a24e-131">Neste exemplo, a resposta retorna a forma padrão para um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="0a24e-131">In this example, the response returns the Default shape for a calendar item.</span></span>
  
> [!NOTE]
> <span data-ttu-id="0a24e-132">A ID do item e a chave de alteração foram reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0a24e-132">The item ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0a24e-133">Código</span><span class="sxs-lookup"><span data-stu-id="0a24e-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="description"></a><span data-ttu-id="0a24e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a24e-134">Description</span></span>

<span data-ttu-id="0a24e-135">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação GetItem.</span><span class="sxs-lookup"><span data-stu-id="0a24e-135">The following example shows a successful response to the GetItem request.</span></span> <span data-ttu-id="0a24e-136">A solicitação que criou essa resposta utilizou a propriedade BaseShape.</span><span class="sxs-lookup"><span data-stu-id="0a24e-136">The request that created this response used the AllProperties baseshape.</span></span> <span data-ttu-id="0a24e-137">Neste exemplo, a resposta retorna a forma myproperties de um item do calendário.</span><span class="sxs-lookup"><span data-stu-id="0a24e-137">In this example, the response returns the AllProperties shape for a calendar item.</span></span>
  
### <a name="code"></a><span data-ttu-id="0a24e-138">Código</span><span class="sxs-lookup"><span data-stu-id="0a24e-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="0a24e-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="0a24e-139">Comments</span></span>

<span data-ttu-id="0a24e-140">Para encontrar outras opções para a mensagem de resposta da operação GetItem, explore a hierarquia do esquema.</span><span class="sxs-lookup"><span data-stu-id="0a24e-140">To find other options for the response message of the GetItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="0a24e-141">Inicie no elemento [GetItemResponse](getitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="0a24e-141">Start at the [GetItemResponse](getitemresponse.md) element.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="0a24e-142">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="0a24e-142">Successful response elements</span></span>

<span data-ttu-id="0a24e-143">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="0a24e-143">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="0a24e-144">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0a24e-144">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="0a24e-145">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="0a24e-145">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="0a24e-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0a24e-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0a24e-147">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0a24e-147">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="0a24e-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0a24e-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0a24e-149">Itens</span><span class="sxs-lookup"><span data-stu-id="0a24e-149">Items</span></span>](items.md)
    
- [<span data-ttu-id="0a24e-150">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="0a24e-150">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="0a24e-151">ItemId</span><span class="sxs-lookup"><span data-stu-id="0a24e-151">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="0a24e-152">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="0a24e-152">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="0a24e-153">ItemClass</span><span class="sxs-lookup"><span data-stu-id="0a24e-153">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="0a24e-154">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="0a24e-154">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="0a24e-155">Body</span><span class="sxs-lookup"><span data-stu-id="0a24e-155">Body</span></span>](body.md)
    
- [<span data-ttu-id="0a24e-156">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="0a24e-156">DateTimeReceived</span></span>](datetimereceived.md)
    
- [<span data-ttu-id="0a24e-157">Tamanho</span><span class="sxs-lookup"><span data-stu-id="0a24e-157">Size</span></span>](size.md)
    
- [<span data-ttu-id="0a24e-158">Importance</span><span class="sxs-lookup"><span data-stu-id="0a24e-158">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="0a24e-159">Isenviado</span><span class="sxs-lookup"><span data-stu-id="0a24e-159">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="0a24e-160">IsDraft</span><span class="sxs-lookup"><span data-stu-id="0a24e-160">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="0a24e-161">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="0a24e-161">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="0a24e-162">IsResend</span><span class="sxs-lookup"><span data-stu-id="0a24e-162">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="0a24e-163">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="0a24e-163">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="0a24e-164">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="0a24e-164">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="0a24e-165">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="0a24e-165">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="0a24e-166">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="0a24e-166">ResponseObjects</span></span>](responseobjects.md)
    
- [<span data-ttu-id="0a24e-167">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="0a24e-167">ForwardItem</span></span>](forwarditem.md)
    
- [<span data-ttu-id="0a24e-168">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="0a24e-168">ReminderDueBy</span></span>](reminderdueby.md)
    
- [<span data-ttu-id="0a24e-169">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="0a24e-169">ReminderIsSet</span></span>](reminderisset.md)
    
- [<span data-ttu-id="0a24e-170">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="0a24e-170">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md)
    
- [<span data-ttu-id="0a24e-171">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="0a24e-171">DisplayCc</span></span>](displaycc.md)
    
- [<span data-ttu-id="0a24e-172">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="0a24e-172">DisplayTo</span></span>](displayto.md)
    
- [<span data-ttu-id="0a24e-173">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="0a24e-173">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="0a24e-174">Cultura</span><span class="sxs-lookup"><span data-stu-id="0a24e-174">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="0a24e-175">Start</span><span class="sxs-lookup"><span data-stu-id="0a24e-175">Start</span></span>](start.md)
    
- [<span data-ttu-id="0a24e-176">Ponto</span><span class="sxs-lookup"><span data-stu-id="0a24e-176">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="0a24e-177">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="0a24e-177">IsAllDayEvent</span></span>](isalldayevent.md)
    
- [<span data-ttu-id="0a24e-178">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="0a24e-178">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md)
    
- [<span data-ttu-id="0a24e-179">Issatisfaçing</span><span class="sxs-lookup"><span data-stu-id="0a24e-179">IsMeeting</span></span>](ismeeting.md)
    
- [<span data-ttu-id="0a24e-180">IsCanceled</span><span class="sxs-lookup"><span data-stu-id="0a24e-180">IsCancelled</span></span>](iscancelled.md)
    
- [<span data-ttu-id="0a24e-181">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="0a24e-181">IsRecurring</span></span>](isrecurring.md)
    
- [<span data-ttu-id="0a24e-182">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="0a24e-182">MeetingRequestWasSent</span></span>](meetingrequestwassent.md)
    
- [<span data-ttu-id="0a24e-183">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="0a24e-183">CalendarItemType</span></span>](calendaritemtype.md)
    
- [<span data-ttu-id="0a24e-184">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="0a24e-184">MyResponseType</span></span>](myresponsetype.md)
    
- [<span data-ttu-id="0a24e-185">Organizador</span><span class="sxs-lookup"><span data-stu-id="0a24e-185">Organizer</span></span>](organizer.md)
    
- [<span data-ttu-id="0a24e-186">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="0a24e-186">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="0a24e-187">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="0a24e-187">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="0a24e-188">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="0a24e-188">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="0a24e-189">RoutingType (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="0a24e-189">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="0a24e-190">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="0a24e-190">ConflictingMeetingCount</span></span>](conflictingmeetingcount.md)
    
- [<span data-ttu-id="0a24e-191">AdjacentMeetingCount</span><span class="sxs-lookup"><span data-stu-id="0a24e-191">AdjacentMeetingCount</span></span>](adjacentmeetingcount.md)
    
- [<span data-ttu-id="0a24e-192">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="0a24e-192">ConflictingMeetings</span></span>](conflictingmeetings.md)
    
- [<span data-ttu-id="0a24e-193">Localização</span><span class="sxs-lookup"><span data-stu-id="0a24e-193">Location</span></span>](location.md)
    
- [<span data-ttu-id="0a24e-194">Duração (itens)</span><span class="sxs-lookup"><span data-stu-id="0a24e-194">Duration (Items)</span></span>](duration-items.md)
    
- [<span data-ttu-id="0a24e-195">TimeZone (item)</span><span class="sxs-lookup"><span data-stu-id="0a24e-195">TimeZone (Item)</span></span>](timezone-item.md)
    
- [<span data-ttu-id="0a24e-196">AppointmentSequenceNumber</span><span class="sxs-lookup"><span data-stu-id="0a24e-196">AppointmentSequenceNumber</span></span>](appointmentsequencenumber.md)
    
- [<span data-ttu-id="0a24e-197">Compromissostate</span><span class="sxs-lookup"><span data-stu-id="0a24e-197">AppointmentState</span></span>](appointmentstate.md)
    
## <a name="see-also"></a><span data-ttu-id="0a24e-198">Também consulte</span><span class="sxs-lookup"><span data-stu-id="0a24e-198">See also</span></span>



[<span data-ttu-id="0a24e-199">Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="0a24e-199">GetItem operation</span></span>](getitem-operation.md)

