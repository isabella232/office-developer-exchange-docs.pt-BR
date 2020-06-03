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
description: O elemento Sender identifica o remetente de um item.
ms.openlocfilehash: f056fefdd5c5832d4b5bf20416e07e376f6a03de
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530576"
---
# <a name="sender"></a><span data-ttu-id="9fa6e-103">Remetente</span><span class="sxs-lookup"><span data-stu-id="9fa6e-103">Sender</span></span>

<span data-ttu-id="9fa6e-104">O elemento **Sender** identifica o remetente de um item.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-104">The **Sender** element identifies the sender of an item.</span></span> 
  
```xml
<Sender>
   <Mailbox/>
</Sender>
```

 <span data-ttu-id="9fa6e-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="9fa6e-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9fa6e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9fa6e-106">Attributes and elements</span></span>

<span data-ttu-id="9fa6e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9fa6e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9fa6e-108">Attributes</span></span>

<span data-ttu-id="9fa6e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9fa6e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9fa6e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9fa6e-110">Child elements</span></span>

|<span data-ttu-id="9fa6e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9fa6e-111">**Element**</span></span>|<span data-ttu-id="9fa6e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9fa6e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fa6e-113">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="9fa6e-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="9fa6e-114">Identifica um objeto do Active Directory habilitado para email que identifica o remetente.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-114">Identifies a mail enabled Active Directory object that identifies the sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9fa6e-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9fa6e-115">Parent elements</span></span>

|<span data-ttu-id="9fa6e-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9fa6e-116">**Element**</span></span>|<span data-ttu-id="9fa6e-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9fa6e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fa6e-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="9fa6e-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="9fa6e-119">Remove um item do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9fa6e-120">Mensagem</span><span class="sxs-lookup"><span data-stu-id="9fa6e-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9fa6e-121">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="9fa6e-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="9fa6e-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="9fa6e-123">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9fa6e-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="9fa6e-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="9fa6e-125">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9fa6e-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="9fa6e-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="9fa6e-127">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9fa6e-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="9fa6e-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="9fa6e-129">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9fa6e-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="9fa6e-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="9fa6e-131">Representa uma resposta de aceitação para uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-131">Represents an accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="9fa6e-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="9fa6e-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="9fa6e-133">Representa uma resposta provisoriamente aceita a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-133">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="9fa6e-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="9fa6e-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="9fa6e-135">Representa uma resposta de recusa a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-135">Represents a decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="9fa6e-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="9fa6e-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="9fa6e-137">Contém uma resposta para o criador de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9fa6e-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="9fa6e-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="9fa6e-139">Contém uma resposta a todos os destinatários identificados de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9fa6e-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="9fa6e-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="9fa6e-141">Contém um item de repositório do Exchange para encaminhar aos destinatários.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="9fa6e-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="9fa6e-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="9fa6e-143">Representa o objeto Response usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-143">Represents the response object used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="9fa6e-144">Item de postagem</span><span class="sxs-lookup"><span data-stu-id="9fa6e-144">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="9fa6e-145">Representa um item de postagem no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-145">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="9fa6e-146">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9fa6e-146">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9fa6e-147">Comentários</span><span class="sxs-lookup"><span data-stu-id="9fa6e-147">Remarks</span></span>

<span data-ttu-id="9fa6e-148">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="9fa6e-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9fa6e-149">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9fa6e-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9fa6e-150">Namespace</span><span class="sxs-lookup"><span data-stu-id="9fa6e-150">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9fa6e-151">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9fa6e-151">Schema Name</span></span>  <br/> |<span data-ttu-id="9fa6e-152">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9fa6e-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="9fa6e-153">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9fa6e-153">Validation File</span></span>  <br/> |<span data-ttu-id="9fa6e-154">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9fa6e-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9fa6e-155">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9fa6e-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="9fa6e-156">False</span><span class="sxs-lookup"><span data-stu-id="9fa6e-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9fa6e-157">Confira também</span><span class="sxs-lookup"><span data-stu-id="9fa6e-157">See also</span></span>



- [<span data-ttu-id="9fa6e-158">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9fa6e-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

