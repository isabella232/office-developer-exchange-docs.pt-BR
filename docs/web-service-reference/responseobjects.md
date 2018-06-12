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
description: O elemento ResponseObjects contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.
ms.openlocfilehash: b1d95063439f5089665d2aad97d747665caef0ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825197"
---
# <a name="responseobjects"></a><span data-ttu-id="3821d-103">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="3821d-103">ResponseObjects</span></span>

<span data-ttu-id="3821d-104">O elemento **ResponseObjects** contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3821d-104">The **ResponseObjects** element contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="3821d-105">**NonEmptyArrayOfResponseObjectsType**</span><span class="sxs-lookup"><span data-stu-id="3821d-105">**NonEmptyArrayOfResponseObjectsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3821d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3821d-106">Attributes and elements</span></span>

<span data-ttu-id="3821d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3821d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3821d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3821d-108">Attributes</span></span>

<span data-ttu-id="3821d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3821d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3821d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3821d-110">Child elements</span></span>

|<span data-ttu-id="3821d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3821d-111">**Element**</span></span>|<span data-ttu-id="3821d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3821d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3821d-113">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="3821d-113">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="3821d-114">Representa uma resposta de aceitar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="3821d-114">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="3821d-115">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="3821d-115">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="3821d-116">Representa um provisório responde a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="3821d-116">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="3821d-117">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="3821d-117">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="3821d-118">Representa uma resposta recusar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="3821d-118">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="3821d-119">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="3821d-119">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="3821d-120">Contém uma resposta para o criador de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3821d-120">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3821d-121">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="3821d-121">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="3821d-122">Contém um item de armazenamento do Exchange para encaminhar para destinatários.</span><span class="sxs-lookup"><span data-stu-id="3821d-122">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="3821d-123">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="3821d-123">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="3821d-124">Contém uma resposta a todos os destinatários identificados de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3821d-124">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3821d-125">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="3821d-125">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="3821d-126">Representa o objeto de resposta usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="3821d-126">Represents the response object used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="3821d-127">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="3821d-127">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="3821d-128">Remove um item de armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3821d-128">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3821d-129">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="3821d-129">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="3821d-130">Contém uma resposta para um item de postagem.</span><span class="sxs-lookup"><span data-stu-id="3821d-130">Contains a reply to a post item.</span></span> <span data-ttu-id="3821d-131">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3821d-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="3821d-132">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="3821d-132">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="3821d-133">Usado para suprimir as solicitações de confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="3821d-133">Used to suppress read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="3821d-134">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="3821d-134">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="3821d-135">Usado para aceitar um convite que permite o acesso aos dados de contatos ou de calendário de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="3821d-135">Used to accept an invitation that allows access to another user's calendar or contacts data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3821d-136">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3821d-136">Parent elements</span></span>

|<span data-ttu-id="3821d-137">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3821d-137">**Element**</span></span>|<span data-ttu-id="3821d-138">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3821d-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3821d-139">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="3821d-139">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="3821d-140">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3821d-140">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3821d-141">Contato</span><span class="sxs-lookup"><span data-stu-id="3821d-141">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="3821d-142">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3821d-142">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="3821d-143">DistributionList</span><span class="sxs-lookup"><span data-stu-id="3821d-143">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="3821d-144">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="3821d-144">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="3821d-145">1.1</span><span class="sxs-lookup"><span data-stu-id="3821d-145">Item</span></span>](item.md) <br/> |<span data-ttu-id="3821d-146">Representa um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3821d-146">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3821d-147">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="3821d-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="3821d-148">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3821d-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3821d-149">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="3821d-149">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="3821d-150">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3821d-150">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3821d-151">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3821d-151">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3821d-152">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3821d-152">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3821d-153">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="3821d-153">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="3821d-154">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3821d-154">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3821d-155">Mensagem</span><span class="sxs-lookup"><span data-stu-id="3821d-155">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3821d-156">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3821d-156">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="3821d-157">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="3821d-157">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="3821d-158">Remove um item de armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3821d-158">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3821d-159">Task</span><span class="sxs-lookup"><span data-stu-id="3821d-159">Task</span></span>](task.md) <br/> |<span data-ttu-id="3821d-160">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3821d-160">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3821d-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="3821d-161">Remarks</span></span>

<span data-ttu-id="3821d-162">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3821d-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3821d-163">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3821d-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3821d-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="3821d-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3821d-165">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3821d-165">Schema Name</span></span>  <br/> |<span data-ttu-id="3821d-166">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3821d-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="3821d-167">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3821d-167">Validation File</span></span>  <br/> |<span data-ttu-id="3821d-168">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3821d-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3821d-169">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3821d-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="3821d-170">False</span><span class="sxs-lookup"><span data-stu-id="3821d-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3821d-171">Ver também</span><span class="sxs-lookup"><span data-stu-id="3821d-171">See also</span></span>



- [<span data-ttu-id="3821d-172">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3821d-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

