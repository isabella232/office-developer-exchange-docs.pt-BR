---
title: CancelCalendarItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CancelCalendarItem
api_type:
- schema
ms.assetid: a2046402-a176-44d5-b4b3-adb696581935
description: O elemento CancelCalendarItem representa o objeto Response que é usado para cancelar uma reunião.
ms.openlocfilehash: 45ad76d19bd43e2081aa9b9eb63547e091014803
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462252"
---
# <a name="cancelcalendaritem"></a><span data-ttu-id="17fba-103">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="17fba-103">CancelCalendarItem</span></span>

<span data-ttu-id="17fba-104">O elemento **CancelCalendarItem** representa o objeto Response que é usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="17fba-104">The **CancelCalendarItem** element represents the response object that is used to cancel a meeting.</span></span> 
  
```xml
<CancelCalendarItem>
   <Subject/>
   <Body/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ReferenceItemId/>
   <NewBodyContent/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
</CancelCalendarItem>
```

 <span data-ttu-id="17fba-105">**CancelCalendarItemType**</span><span class="sxs-lookup"><span data-stu-id="17fba-105">**CancelCalendarItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17fba-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="17fba-106">Attributes and elements</span></span>

<span data-ttu-id="17fba-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="17fba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17fba-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="17fba-108">Attributes</span></span>

<span data-ttu-id="17fba-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="17fba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17fba-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="17fba-110">Child elements</span></span>

|<span data-ttu-id="17fba-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="17fba-111">**Element**</span></span>|<span data-ttu-id="17fba-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="17fba-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17fba-113">Assunto</span><span class="sxs-lookup"><span data-stu-id="17fba-113">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="17fba-114">Representa a propriedade Subject dos itens do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="17fba-114">Represents the subject property of Exchange store items.</span></span>  <br/> |
|[<span data-ttu-id="17fba-115">Body</span><span class="sxs-lookup"><span data-stu-id="17fba-115">Body</span></span>](body.md) <br/> |<span data-ttu-id="17fba-116">Não usado pelo **CancelCalendarItem**.</span><span class="sxs-lookup"><span data-stu-id="17fba-116">Not used by **CancelCalendarItem**.</span></span> <span data-ttu-id="17fba-117">Use a propriedade [NewBodyContent](newbodycontent.md) para definir o conteúdo do corpo.</span><span class="sxs-lookup"><span data-stu-id="17fba-117">Use the [NewBodyContent](newbodycontent.md) property to set the body content.</span></span>  <br/> |
|[<span data-ttu-id="17fba-118">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="17fba-118">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="17fba-119">Contém um conjunto de destinatários de um item.</span><span class="sxs-lookup"><span data-stu-id="17fba-119">Contains a set of recipients of an item.</span></span> <span data-ttu-id="17fba-120">Estes são os principais destinatários de um item.</span><span class="sxs-lookup"><span data-stu-id="17fba-120">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="17fba-121">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="17fba-121">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="17fba-122">Representa uma coleção de destinatários que receberão uma cópia da mensagem.</span><span class="sxs-lookup"><span data-stu-id="17fba-122">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="17fba-123">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="17fba-123">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="17fba-124">Representa uma coleção de destinatários para receber uma cópia oculta (Cco) de um email.</span><span class="sxs-lookup"><span data-stu-id="17fba-124">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="17fba-125">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="17fba-125">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="17fba-126">Indica se o remetente de um item solicita uma confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="17fba-126">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="17fba-127">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="17fba-127">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="17fba-128">Indica se o remetente de um item solicita uma confirmação de entrega.</span><span class="sxs-lookup"><span data-stu-id="17fba-128">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="17fba-129">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="17fba-129">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="17fba-130">Identifica o item ao qual o objeto Response se refere.</span><span class="sxs-lookup"><span data-stu-id="17fba-130">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="17fba-131">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="17fba-131">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="17fba-132">Representa o novo conteúdo do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="17fba-132">Represents the new body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="17fba-133">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="17fba-133">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="17fba-134">Identifica o representante em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="17fba-134">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="17fba-135">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="17fba-135">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="17fba-136">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="17fba-136">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="17fba-137">Identifica o principal em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="17fba-137">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="17fba-138">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="17fba-138">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="17fba-139">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="17fba-139">Parent elements</span></span>

|<span data-ttu-id="17fba-140">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="17fba-140">**Element**</span></span>|<span data-ttu-id="17fba-141">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="17fba-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17fba-142">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="17fba-142">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="17fba-143">Descreve todos os itens que estão adjacentes a um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="17fba-143">Describes all items that are adjacent to a meeting time.</span></span><br/><br/> <span data-ttu-id="17fba-144">A seguir estão algumas das expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="17fba-144">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="17fba-145">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="17fba-145">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="17fba-146">Descreve todos os itens que entram em conflito com um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="17fba-146">Describes all items that conflict with a meeting time.</span></span><br/><br/><span data-ttu-id="17fba-147">A seguir estão algumas das expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="17fba-147">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="17fba-148">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="17fba-148">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="17fba-149">Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="17fba-149">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="17fba-150">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="17fba-150">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="17fba-151">Contém uma matriz de itens a serem criados na pasta identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="17fba-151">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="17fba-152">Comentários</span><span class="sxs-lookup"><span data-stu-id="17fba-152">Remarks</span></span>

<span data-ttu-id="17fba-153">O elemento **CancelCalendarItem** é exibido apenas pelo organizador.</span><span class="sxs-lookup"><span data-stu-id="17fba-153">The **CancelCalendarItem** element is only viewed by the organizer.</span></span> <span data-ttu-id="17fba-154">Ele só se aplica ao item de calendário do organizador.</span><span class="sxs-lookup"><span data-stu-id="17fba-154">It only applies to the organizer's calendar item.</span></span> 
  
<span data-ttu-id="17fba-155">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="17fba-155">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17fba-156">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="17fba-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17fba-157">Namespace</span><span class="sxs-lookup"><span data-stu-id="17fba-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="17fba-158">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="17fba-158">Schema Name</span></span>  <br/> |<span data-ttu-id="17fba-159">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="17fba-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="17fba-160">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="17fba-160">Validation File</span></span>  <br/> |<span data-ttu-id="17fba-161">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="17fba-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="17fba-162">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="17fba-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="17fba-163">False</span><span class="sxs-lookup"><span data-stu-id="17fba-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17fba-164">Confira também</span><span class="sxs-lookup"><span data-stu-id="17fba-164">See also</span></span>

- [<span data-ttu-id="17fba-165">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="17fba-165">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

