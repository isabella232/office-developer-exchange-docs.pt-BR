---
title: AcceptItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AcceptItem
api_type:
- schema
ms.assetid: 05a15431-77e1-411a-a16b-5481d364d3cc
description: O elemento AcceptItem representa uma resposta de aceitar a uma solicitação de reunião.
ms.openlocfilehash: 532862fc5299364e51ed469047deaea058692e83
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752216"
---
# <a name="acceptitem"></a><span data-ttu-id="d33cd-103">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="d33cd-103">AcceptItem</span></span>

<span data-ttu-id="d33cd-104">O elemento **AcceptItem** representa uma resposta de aceitar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="d33cd-104">The **AcceptItem** element represents an Accept reply to a meeting request.</span></span> 
  
```xml
<AcceptItem>
   <ItemClass/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <InternetMessageHeaders/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ReferenceItemId/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
   <ProposedStart/>
   <ProposedEnd/>
</AcceptItem>
```

 <span data-ttu-id="d33cd-105">**AcceptItemType**</span><span class="sxs-lookup"><span data-stu-id="d33cd-105">**AcceptItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d33cd-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d33cd-106">Attributes and elements</span></span>

<span data-ttu-id="d33cd-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d33cd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d33cd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d33cd-108">Attributes</span></span>

<span data-ttu-id="d33cd-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d33cd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d33cd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d33cd-110">Child elements</span></span>

|<span data-ttu-id="d33cd-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d33cd-111">**Element**</span></span>|<span data-ttu-id="d33cd-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d33cd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d33cd-113">ItemClass</span><span class="sxs-lookup"><span data-stu-id="d33cd-113">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="d33cd-114">Representa a classe de mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="d33cd-114">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="d33cd-115">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="d33cd-115">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="d33cd-116">Indica o nível de sensibilidade de um item.</span><span class="sxs-lookup"><span data-stu-id="d33cd-116">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="d33cd-117">Corpo</span><span class="sxs-lookup"><span data-stu-id="d33cd-117">Body</span></span>](body.md) <br/> |<span data-ttu-id="d33cd-118">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="d33cd-118">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="d33cd-119">Anexos</span><span class="sxs-lookup"><span data-stu-id="d33cd-119">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d33cd-120">Contém o item ou arquivo anexado a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d33cd-120">Contains the item or file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d33cd-121">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="d33cd-121">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="d33cd-122">Representa o nome de cabeçalho de mensagem da Internet para um determinado cabeçalho dentro da coleção de cabeçalhos.</span><span class="sxs-lookup"><span data-stu-id="d33cd-122">Represents the Internet message header name for a given header within the headers collection.</span></span>  <br/> |
|[<span data-ttu-id="d33cd-123">Sender</span><span class="sxs-lookup"><span data-stu-id="d33cd-123">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="d33cd-124">Identifica o remetente de um item.</span><span class="sxs-lookup"><span data-stu-id="d33cd-124">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="d33cd-125">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="d33cd-125">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="d33cd-126">Contém um conjunto de destinatários de um item.</span><span class="sxs-lookup"><span data-stu-id="d33cd-126">Contains a set of recipients of an item.</span></span> <span data-ttu-id="d33cd-127">Estes são os principais destinatários de um item.</span><span class="sxs-lookup"><span data-stu-id="d33cd-127">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="d33cd-128">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="d33cd-128">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="d33cd-129">Representa uma coleção dos destinatários que receberão uma cópia da mensagem.</span><span class="sxs-lookup"><span data-stu-id="d33cd-129">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="d33cd-130">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="d33cd-130">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="d33cd-131">Representa uma coleção de destinatários para receber uma cópia oculta (Cco) de um email.</span><span class="sxs-lookup"><span data-stu-id="d33cd-131">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="d33cd-132">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d33cd-132">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="d33cd-133">Indica se o remetente de um item solicita uma confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="d33cd-133">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="d33cd-134">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d33cd-134">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="d33cd-135">Indica se o remetente de um item solicita uma confirmação de entrega.</span><span class="sxs-lookup"><span data-stu-id="d33cd-135">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="d33cd-136">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="d33cd-136">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="d33cd-137">Identifica o item ao qual se refere no objeto response.</span><span class="sxs-lookup"><span data-stu-id="d33cd-137">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="d33cd-138">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="d33cd-138">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="d33cd-139">Identifica o delegado em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="d33cd-139">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="d33cd-140">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d33cd-140">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="d33cd-141">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="d33cd-141">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="d33cd-142">Identifica a entidade em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="d33cd-142">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="d33cd-143">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d33cd-143">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d33cd-144">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="d33cd-144">ProposedStart</span></span>](proposedstart.md) <br/> |<span data-ttu-id="d33cd-145">Especifica a hora de início proposta da reunião.</span><span class="sxs-lookup"><span data-stu-id="d33cd-145">Specifies the proposed start time of the meeting.</span></span>  <br/> |
|[<span data-ttu-id="d33cd-146">ProposedEnd</span><span class="sxs-lookup"><span data-stu-id="d33cd-146">ProposedEnd</span></span>](proposedend.md) <br/> |<span data-ttu-id="d33cd-147">Especifica a hora de término proposta da reunião.</span><span class="sxs-lookup"><span data-stu-id="d33cd-147">Specifies the proposed end time of the meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d33cd-148">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d33cd-148">Parent elements</span></span>

|<span data-ttu-id="d33cd-149">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d33cd-149">**Element**</span></span>|<span data-ttu-id="d33cd-150">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d33cd-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d33cd-151">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="d33cd-151">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="d33cd-152">Descreve todos os itens que são adjacentes para um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="d33cd-152">Describes all items that are adjacent to a meeting time.</span></span><br/><br/>  <span data-ttu-id="d33cd-153">A seguir estão algumas das expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="d33cd-153">The following are some of the XPath expressions to this element:</span></span><br/><br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="d33cd-154">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="d33cd-154">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="d33cd-155">Descreve todos os itens que estão em conflito com um tempo de reunião.</span><span class="sxs-lookup"><span data-stu-id="d33cd-155">Describes all items that conflict with a meeting time.</span></span><br/><br/>  <span data-ttu-id="d33cd-156">A seguir estão algumas das expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="d33cd-156">The following are some of the XPath expressions to this element:</span></span><br/><br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="d33cd-157">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="d33cd-157">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="d33cd-158">Contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d33cd-158">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d33cd-159">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="d33cd-159">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="d33cd-160">Contém uma matriz de itens para criar a pasta identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="d33cd-160">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d33cd-161">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="d33cd-161">Remarks</span></span>

<span data-ttu-id="d33cd-162">O esquema que descreve este elemento está localizado no diretório EWS do servidor do Exchange que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d33cd-162">The schema that describes this element is located in the EWS directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d33cd-163">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d33cd-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d33cd-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="d33cd-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d33cd-165">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d33cd-165">Schema Name</span></span>  <br/> |<span data-ttu-id="d33cd-166">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d33cd-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="d33cd-167">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d33cd-167">Validation File</span></span>  <br/> |<span data-ttu-id="d33cd-168">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d33cd-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d33cd-169">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d33cd-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="d33cd-170">False</span><span class="sxs-lookup"><span data-stu-id="d33cd-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d33cd-171">Ver também</span><span class="sxs-lookup"><span data-stu-id="d33cd-171">See also</span></span>

- [<span data-ttu-id="d33cd-172">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d33cd-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

