---
title: Propor um novo horário de reunião usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d5ac8e5b-3876-4f20-b4d3-44505e066042
description: Descubra como propor novos horários de reunião do seu aplicativo de cliente do Exchange usando o EWS no Exchange.
ms.openlocfilehash: 4f001bb82d2325624b567412620283619b51f25b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456805"
---
# <a name="propose-a-new-meeting-time-by-using-ews-in-exchange"></a><span data-ttu-id="e156e-103">Propor um novo horário de reunião usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e156e-103">Propose a new meeting time by using EWS in Exchange</span></span>

<span data-ttu-id="e156e-104">Descubra como propor novos horários de reunião do seu aplicativo de cliente do Exchange usando o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="e156e-104">Find out how to propose new meeting times from your Exchange client application by using EWS in Exchange.</span></span>
  
<span data-ttu-id="e156e-105">O recurso propor novo horário permite que os participantes proponham novos horários de reunião ao organizador da reunião como parte do fluxo de trabalho do calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e156e-105">The propose new time feature enables attendees to propose new meeting times to the meeting organizer as part of the Exchange calendar workflow.</span></span> <span data-ttu-id="e156e-106">Quando um participante propõe uma nova reunião, o organizador pode usar o novo tempo proposto para a reunião para atualizar a reunião e enviar atualizações a todos os participantes.</span><span class="sxs-lookup"><span data-stu-id="e156e-106">When an attendee proposes a new meeting, the organizer can use the proposed new meeting time to update the meeting and send updates to all attendees.</span></span> <span data-ttu-id="e156e-107">Antes de poder permitir que os participantes proponham novos horários de reunião, você precisa determinar se o organizador permite novas propostas de horários.</span><span class="sxs-lookup"><span data-stu-id="e156e-107">Before you can enable attendees to propose new meeting times, you need to determine whether the organizer allows for new time proposals.</span></span> <span data-ttu-id="e156e-108">Este artigo descreve como determinar se você pode propor um novo horário e como usar o EWS para propor um novo horário.</span><span class="sxs-lookup"><span data-stu-id="e156e-108">This article describes how to determine whether you can propose a new time and how to use EWS to propose a new time.</span></span>
  
> [!NOTE]
> <span data-ttu-id="e156e-109">A API gerenciada EWS não implementa essa funcionalidade.</span><span class="sxs-lookup"><span data-stu-id="e156e-109">The EWS Managed API does not implement this functionality.</span></span> 
  
## <a name="determine-whether-you-can-propose-a-new-time-for-a-meeting-by-using-ews"></a><span data-ttu-id="e156e-110">Determinar se você pode propor um novo horário para uma reunião usando o EWS</span><span class="sxs-lookup"><span data-stu-id="e156e-110">Determine whether you can propose a new time for a meeting by using EWS</span></span>
<span data-ttu-id="e156e-111"><a name="bk_Determine"> </a></span><span class="sxs-lookup"><span data-stu-id="e156e-111"><a name="bk_Determine"> </a></span></span>

<span data-ttu-id="e156e-112">Antes de propor um novo horário para uma reunião, você precisa encontrar uma referência a essa reunião e determinar se o organizador da reunião configurou a reunião para dar suporte a novas propostas de horário.</span><span class="sxs-lookup"><span data-stu-id="e156e-112">Before you can propose a new time for a meeting, you need to find a reference to that meeting and determine whether the meeting organizer configured the meeting to support new time proposals.</span></span> <span data-ttu-id="e156e-113">Você pode obter uma referência a uma reunião seguindo um destes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="e156e-113">You can get a reference to a meeting by doing either of the following:</span></span> 
  
- <span data-ttu-id="e156e-114">Localizando a solicitação de reunião na caixa de entrada</span><span class="sxs-lookup"><span data-stu-id="e156e-114">Finding the meeting request in the Inbox</span></span>
    
- <span data-ttu-id="e156e-115">Localizar o compromisso no calendário</span><span class="sxs-lookup"><span data-stu-id="e156e-115">Finding the appointment in the calendar</span></span>
    
<span data-ttu-id="e156e-116">Use as etapas a seguir para encontrar uma referência de reunião:</span><span class="sxs-lookup"><span data-stu-id="e156e-116">Use the following steps to find a meeting reference:</span></span>
  
