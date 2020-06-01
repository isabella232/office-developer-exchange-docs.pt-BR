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
description: O elemento ResponseObjects contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.
ms.openlocfilehash: 675bfda4addb38535736efc0c790577ff4739108
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457435"
---
# <a name="responseobjects"></a><span data-ttu-id="67b66-103">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="67b66-103">ResponseObjects</span></span>

<span data-ttu-id="67b66-104">O elemento **ResponseObjects** contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b66-104">The **ResponseObjects** element contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span> 
  
```XML
<ResponseObjects>
   <AcceptItem/>
   <TentativelyAcceptItem/>
   <DeclineItem/>
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

 <span data-ttu-id="67b66-105">**NonEmptyArrayOfResponseObjectsType**</span><span class="sxs-lookup"><span data-stu-id="67b66-105">**NonEmptyArrayOfResponseObjectsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="67b66-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="67b66-106">Attributes and elements</span></span>

<span data-ttu-id="67b66-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="67b66-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67b66-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="67b66-108">Attributes</span></span>

<span data-ttu-id="67b66-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="67b66-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="67b66-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="67b66-110">Child elements</span></span>

|<span data-ttu-id="67b66-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="67b66-111">**Element**</span></span>|<span data-ttu-id="67b66-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="67b66-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67b66-113">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="67b66-113">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="67b66-114">Representa uma resposta de aceitação para uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="67b66-114">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="67b66-115">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="67b66-115">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="67b66-116">Representa uma resposta provisória a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="67b66-116">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="67b66-117">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="67b66-117">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="67b66-118">Representa uma resposta de recusa a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="67b66-118">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="67b66-119">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="67b66-119">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="67b66-120">Contém uma resposta para o criador de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b66-120">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="67b66-121">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="67b66-121">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="67b66-122">Contém um item de repositório do Exchange para encaminhar aos destinatários.</span><span class="sxs-lookup"><span data-stu-id="67b66-122">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="67b66-123">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="67b66-123">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="67b66-124">Contém uma resposta a todos os destinatários identificados de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b66-124">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="67b66-125">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="67b66-125">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="67b66-126">Representa o objeto Response usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="67b66-126">Represents the response object used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="67b66-127">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="67b66-127">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="67b66-128">Remove um item do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b66-128">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="67b66-129">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="67b66-129">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="67b66-130">Contém uma resposta a um item de postagem.</span><span class="sxs-lookup"><span data-stu-id="67b66-130">Contains a reply to a post item.</span></span> <span data-ttu-id="67b66-131">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="67b66-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="67b66-132">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="67b66-132">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="67b66-133">Usado para suprimir solicitações de confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="67b66-133">Used to suppress read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="67b66-134">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="67b66-134">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="67b66-135">Usado para aceitar um convite que permite o acesso a dados do calendário ou contatos de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="67b66-135">Used to accept an invitation that allows access to another user's calendar or contacts data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="67b66-136">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="67b66-136">Parent elements</span></span>

|<span data-ttu-id="67b66-137">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="67b66-137">**Element**</span></span>|<span data-ttu-id="67b66-138">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="67b66-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67b66-139">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="67b66-139">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="67b66-140">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b66-140">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="67b66-141">Contato</span><span class="sxs-lookup"><span data-stu-id="67b66-141">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="67b66-142">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b66-142">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="67b66-143">DistributionList</span><span class="sxs-lookup"><span data-stu-id="67b66-143">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="67b66-144">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="67b66-144">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="67b66-145">Item</span><span class="sxs-lookup"><span data-stu-id="67b66-145">Item</span></span>](item.md) <br/> |<span data-ttu-id="67b66-146">Representa um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b66-146">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="67b66-147">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="67b66-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="67b66-148">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b66-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="67b66-149">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="67b66-149">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="67b66-150">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b66-150">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="67b66-151">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="67b66-151">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="67b66-152">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b66-152">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="67b66-153">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="67b66-153">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="67b66-154">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b66-154">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="67b66-155">Message</span><span class="sxs-lookup"><span data-stu-id="67b66-155">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="67b66-156">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b66-156">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="67b66-157">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="67b66-157">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="67b66-158">Remove um item do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b66-158">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="67b66-159">Tarefa</span><span class="sxs-lookup"><span data-stu-id="67b66-159">Task</span></span>](task.md) <br/> |<span data-ttu-id="67b66-160">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b66-160">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="67b66-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="67b66-161">Remarks</span></span>

<span data-ttu-id="67b66-162">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b66-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="67b66-163">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="67b66-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67b66-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="67b66-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="67b66-165">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="67b66-165">Schema Name</span></span>  <br/> |<span data-ttu-id="67b66-166">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="67b66-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="67b66-167">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="67b66-167">Validation File</span></span>  <br/> |<span data-ttu-id="67b66-168">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="67b66-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="67b66-169">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="67b66-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="67b66-170">False</span><span class="sxs-lookup"><span data-stu-id="67b66-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="67b66-171">Confira também</span><span class="sxs-lookup"><span data-stu-id="67b66-171">See also</span></span>



- [<span data-ttu-id="67b66-172">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="67b66-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

