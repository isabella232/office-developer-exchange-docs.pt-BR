---
title: ToRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ToRecipients
api_type:
- schema
ms.assetid: 72dc3be8-30bb-4ae1-acf4-fb94ff490631
description: O elemento ToRecipients contém uma matriz de destinatários de um item. Estes são os principais destinatários de um item.
ms.openlocfilehash: 39ee359e1eaf3d0b6455fb1734222e78054dc7f3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467540"
---
# <a name="torecipients"></a><span data-ttu-id="1633c-104">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="1633c-104">ToRecipients</span></span>

<span data-ttu-id="1633c-105">O elemento **ToRecipients** contém uma matriz de destinatários de um item.</span><span class="sxs-lookup"><span data-stu-id="1633c-105">The **ToRecipients** element contains an array of recipients of an item.</span></span> <span data-ttu-id="1633c-106">Estes são os principais destinatários de um item.</span><span class="sxs-lookup"><span data-stu-id="1633c-106">These are the primary recipients of an item.</span></span> 
  
```xml
<ToRecipients>
   <Mailbox/>
</ToRecipients>
```

 <span data-ttu-id="1633c-107">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="1633c-107">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1633c-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1633c-108">Attributes and elements</span></span>

<span data-ttu-id="1633c-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1633c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1633c-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="1633c-110">Attributes</span></span>

<span data-ttu-id="1633c-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1633c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1633c-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1633c-112">Child elements</span></span>

|<span data-ttu-id="1633c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1633c-113">**Element**</span></span>|<span data-ttu-id="1633c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1633c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1633c-115">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="1633c-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="1633c-116">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="1633c-116">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1633c-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1633c-117">Parent elements</span></span>

|<span data-ttu-id="1633c-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1633c-118">**Element**</span></span>|<span data-ttu-id="1633c-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1633c-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1633c-120">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="1633c-120">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="1633c-121">Remove um item do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1633c-121">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1633c-122">Message</span><span class="sxs-lookup"><span data-stu-id="1633c-122">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1633c-123">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1633c-123">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="1633c-124">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="1633c-124">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="1633c-125">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1633c-125">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1633c-126">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="1633c-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="1633c-127">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1633c-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1633c-128">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="1633c-128">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="1633c-129">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1633c-129">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1633c-130">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="1633c-130">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="1633c-131">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1633c-131">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1633c-132">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="1633c-132">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="1633c-133">Representa uma resposta de aceitação para uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="1633c-133">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="1633c-134">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="1633c-134">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="1633c-135">Representa uma resposta provisória a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="1633c-135">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="1633c-136">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="1633c-136">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="1633c-137">Representa uma resposta de recusa a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="1633c-137">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="1633c-138">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="1633c-138">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="1633c-139">Contém uma resposta para o criador de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1633c-139">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1633c-140">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="1633c-140">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="1633c-141">Contém uma resposta a todos os destinatários identificados de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1633c-141">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1633c-142">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="1633c-142">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="1633c-143">Contém um item de repositório do Exchange para encaminhar aos destinatários.</span><span class="sxs-lookup"><span data-stu-id="1633c-143">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="1633c-144">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="1633c-144">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="1633c-145">Representa o objeto Response que é usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="1633c-145">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1633c-146">Comentários</span><span class="sxs-lookup"><span data-stu-id="1633c-146">Remarks</span></span>

<span data-ttu-id="1633c-147">Não é possível obter todos os **destinatários** usando uma solicitação FindItem.</span><span class="sxs-lookup"><span data-stu-id="1633c-147">You cannot get **ToRecipients** by using a FindItem request.</span></span> <span data-ttu-id="1633c-148">Use uma solicitação GetItem para obter o **ToRecipients**.</span><span class="sxs-lookup"><span data-stu-id="1633c-148">Use a GetItem request to get the **ToRecipients**.</span></span>
  
<span data-ttu-id="1633c-149">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="1633c-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1633c-150">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1633c-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1633c-151">Namespace</span><span class="sxs-lookup"><span data-stu-id="1633c-151">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1633c-152">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1633c-152">Schema Name</span></span>  <br/> |<span data-ttu-id="1633c-153">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1633c-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="1633c-154">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1633c-154">Validation File</span></span>  <br/> |<span data-ttu-id="1633c-155">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1633c-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1633c-156">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1633c-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="1633c-157">False</span><span class="sxs-lookup"><span data-stu-id="1633c-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1633c-158">Confira também</span><span class="sxs-lookup"><span data-stu-id="1633c-158">See also</span></span>



- [<span data-ttu-id="1633c-159">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1633c-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