1. <span data-ttu-id="e156e-117">Use a operação [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS (ou o método [Folder. FINDITEMS](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) EWS Managed API) para localizar a solicitação de reunião de destino ou o item de calendário.</span><span class="sxs-lookup"><span data-stu-id="e156e-117">Use the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS operation (or the [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) EWS Managed API method) to find the target meeting request or calendar item.</span></span> <span data-ttu-id="e156e-118">Como alternativa, você pode usar a operação [SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) EWS para obter o identificador da solicitação de reunião de destino ou do item de calendário.</span><span class="sxs-lookup"><span data-stu-id="e156e-118">Alternatively, you can use the [SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) EWS operation to get the identifier of the target meeting request or calendar item.</span></span> 
    
2. <span data-ttu-id="e156e-119">Analise os resultados da operação **FindItem** (ou do método **Folder. FindItems** ) para obter o identificador de item do item de reunião.</span><span class="sxs-lookup"><span data-stu-id="e156e-119">Parse the results of the **FindItem** operation (or **Folder.FindItems** method) to get the item identifier of the meeting item.</span></span> 
    
3. <span data-ttu-id="e156e-120">Use a operação [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS para obter os objetos Response da reunião.</span><span class="sxs-lookup"><span data-stu-id="e156e-120">Use the [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS operation to get the response objects for the meeting.</span></span> 
    
<span data-ttu-id="e156e-121">O XML a seguir mostra o que é enviado para solicitar os objetos Response em um item.</span><span class="sxs-lookup"><span data-stu-id="e156e-121">The following XML shows what is sent to request the response objects on an item.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:MailboxCulture>en-US</t:MailboxCulture>
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ResponseObjects"/>
          <t:FieldURI FieldURI="item:Subject"/>
          <t:FieldURI FieldURI="calendar:Start"/>
          <t:FieldURI FieldURI="calendar:End"/>
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="e156e-122">A resposta da operação **GetItem** será semelhante ao seguinte XML se você solicitar o identificador do item, a hora de início e término da reunião, a coleção de objetos de resposta e se o organizador permitir alterações propostas no horário da reunião.</span><span class="sxs-lookup"><span data-stu-id="e156e-122">The **GetItem** operation response will look similar to the following XML if you request the item identifier, the meeting start and end time, the response object collection, and if the organizer allows for proposed changes to the meeting time.</span></span> <span data-ttu-id="e156e-123">A coleção de objetos Response, que é representada pelo elemento [ResponseObjects](https://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) , contém o conjunto de respostas válidas para o item de calendário.</span><span class="sxs-lookup"><span data-stu-id="e156e-123">The response object collection, which is represented by the [ResponseObjects](https://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) element, contains the set of responses that are valid for the calendar item.</span></span> <span data-ttu-id="e156e-124">O elemento **ProposeNewTime** é um objeto Response que indica que o usuário pode propor um novo horário para a reunião.</span><span class="sxs-lookup"><span data-stu-id="e156e-124">The **ProposeNewTime** element is a response object that indicates that the user can propose a new time for the meeting.</span></span> <span data-ttu-id="e156e-125">Os elementos [AcceptItem](https://msdn.microsoft.com/library/05a15431-77e1-411a-a16b-5481d364d3cc%28Office.15%29.aspx), [TentativelyAcceptItem](https://msdn.microsoft.com/library/ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0%28Office.15%29.aspx)e [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) representam os objetos de resposta que você pode usar para propor um novo horário de reunião para o organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="e156e-125">The [AcceptItem](https://msdn.microsoft.com/library/05a15431-77e1-411a-a16b-5481d364d3cc%28Office.15%29.aspx), [TentativelyAcceptItem](https://msdn.microsoft.com/library/ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0%28Office.15%29.aspx), and [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) elements represent the response objects that you can use to propose a new meeting time to the meeting organizer.</span></span> 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:MeetingRequest>
              <t:ItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
              <t:Subject>Competitive analysis: kick off meeting</t:Subject>
              <t:ResponseObjects>
                <t:AcceptItem/>
                <t:TentativelyAcceptItem/>
                <t:DeclineItem/>
                <t:ProposeNewTime/>
                <t:ReplyToItem/>
                <t:ReplyAllToItem/>
                <t:ForwardItem/>
              </t:ResponseObjects>
              <t:Start>2013-11-09T17:00:00Z</t:Start>
              <t:End>2013-11-09T17:30:00Z</t:End>
            </t:MeetingRequest>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="propose-a-new-meeting-time-by-using-ews"></a><span data-ttu-id="e156e-126">Propor um novo horário de reunião usando o EWS</span><span class="sxs-lookup"><span data-stu-id="e156e-126">Propose a new meeting time by using EWS</span></span>
<span data-ttu-id="e156e-127"><a name="bk_Propose"> </a></span><span class="sxs-lookup"><span data-stu-id="e156e-127"><a name="bk_Propose"> </a></span></span>

<span data-ttu-id="e156e-128">Se você recebeu um objeto de resposta **ProposeNewTime** quando utilizou a operação **GetItem** para obter um item de calendário ou uma solicitação de reunião, é possível responder com um novo horário de reunião proposto.</span><span class="sxs-lookup"><span data-stu-id="e156e-128">If you received a **ProposeNewTime** response object when you used the **GetItem** operation to get a calendar item or meeting request, you can respond with a proposed new meeting time.</span></span> <span data-ttu-id="e156e-129">Se você não recebeu um objeto de resposta **ProposeNewTime** , não será possível propor um novo horário de reunião como parte do fluxo de trabalho do calendário.</span><span class="sxs-lookup"><span data-stu-id="e156e-129">If you didn't receive a **ProposeNewTime** response object, you won't be able to propose a new meeting time as part of the calendar workflow.</span></span> <span data-ttu-id="e156e-130">No entanto, você pode responder ao organizador para solicitar um novo horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="e156e-130">You can, however, reply to the organizer to request a new meeting time.</span></span> <span data-ttu-id="e156e-131">Se você receber um objeto de resposta **ProposeNewTime** , poderá responder à reunião referenciando seu identificador e propor um novo horário de reunião para o organizador.</span><span class="sxs-lookup"><span data-stu-id="e156e-131">If you receive a **ProposeNewTime** response object, you can respond to the meeting by referencing its identifier, and propose a new meeting time to the organizer.</span></span> <span data-ttu-id="e156e-132">É aí que o objeto de resposta **ProposeNewTime** é diferente do padrão de objeto Response típico, pois você não responde com um objeto de resposta **ProposeNewTime** .</span><span class="sxs-lookup"><span data-stu-id="e156e-132">This is where the **ProposeNewTime** response object is different than the typical response object pattern in that you don't respond with a **ProposeNewTime** response object.</span></span> <span data-ttu-id="e156e-133">Você usa um dos outros objetos de resposta da reunião, como **AcceptItem**, **TentativelyAcceptItem**ou **DeclineItem**, para propor uma nova reunião.</span><span class="sxs-lookup"><span data-stu-id="e156e-133">You use one of the other meeting response objects, such as **AcceptItem**, **TentativelyAcceptItem**, or **DeclineItem**, to propose a new meeting.</span></span> <span data-ttu-id="e156e-134">Este exemplo usa o objeto de resposta **AcceptItem** .</span><span class="sxs-lookup"><span data-stu-id="e156e-134">This example uses the **AcceptItem** response object.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013"/>
  </soap:Header>
  <soap:Body>
    <m:CreateItem>
      <m:Items>
        <t:AcceptItem>
          <t:Body BodyType="Text">This time works better for the HiPPO.</t:Body>
          <t:ReferenceItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
          <t:ProposedStart>2013-11-28T04:00:00Z</t:ProposedStart>
          <t:ProposedEnd>2013-11-28T04:30:00Z</t:ProposedEnd>
        </t:AcceptItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="e156e-135">A resposta a essa solicitação contém o identificador do item de calendário que foi adicionado ao calendário do participante e uma cópia da solicitação de reunião que foi colocada na pasta itens excluídos do participante.</span><span class="sxs-lookup"><span data-stu-id="e156e-135">The response to this request contains the identifier of the calendar item that was added to the attendee's calendar and a copy of the meeting request that was placed in the attendee's Deleted Items folder.</span></span> <span data-ttu-id="e156e-136">A mensagem de resposta com a nova proposta de tempo também foi salva na pasta Itens enviados do participante (você precisará localizar a mensagem de resposta da reunião para obter um identificador nela).</span><span class="sxs-lookup"><span data-stu-id="e156e-136">The response message with the new time proposal was also saved in the attendee's Sent Items folder (you will need to find the meeting response message to get a handle on it).</span></span>
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAGRmOWE2OWAAA=" ChangeKey="DwAAJsmU"/>
            </t:CalendarItem>
            <t:MeetingRequest>
              <t:ItemId Id="AAMkAGRmOWE2AAABB=" ChangeKey="AAAGJu1A"/>
            </t:MeetingRequest>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="e156e-137">O organizador receberá uma mensagem do [MeetingResponse](https://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx) quando o participante responder com um novo horário de reunião proposto.</span><span class="sxs-lookup"><span data-stu-id="e156e-137">The organizer will receive a [MeetingResponse](https://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx) message when the attendee responds with a proposed new meeting time.</span></span> <span data-ttu-id="e156e-138">A mensagem **MeetingResponse** contém a nova hora de início e a hora de início da reunião propostas e o identificador do item de calendário associado no calendário do organizador.</span><span class="sxs-lookup"><span data-stu-id="e156e-138">The **MeetingResponse** message contains the proposed new meeting start time and end time, and the identifier of the associated calendar item in the organizer's calendar.</span></span> <span data-ttu-id="e156e-139">O organizador pode usar essas informações para atualizar o item de calendário existente para a reunião.</span><span class="sxs-lookup"><span data-stu-id="e156e-139">The organizer can use that information to update their existing calendar item for the meeting.</span></span> <span data-ttu-id="e156e-140">Veja a seguir o fluxo de trabalho do organizador para responder a uma mensagem do **MeetingResponse** que propõe um novo horário de reunião:</span><span class="sxs-lookup"><span data-stu-id="e156e-140">The following is the workflow for the organizer to respond to a **MeetingResponse** message that proposes a new meeting time:</span></span> 
  
1. <span data-ttu-id="e156e-141">Determine se os elementos **ProposedStart** ou **ProposedEnd** foram definidos no **MeetingResponse**.</span><span class="sxs-lookup"><span data-stu-id="e156e-141">Determine whether the **ProposedStart** or **ProposedEnd** elements have been set in the **MeetingResponse**.</span></span> <span data-ttu-id="e156e-142">Em caso afirmativo, vá para a etapa 2.</span><span class="sxs-lookup"><span data-stu-id="e156e-142">If so, go to step 2.</span></span> <span data-ttu-id="e156e-143">Caso contrário, a mensagem **MeetingResponse** indicará se o participante aceitou, aceitou provisoriamente ou recusou a reunião.</span><span class="sxs-lookup"><span data-stu-id="e156e-143">If not, the **MeetingResponse** message only indicates whether the attendee has accepted, tentatively accepted, or declined the meeting.</span></span> 
    
2. <span data-ttu-id="e156e-144">Obtenha o item de calendário existente do organizador da reunião usando o identificador EWS retornado no elemento **AssociatedCalendarItemId** .</span><span class="sxs-lookup"><span data-stu-id="e156e-144">Get the organizer's existing calendar item for the meeting by using the EWS identifier returned in the **AssociatedCalendarItemId** element.</span></span> 
    
3. <span data-ttu-id="e156e-145">Compare o horário original de início e de término com o novo horário proposto da reunião.</span><span class="sxs-lookup"><span data-stu-id="e156e-145">Compare the original start and end time with the proposed new meeting time.</span></span> <span data-ttu-id="e156e-146">Se o novo horário proposto da reunião for aceitável para o organizador, vá para a etapa 4.</span><span class="sxs-lookup"><span data-stu-id="e156e-146">If the proposed new meeting time is acceptable to the organizer, go to step 4.</span></span> <span data-ttu-id="e156e-147">Caso contrário, o organizador da reunião poderá ignorar o tempo de reunião proposto ou enviar uma resposta de email ao participante que propôs o novo horário da reunião.</span><span class="sxs-lookup"><span data-stu-id="e156e-147">Otherwise, the meeting organizer can either ignore the proposed meeting time, or send an email response to the attendee that proposed the new meeting time.</span></span>
    
4. <span data-ttu-id="e156e-148">Opcion Execute uma chamada de operação do EWS do [GetUserAvailability](https://msdn.microsoft.com/library/8da17226-5d3a-4525-9ffa-d83730f47bb1%28Office.15%29.aspx) para descobrir se o tempo proposto funcionará para todos os participantes, incluindo as caixas de correio de sala e de recurso.</span><span class="sxs-lookup"><span data-stu-id="e156e-148">(Optional) Perform a [GetUserAvailability](https://msdn.microsoft.com/library/8da17226-5d3a-4525-9ffa-d83730f47bb1%28Office.15%29.aspx) EWS operation call to find out whether the proposed time will work for all attendees, including room and resource mailboxes.</span></span> <span data-ttu-id="e156e-149">(Você também pode usar o método [ExchangeService. GetUserAvailability](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) EWS Managed API para fazer isso.)</span><span class="sxs-lookup"><span data-stu-id="e156e-149">(You can also use the [ExchangeService.GetUserAvailability](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) EWS Managed API method to do this.)</span></span> 
    
5. <span data-ttu-id="e156e-150">O organizador pode atualizar sua reunião com os novos horários de reunião propostos e enviar as atualizações a todos os participantes usando a operação [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS (ou o [compromisso. atualizar](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) o método de API gerenciada do EWS).</span><span class="sxs-lookup"><span data-stu-id="e156e-150">The organizer can then update their meeting with the new proposed meeting times and send the updates to all attendees by using the [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS operation (or the [Appointment.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) EWS Managed API method).</span></span> 
    
<span data-ttu-id="e156e-151">A figura a seguir mostra o processo que ocorre entre o organizador da reunião, o participante e o servidor do Exchange que tratou as chamadas do EWS.</span><span class="sxs-lookup"><span data-stu-id="e156e-151">The following figure shows the process that occurs between the meeting organizer, the attendee, and the Exchange server that handled the EWS calls.</span></span>
  
<span data-ttu-id="e156e-152">**Figura 1. Processo para propor um novo horário de reunião**</span><span class="sxs-lookup"><span data-stu-id="e156e-152">**Figure 1. Process for proposing a new meeting time**</span></span>

![A figura mostra o fluxo de trabalho entre o organizador, o Exchange e um participante quando um novo horário de reunião é proposto. Se o organizador permitir novas propostas de reuniões, um participante poderá propor um novo horário para a reunião com um objeto de resposta.](media/Ex_ProposeNewMeetingTime.png)
  
## <a name="version-differences"></a><span data-ttu-id="e156e-155">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="e156e-155">Version differences</span></span>
<span data-ttu-id="e156e-156"><a name="bk_Behavior"> </a></span><span class="sxs-lookup"><span data-stu-id="e156e-156"><a name="bk_Behavior"> </a></span></span>

<span data-ttu-id="e156e-157">O recurso propor novo horário foi introduzido na versão de compilação do Exchange 15.00.0800.007.</span><span class="sxs-lookup"><span data-stu-id="e156e-157">The propose new time feature was introduced in Exchange build version 15.00.0800.007.</span></span> <span data-ttu-id="e156e-158">Nas versões anteriores do Exchange, os usuários do aplicativo EWS precisam enviar um email separado ao organizador da reunião para solicitar um horário de reunião diferente.</span><span class="sxs-lookup"><span data-stu-id="e156e-158">In earlier versions of Exchange, EWS application users have to send a separate email to the meeting organizer to request a different meeting time.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="e156e-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="e156e-159">See also</span></span>


- [<span data-ttu-id="e156e-160">Calendários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e156e-160">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="e156e-161">Criar compromissos e reuniões usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e156e-161">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="e156e-162">Obter compromissos e reuniões usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e156e-162">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="e156e-163">Atualizar compromissos e reuniões usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e156e-163">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="e156e-164">Excluir compromissos e cancelar reuniões usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e156e-164">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

