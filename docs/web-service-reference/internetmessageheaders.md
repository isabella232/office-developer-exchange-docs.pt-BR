---
title: Propriedadeinternetmessageheaders
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
description: O elemento Propriedadeinternetmessageheaders contém uma coleção de alguns cabeçalhos de mensagens da Internet que estão contidos em um item em uma caixa de correio. Para obter a coleção inteira de cabeçalhos de mensagens da Internet, use a propriedade PR_TRANSPORT_MESSAGE_HEADERS. Para obter mais informações sobre o EWS e cabeçalhos de mensagens da Internet, Consulteobter Internet Message cabeçalhos no EWS, MIME e os cabeçalhos de mensagem da Internet ausentes.
ms.openlocfilehash: 4719050c02590e021b29173c234466de3fdc58a4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467323"
---
# <a name="internetmessageheaders"></a><span data-ttu-id="e1cfe-105">Propriedadeinternetmessageheaders</span><span class="sxs-lookup"><span data-stu-id="e1cfe-105">InternetMessageHeaders</span></span>

<span data-ttu-id="e1cfe-106">O elemento **propriedadeinternetmessageheaders** contém uma coleção de alguns cabeçalhos de mensagens da Internet que estão contidos em um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-106">The **InternetMessageHeaders** element contains a collection of some of the Internet message headers that are contained in an item in a mailbox.</span></span> <span data-ttu-id="e1cfe-107">Para obter a coleção inteira de cabeçalhos de mensagens da Internet, use a propriedade **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="e1cfe-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="e1cfe-108">Para obter mais informações sobre o EWS e cabeçalhos de mensagens da Internet, consulte "obtendo cabeçalhos de mensagens da Internet" em [EWS, MIME e cabeçalhos de mensagem da Internet ausentes](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="e1cfe-108">For more information about EWS and Internet message headers, see "Getting Internet message headers" in [EWS, MIME, and the missing Internet message headers](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeaders>
   <InternetMessageHeader/>
</InternetMessageHeaders>
```

 <span data-ttu-id="e1cfe-109">**NonEmptyArrayOfInternetHeadersType**</span><span class="sxs-lookup"><span data-stu-id="e1cfe-109">**NonEmptyArrayOfInternetHeadersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1cfe-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e1cfe-110">Attributes and elements</span></span>

<span data-ttu-id="e1cfe-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1cfe-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="e1cfe-112">Attributes</span></span>

<span data-ttu-id="e1cfe-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1cfe-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1cfe-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e1cfe-114">Child elements</span></span>

|<span data-ttu-id="e1cfe-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e1cfe-115">**Element**</span></span>|<span data-ttu-id="e1cfe-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1cfe-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1cfe-117">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="e1cfe-117">InternetMessageHeader</span></span>](internetmessageheader.md) <br/> |<span data-ttu-id="e1cfe-118">Representa o cabeçalho da mensagem da Internet para um determinado cabeçalho dentro da coleção Headers.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-118">Represents the Internet message header for a given header within the headers collection.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e1cfe-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e1cfe-119">Parent elements</span></span>

|<span data-ttu-id="e1cfe-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e1cfe-120">**Element**</span></span>|<span data-ttu-id="e1cfe-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1cfe-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1cfe-122">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="e1cfe-122">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="e1cfe-123">Representa uma resposta de aceitação para uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-123">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="e1cfe-124">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="e1cfe-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e1cfe-125">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="e1cfe-126">Contato</span><span class="sxs-lookup"><span data-stu-id="e1cfe-126">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="e1cfe-127">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-127">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="e1cfe-128">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="e1cfe-128">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="e1cfe-129">Representa uma resposta de recusa a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-129">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="e1cfe-130">DistributionList</span><span class="sxs-lookup"><span data-stu-id="e1cfe-130">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="e1cfe-131">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-131">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="e1cfe-132">Item</span><span class="sxs-lookup"><span data-stu-id="e1cfe-132">Item</span></span>](item.md) <br/> |<span data-ttu-id="e1cfe-133">Representa um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-133">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e1cfe-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="e1cfe-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="e1cfe-135">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-135">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e1cfe-136">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="e1cfe-136">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="e1cfe-137">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-137">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e1cfe-138">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="e1cfe-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e1cfe-139">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e1cfe-140">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="e1cfe-140">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="e1cfe-141">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-141">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e1cfe-142">Message</span><span class="sxs-lookup"><span data-stu-id="e1cfe-142">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e1cfe-143">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-143">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="e1cfe-144">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="e1cfe-144">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="e1cfe-145">Remove um item do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-145">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e1cfe-146">Tarefa</span><span class="sxs-lookup"><span data-stu-id="e1cfe-146">Task</span></span>](task.md) <br/> |<span data-ttu-id="e1cfe-147">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-147">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e1cfe-148">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="e1cfe-148">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="e1cfe-149">Representa uma resposta provisoriamente aceita a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-149">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e1cfe-150">Comentários</span><span class="sxs-lookup"><span data-stu-id="e1cfe-150">Remarks</span></span>

<span data-ttu-id="e1cfe-151">A seguir está a definição da propriedade estendida da API gerenciada do EWS para a propriedade **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="e1cfe-151">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="e1cfe-152">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1cfe-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1cfe-153">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e1cfe-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1cfe-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="e1cfe-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e1cfe-155">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e1cfe-155">Schema Name</span></span>  <br/> |<span data-ttu-id="e1cfe-156">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e1cfe-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="e1cfe-157">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e1cfe-157">Validation File</span></span>  <br/> |<span data-ttu-id="e1cfe-158">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e1cfe-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e1cfe-159">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e1cfe-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="e1cfe-160">False</span><span class="sxs-lookup"><span data-stu-id="e1cfe-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1cfe-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="e1cfe-161">See also</span></span>



- [<span data-ttu-id="e1cfe-162">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e1cfe-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="e1cfe-163">EWS, MIME e os cabeçalhos de mensagem da Internet ausentes</span><span class="sxs-lookup"><span data-stu-id="e1cfe-163">EWS, MIME, and the missing Internet message headers</span></span>](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

