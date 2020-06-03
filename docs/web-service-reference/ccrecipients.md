---
title: CcRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CcRecipients
api_type:
- schema
ms.assetid: 5c20ec3a-0bee-4e67-b220-586ed0d601c9
description: O elemento CcRecipients representa uma coleção de destinatários que receberá uma cópia da mensagem.
ms.openlocfilehash: 57d0e2d3b2c44fbd7bb30696002b27e83d1e274e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462203"
---
# <a name="ccrecipients"></a><span data-ttu-id="c72c0-103">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="c72c0-103">CcRecipients</span></span>

<span data-ttu-id="c72c0-104">O elemento **CcRecipients** representa uma coleção de destinatários que receberá uma cópia da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c72c0-104">The **CcRecipients** element represents a collection of recipients that will receive a copy of the message.</span></span> 
  
```xml
<CcRecipients>
   <Mailbox/>
</CcRecipients>
```

 <span data-ttu-id="c72c0-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="c72c0-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c72c0-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c72c0-106">Attributes and elements</span></span>

<span data-ttu-id="c72c0-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c72c0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c72c0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c72c0-108">Attributes</span></span>

<span data-ttu-id="c72c0-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c72c0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c72c0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c72c0-110">Child elements</span></span>

|<span data-ttu-id="c72c0-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c72c0-111">**Element**</span></span>|<span data-ttu-id="c72c0-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c72c0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c72c0-113">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="c72c0-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="c72c0-114">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="c72c0-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c72c0-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c72c0-115">Parent elements</span></span>

|<span data-ttu-id="c72c0-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c72c0-116">**Element**</span></span>|<span data-ttu-id="c72c0-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c72c0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c72c0-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="c72c0-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="c72c0-119">Remove um item do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c72c0-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c72c0-120">Mensagem</span><span class="sxs-lookup"><span data-stu-id="c72c0-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c72c0-121">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c72c0-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="c72c0-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="c72c0-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="c72c0-123">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c72c0-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c72c0-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c72c0-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c72c0-125">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c72c0-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c72c0-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="c72c0-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="c72c0-127">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c72c0-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c72c0-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="c72c0-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="c72c0-129">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c72c0-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c72c0-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="c72c0-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="c72c0-131">Representa uma resposta de aceitação para uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="c72c0-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="c72c0-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="c72c0-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="c72c0-133">Representa uma resposta provisória a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="c72c0-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="c72c0-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="c72c0-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="c72c0-135">Representa uma resposta de recusa a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="c72c0-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="c72c0-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="c72c0-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="c72c0-137">Contém uma resposta para o criador de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c72c0-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c72c0-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="c72c0-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="c72c0-139">Contém uma resposta a todos os destinatários identificados de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c72c0-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c72c0-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="c72c0-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="c72c0-141">Contém um item de repositório do Exchange para encaminhar aos destinatários.</span><span class="sxs-lookup"><span data-stu-id="c72c0-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="c72c0-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="c72c0-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="c72c0-143">Representa o objeto Response que é usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="c72c0-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c72c0-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="c72c0-144">Remarks</span></span>

<span data-ttu-id="c72c0-145">Você não pode obter **CcRecipients** usando uma solicitação FindItem.</span><span class="sxs-lookup"><span data-stu-id="c72c0-145">You cannot get **CcRecipients** by using a FindItem request.</span></span> <span data-ttu-id="c72c0-146">Use uma solicitação GetItem para obter o **CcRecipients**.</span><span class="sxs-lookup"><span data-stu-id="c72c0-146">Use a GetItem request to get **CcRecipients**.</span></span>
  
<span data-ttu-id="c72c0-147">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c72c0-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c72c0-148">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c72c0-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c72c0-149">Namespace</span><span class="sxs-lookup"><span data-stu-id="c72c0-149">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c72c0-150">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c72c0-150">Schema Name</span></span>  <br/> |<span data-ttu-id="c72c0-151">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c72c0-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="c72c0-152">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c72c0-152">Validation File</span></span>  <br/> |<span data-ttu-id="c72c0-153">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c72c0-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c72c0-154">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c72c0-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="c72c0-155">False</span><span class="sxs-lookup"><span data-stu-id="c72c0-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c72c0-156">Confira também</span><span class="sxs-lookup"><span data-stu-id="c72c0-156">See also</span></span>



- [<span data-ttu-id="c72c0-157">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c72c0-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

