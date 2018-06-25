---
title: Remetente
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Sender
api_type:
- schema
ms.assetid: 26d1a46e-e1d3-44b8-a02d-fa6f83aa5cda
description: O elemento de remetente identifica o remetente de um item.
ms.openlocfilehash: a7b06543fadd7cf7ae05f7ae8f86122138e11076
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825323"
---
# <a name="sender"></a><span data-ttu-id="84411-103">Remetente</span><span class="sxs-lookup"><span data-stu-id="84411-103">Sender</span></span>

<span data-ttu-id="84411-104">O elemento de **remetente** identifica o remetente de um item.</span><span class="sxs-lookup"><span data-stu-id="84411-104">The **Sender** element identifies the sender of an item.</span></span> 
  
```xml
<Sender>
   <Mailbox/>
</Sender>
```

 <span data-ttu-id="84411-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="84411-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="84411-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="84411-106">Attributes and elements</span></span>

<span data-ttu-id="84411-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="84411-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="84411-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="84411-108">Attributes</span></span>

<span data-ttu-id="84411-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="84411-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="84411-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="84411-110">Child elements</span></span>

|<span data-ttu-id="84411-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="84411-111">**Element**</span></span>|<span data-ttu-id="84411-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="84411-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="84411-113">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="84411-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="84411-114">Identifica um objeto do Active Directory habilitado para email que identifique o remetente.</span><span class="sxs-lookup"><span data-stu-id="84411-114">Identifies a mail enabled Active Directory object that identifies the sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="84411-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="84411-115">Parent elements</span></span>

|<span data-ttu-id="84411-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="84411-116">**Element**</span></span>|<span data-ttu-id="84411-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="84411-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="84411-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="84411-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="84411-119">Remove um item de armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="84411-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="84411-120">Mensagem</span><span class="sxs-lookup"><span data-stu-id="84411-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="84411-121">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="84411-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="84411-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="84411-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="84411-123">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="84411-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="84411-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="84411-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="84411-125">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="84411-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="84411-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="84411-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="84411-127">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="84411-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="84411-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="84411-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="84411-129">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="84411-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="84411-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="84411-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="84411-131">Representa uma resposta de aceitar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="84411-131">Represents an accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="84411-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="84411-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="84411-133">Representa uma resposta provisoriamente aceita para uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="84411-133">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="84411-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="84411-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="84411-135">Representa uma resposta recusar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="84411-135">Represents a decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="84411-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="84411-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="84411-137">Contém uma resposta para o criador de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="84411-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="84411-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="84411-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="84411-139">Contém uma resposta a todos os destinatários identificados de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="84411-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="84411-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="84411-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="84411-141">Contém um item de armazenamento do Exchange para encaminhar para destinatários.</span><span class="sxs-lookup"><span data-stu-id="84411-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="84411-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="84411-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="84411-143">Representa o objeto de resposta usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="84411-143">Represents the response object used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="84411-144">PostItem</span><span class="sxs-lookup"><span data-stu-id="84411-144">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="84411-145">Representa um item de postagem no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="84411-145">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="84411-146">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="84411-146">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="84411-147">Comentários</span><span class="sxs-lookup"><span data-stu-id="84411-147">Remarks</span></span>

<span data-ttu-id="84411-148">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="84411-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="84411-149">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="84411-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84411-150">Namespace</span><span class="sxs-lookup"><span data-stu-id="84411-150">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="84411-151">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="84411-151">Schema Name</span></span>  <br/> |<span data-ttu-id="84411-152">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="84411-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="84411-153">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="84411-153">Validation File</span></span>  <br/> |<span data-ttu-id="84411-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="84411-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="84411-155">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="84411-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="84411-156">False</span><span class="sxs-lookup"><span data-stu-id="84411-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="84411-157">Ver também</span><span class="sxs-lookup"><span data-stu-id="84411-157">See also</span></span>



- [<span data-ttu-id="84411-158">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="84411-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

