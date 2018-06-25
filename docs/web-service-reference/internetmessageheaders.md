---
title: InternetMessageHeaders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternetMessageHeaders
api_type:
- schema
ms.assetid: 4dcf8671-96df-4a2d-9836-7e8e3a67e0db
description: O elemento InternetMessageHeaders contém uma coleção de alguns dos cabeçalhos de mensagem da Internet que estão contidos em um item em uma caixa de correio. Para obter toda a coleção de cabeçalhos de mensagem da Internet, use a propriedade PR_TRANSPORT_MESSAGE_HEADERS. Para obter mais informações sobre o EWS e cabeçalhos de mensagens da Internet, seeGetting Internet mensagem headersin EWS, MIME e os cabeçalhos das mensagens de Internet ausentes.
ms.openlocfilehash: 2da529a8a3532cebb2791b285b7673c962a2a656
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823954"
---
# <a name="internetmessageheaders"></a><span data-ttu-id="abf62-105">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="abf62-105">InternetMessageHeaders</span></span>

<span data-ttu-id="abf62-106">O elemento **InternetMessageHeaders** contém uma coleção de alguns dos cabeçalhos de mensagem da Internet que estão contidos em um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="abf62-106">The **InternetMessageHeaders** element contains a collection of some of the Internet message headers that are contained in an item in a mailbox.</span></span> <span data-ttu-id="abf62-107">Para obter toda a coleção de cabeçalhos de mensagem da Internet, use a propriedade **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="abf62-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="abf62-108">Para obter mais informações sobre cabeçalhos de mensagem do EWS e a Internet, consulte "Cabeçalhos de mensagens da Internet Getting" em [EWS, MIME e os cabeçalhos das mensagens de Internet ausentes](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="abf62-108">For more information about EWS and Internet message headers, see "Getting Internet message headers" in [EWS, MIME, and the missing Internet message headers](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeaders>
   <InternetMessageHeader/>
</InternetMessageHeaders>
```

 <span data-ttu-id="abf62-109">**NonEmptyArrayOfInternetHeadersType**</span><span class="sxs-lookup"><span data-stu-id="abf62-109">**NonEmptyArrayOfInternetHeadersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="abf62-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="abf62-110">Attributes and elements</span></span>

<span data-ttu-id="abf62-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="abf62-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="abf62-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="abf62-112">Attributes</span></span>

<span data-ttu-id="abf62-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="abf62-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="abf62-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="abf62-114">Child elements</span></span>

|<span data-ttu-id="abf62-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="abf62-115">**Element**</span></span>|<span data-ttu-id="abf62-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="abf62-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="abf62-117">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="abf62-117">InternetMessageHeader</span></span>](internetmessageheader.md) <br/> |<span data-ttu-id="abf62-118">Representa o cabeçalho da mensagem para um determinado cabeçalho dentro da coleção de cabeçalhos da Internet.</span><span class="sxs-lookup"><span data-stu-id="abf62-118">Represents the Internet message header for a given header within the headers collection.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="abf62-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="abf62-119">Parent elements</span></span>

|<span data-ttu-id="abf62-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="abf62-120">**Element**</span></span>|<span data-ttu-id="abf62-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="abf62-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="abf62-122">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="abf62-122">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="abf62-123">Representa uma resposta de aceitar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="abf62-123">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="abf62-124">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="abf62-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="abf62-125">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="abf62-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="abf62-126">Contato</span><span class="sxs-lookup"><span data-stu-id="abf62-126">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="abf62-127">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="abf62-127">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="abf62-128">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="abf62-128">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="abf62-129">Representa uma resposta recusar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="abf62-129">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="abf62-130">DistributionList</span><span class="sxs-lookup"><span data-stu-id="abf62-130">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="abf62-131">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="abf62-131">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="abf62-132">1.1</span><span class="sxs-lookup"><span data-stu-id="abf62-132">Item</span></span>](item.md) <br/> |<span data-ttu-id="abf62-133">Representa um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="abf62-133">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="abf62-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="abf62-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="abf62-135">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="abf62-135">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="abf62-136">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="abf62-136">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="abf62-137">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="abf62-137">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="abf62-138">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="abf62-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="abf62-139">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="abf62-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="abf62-140">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="abf62-140">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="abf62-141">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="abf62-141">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="abf62-142">Mensagem</span><span class="sxs-lookup"><span data-stu-id="abf62-142">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="abf62-143">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="abf62-143">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="abf62-144">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="abf62-144">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="abf62-145">Remove um item de armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="abf62-145">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="abf62-146">Task</span><span class="sxs-lookup"><span data-stu-id="abf62-146">Task</span></span>](task.md) <br/> |<span data-ttu-id="abf62-147">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="abf62-147">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="abf62-148">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="abf62-148">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="abf62-149">Representa uma resposta provisoriamente aceita para uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="abf62-149">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="abf62-150">Comentários</span><span class="sxs-lookup"><span data-stu-id="abf62-150">Remarks</span></span>

<span data-ttu-id="abf62-151">Apresentamos a seguir o EWS Managed API estendido a definição de propriedade para a propriedade **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="abf62-151">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="abf62-152">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="abf62-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="abf62-153">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="abf62-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="abf62-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="abf62-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="abf62-155">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="abf62-155">Schema Name</span></span>  <br/> |<span data-ttu-id="abf62-156">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="abf62-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="abf62-157">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="abf62-157">Validation File</span></span>  <br/> |<span data-ttu-id="abf62-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="abf62-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="abf62-159">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="abf62-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="abf62-160">False</span><span class="sxs-lookup"><span data-stu-id="abf62-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="abf62-161">Ver também</span><span class="sxs-lookup"><span data-stu-id="abf62-161">See also</span></span>



- [<span data-ttu-id="abf62-162">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="abf62-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="abf62-163">EWS, MIME e os cabeçalhos das mensagens de Internet ausentes</span><span class="sxs-lookup"><span data-stu-id="abf62-163">EWS, MIME, and the missing Internet message headers</span></span>](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)

