---
title: De
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- From
api_type:
- schema
ms.assetid: 5a52d644-3677-4049-874c-12bd5c3080dc
description: O elemento From representa o endereço do qual a mensagem foi enviada.
ms.openlocfilehash: 39c8c8ef84ff445e8f44ebb9f2285ccfc42353a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752380"
---
# <a name="from"></a><span data-ttu-id="8de3b-103">De</span><span class="sxs-lookup"><span data-stu-id="8de3b-103">From</span></span>

<span data-ttu-id="8de3b-104">O elemento **de** representa o endereço do qual a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="8de3b-104">The **From** element represents the address from which the message was sent.</span></span> 
  
```xml
<From>
   <Mailbox/>
</From>
```

 <span data-ttu-id="8de3b-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="8de3b-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8de3b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8de3b-106">Attributes and elements</span></span>

<span data-ttu-id="8de3b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8de3b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8de3b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8de3b-108">Attributes</span></span>

<span data-ttu-id="8de3b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8de3b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8de3b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8de3b-110">Child elements</span></span>

|<span data-ttu-id="8de3b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8de3b-111">**Element**</span></span>|<span data-ttu-id="8de3b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8de3b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8de3b-113">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="8de3b-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="8de3b-114">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="8de3b-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8de3b-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8de3b-115">Parent elements</span></span>

|<span data-ttu-id="8de3b-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8de3b-116">**Element**</span></span>|<span data-ttu-id="8de3b-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8de3b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8de3b-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="8de3b-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="8de3b-119">Remove um item de armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8de3b-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8de3b-120">Mensagem</span><span class="sxs-lookup"><span data-stu-id="8de3b-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8de3b-121">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8de3b-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="8de3b-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="8de3b-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="8de3b-123">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8de3b-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8de3b-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8de3b-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="8de3b-125">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8de3b-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8de3b-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="8de3b-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="8de3b-127">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8de3b-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8de3b-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="8de3b-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="8de3b-129">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8de3b-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8de3b-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="8de3b-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="8de3b-131">Representa uma resposta de aceitar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="8de3b-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="8de3b-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="8de3b-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="8de3b-133">Representa um provisório responde a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="8de3b-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="8de3b-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="8de3b-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="8de3b-135">Representa uma resposta recusar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="8de3b-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="8de3b-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="8de3b-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="8de3b-137">Contém uma resposta para o criador de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8de3b-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8de3b-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="8de3b-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="8de3b-139">Contém uma resposta a todos os destinatários identificados de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8de3b-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8de3b-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="8de3b-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="8de3b-141">Contém um item de armazenamento do Exchange para encaminhar para destinatários.</span><span class="sxs-lookup"><span data-stu-id="8de3b-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="8de3b-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="8de3b-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="8de3b-143">Representa o objeto de resposta é usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="8de3b-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="8de3b-144">PostItem</span><span class="sxs-lookup"><span data-stu-id="8de3b-144">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="8de3b-145">Representa um item de postagem no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8de3b-145">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="8de3b-146">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8de3b-146">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8de3b-147">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="8de3b-147">Remarks</span></span>

<span data-ttu-id="8de3b-148">Esse elemento é usado para emails "Enviar em nome de".</span><span class="sxs-lookup"><span data-stu-id="8de3b-148">This element is used for "send on behalf of" e-mails.</span></span>
  
<span data-ttu-id="8de3b-149">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="8de3b-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8de3b-150">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8de3b-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8de3b-151">Namespace</span><span class="sxs-lookup"><span data-stu-id="8de3b-151">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8de3b-152">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8de3b-152">Schema Name</span></span>  <br/> |<span data-ttu-id="8de3b-153">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8de3b-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="8de3b-154">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8de3b-154">Validation File</span></span>  <br/> |<span data-ttu-id="8de3b-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8de3b-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8de3b-156">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8de3b-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="8de3b-157">False</span><span class="sxs-lookup"><span data-stu-id="8de3b-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8de3b-158">Ver também</span><span class="sxs-lookup"><span data-stu-id="8de3b-158">See also</span></span>



- [<span data-ttu-id="8de3b-159">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8de3b-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

