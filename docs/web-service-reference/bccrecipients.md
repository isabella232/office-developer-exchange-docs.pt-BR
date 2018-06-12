---
title: BccRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BccRecipients
api_type:
- schema
ms.assetid: c4e05168-d36b-4740-a526-4b7da53553c1
description: O elemento BccRecipients representa uma coleção de destinatários para receber uma cópia carbono oculta (Cco) de uma mensagem de email.
ms.openlocfilehash: 858fe74c32cb7d1ed624888c06bba4ffe09d489e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751263"
---
# <a name="bccrecipients"></a><span data-ttu-id="b6b39-103">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="b6b39-103">BccRecipients</span></span>

<span data-ttu-id="b6b39-104">O elemento **BccRecipients** representa uma coleção de destinatários para receber uma cópia carbono oculta (Cco) de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="b6b39-104">The **BccRecipients** element represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span> 
  
```xml
<BccRecipients>
   <Mailbox/>
</BccRecipients>
```

 <span data-ttu-id="b6b39-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="b6b39-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6b39-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b6b39-106">Attributes and elements</span></span>

<span data-ttu-id="b6b39-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b6b39-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6b39-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b6b39-108">Attributes</span></span>

<span data-ttu-id="b6b39-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b6b39-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6b39-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b6b39-110">Child elements</span></span>

|<span data-ttu-id="b6b39-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b6b39-111">**Element**</span></span>|<span data-ttu-id="b6b39-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b6b39-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6b39-113">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="b6b39-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="b6b39-114">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="b6b39-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b6b39-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b6b39-115">Parent elements</span></span>

|<span data-ttu-id="b6b39-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b6b39-116">**Element**</span></span>|<span data-ttu-id="b6b39-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b6b39-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6b39-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="b6b39-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="b6b39-119">Remove um item de armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6b39-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b6b39-120">Mensagem</span><span class="sxs-lookup"><span data-stu-id="b6b39-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b6b39-121">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6b39-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="b6b39-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="b6b39-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="b6b39-123">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6b39-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b6b39-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b6b39-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b6b39-125">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6b39-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b6b39-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b6b39-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="b6b39-127">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6b39-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b6b39-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="b6b39-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="b6b39-129">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6b39-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b6b39-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="b6b39-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="b6b39-131">Representa uma resposta de aceitar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="b6b39-131">Represents an accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="b6b39-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="b6b39-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="b6b39-133">Representa uma resposta provisoriamente aceita para uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="b6b39-133">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="b6b39-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="b6b39-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="b6b39-135">Representa uma resposta recusar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="b6b39-135">Represents a decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="b6b39-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="b6b39-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="b6b39-137">Contém uma resposta para o criador de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6b39-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b6b39-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="b6b39-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="b6b39-139">Contém uma resposta a todos os destinatários identificados de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6b39-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b6b39-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="b6b39-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="b6b39-141">Contém um item de armazenamento do Exchange para encaminhar para destinatários.</span><span class="sxs-lookup"><span data-stu-id="b6b39-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="b6b39-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="b6b39-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="b6b39-143">Representa o objeto de resposta é usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="b6b39-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b6b39-144">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="b6b39-144">Remarks</span></span>

<span data-ttu-id="b6b39-145">Você não pode obter **BccRecipients** usando uma solicitação FindItem.</span><span class="sxs-lookup"><span data-stu-id="b6b39-145">You cannot get **BccRecipients** by using a FindItem request.</span></span> <span data-ttu-id="b6b39-146">Use uma solicitação de GetItem para obter **BccRecipients**.</span><span class="sxs-lookup"><span data-stu-id="b6b39-146">Use a GetItem request to get **BccRecipients**.</span></span>
  
<span data-ttu-id="b6b39-147">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="b6b39-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6b39-148">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b6b39-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6b39-149">Namespace</span><span class="sxs-lookup"><span data-stu-id="b6b39-149">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b6b39-150">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b6b39-150">Schema Name</span></span>  <br/> |<span data-ttu-id="b6b39-151">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b6b39-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="b6b39-152">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b6b39-152">Validation File</span></span>  <br/> |<span data-ttu-id="b6b39-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b6b39-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b6b39-154">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b6b39-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="b6b39-155">False</span><span class="sxs-lookup"><span data-stu-id="b6b39-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b6b39-156">Ver também</span><span class="sxs-lookup"><span data-stu-id="b6b39-156">See also</span></span>



- [<span data-ttu-id="b6b39-157">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b6b39-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

