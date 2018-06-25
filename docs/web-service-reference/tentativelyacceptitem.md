---
title: TentativelyAcceptItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TentativelyAcceptItem
api_type:
- schema
ms.assetid: ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0
description: A element TentativelyAcceptItem representa um provisório responder a uma solicitação de reunião.
ms.openlocfilehash: 203028aae2ec972e36209b2a97420e83d61ddd81
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837719"
---
# <a name="tentativelyacceptitem"></a><span data-ttu-id="e94fe-103">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="e94fe-103">TentativelyAcceptItem</span></span>

<span data-ttu-id="e94fe-104">A element **TentativelyAcceptItem** representa um provisório responder a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="e94fe-104">The **TentativelyAcceptItem** element represents a Tentative reply to a meeting request.</span></span> 
  
```xml
<TentativelyAcceptItem>
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
</TentativelyAcceptItem>
```

 <span data-ttu-id="e94fe-105">**TentativelyAcceptItemType**</span><span class="sxs-lookup"><span data-stu-id="e94fe-105">**TentativelyAcceptItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e94fe-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e94fe-106">Attributes and elements</span></span>

<span data-ttu-id="e94fe-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e94fe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e94fe-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e94fe-108">Attributes</span></span>

<span data-ttu-id="e94fe-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e94fe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e94fe-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e94fe-110">Child elements</span></span>

|<span data-ttu-id="e94fe-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e94fe-111">**Element**</span></span>|<span data-ttu-id="e94fe-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e94fe-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e94fe-113">ItemClass</span><span class="sxs-lookup"><span data-stu-id="e94fe-113">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="e94fe-114">Representa a classe de mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="e94fe-114">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="e94fe-115">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="e94fe-115">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="e94fe-116">Identifica a sensibilidade de um item.</span><span class="sxs-lookup"><span data-stu-id="e94fe-116">Identifies the sensitivity of an item.</span></span>  <br/> |
|[<span data-ttu-id="e94fe-117">Corpo</span><span class="sxs-lookup"><span data-stu-id="e94fe-117">Body</span></span>](body.md) <br/> |<span data-ttu-id="e94fe-118">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="e94fe-118">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="e94fe-119">Anexos</span><span class="sxs-lookup"><span data-stu-id="e94fe-119">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e94fe-120">Contém o item ou arquivo anexado a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e94fe-120">Contains the item or file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e94fe-121">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="e94fe-121">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="e94fe-122">Representa o nome de cabeçalho de mensagem da Internet para um determinado cabeçalho dentro da coleção de cabeçalhos.</span><span class="sxs-lookup"><span data-stu-id="e94fe-122">Represents the Internet message header name for a given header within the headers collection.</span></span>  <br/> |
|[<span data-ttu-id="e94fe-123">Sender</span><span class="sxs-lookup"><span data-stu-id="e94fe-123">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="e94fe-124">Identifica o remetente de um item.</span><span class="sxs-lookup"><span data-stu-id="e94fe-124">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="e94fe-125">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="e94fe-125">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="e94fe-126">Contém um conjunto de destinatários de um item.</span><span class="sxs-lookup"><span data-stu-id="e94fe-126">Contains a set of recipients of an item.</span></span> <span data-ttu-id="e94fe-127">Estes são os principais destinatários de um item.</span><span class="sxs-lookup"><span data-stu-id="e94fe-127">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="e94fe-128">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="e94fe-128">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="e94fe-129">Representa uma coleção dos destinatários que receberão uma cópia da mensagem.</span><span class="sxs-lookup"><span data-stu-id="e94fe-129">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="e94fe-130">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="e94fe-130">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="e94fe-131">Representa uma coleção de destinatários para receber uma cópia oculta (Cco) de um email.</span><span class="sxs-lookup"><span data-stu-id="e94fe-131">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="e94fe-132">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="e94fe-132">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="e94fe-133">Indica se o remetente de um item solicita uma confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="e94fe-133">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="e94fe-134">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="e94fe-134">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="e94fe-135">Indica se o remetente de um item solicita uma confirmação de entrega.</span><span class="sxs-lookup"><span data-stu-id="e94fe-135">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="e94fe-136">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="e94fe-136">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="e94fe-137">Identifica o item ao qual se refere no objeto response.</span><span class="sxs-lookup"><span data-stu-id="e94fe-137">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="e94fe-138">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="e94fe-138">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="e94fe-139">Identifica o delegado em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="e94fe-139">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="e94fe-140">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e94fe-140">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="e94fe-141">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="e94fe-141">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="e94fe-142">Identifica a entidade em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="e94fe-142">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="e94fe-143">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e94fe-143">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="e94fe-144">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="e94fe-144">ProposedStart</span></span>](proposedstart.md) <br/> |<span data-ttu-id="e94fe-145">Especifica a hora de início proposta da solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="e94fe-145">Specifies the proposed start time of the meeting request.</span></span>  <br/> |
|[<span data-ttu-id="e94fe-146">ProposedEnd</span><span class="sxs-lookup"><span data-stu-id="e94fe-146">ProposedEnd</span></span>](proposedend.md) <br/> |<span data-ttu-id="e94fe-147">Especifica a hora de término proposta da solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="e94fe-147">Specifies the proposed end time of the meeting request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e94fe-148">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e94fe-148">Parent elements</span></span>

|<span data-ttu-id="e94fe-149">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e94fe-149">**Element**</span></span>|<span data-ttu-id="e94fe-150">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e94fe-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e94fe-151">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="e94fe-151">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="e94fe-152">Descreve todos os itens que são adjacentes para um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="e94fe-152">Describes all items that are adjacent to a meeting time.</span></span>  <br/> <br/> <span data-ttu-id="e94fe-153">A seguir estão algumas das expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="e94fe-153">The following are some of the XPath expressions to this element:</span></span>  <br/><br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="e94fe-154">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="e94fe-154">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="e94fe-155">Descreve todos os itens que estão em conflito com um tempo de reunião.</span><span class="sxs-lookup"><span data-stu-id="e94fe-155">Describes all items that conflict with a meeting time.</span></span> <br/> <br/>  <span data-ttu-id="e94fe-156">A seguir estão algumas das expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="e94fe-156">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="e94fe-157">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="e94fe-157">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="e94fe-158">Contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e94fe-158">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e94fe-159">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="e94fe-159">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="e94fe-160">Contém uma matriz de itens para criar a pasta identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="e94fe-160">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e94fe-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="e94fe-161">Remarks</span></span>

<span data-ttu-id="e94fe-162">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="e94fe-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e94fe-163">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e94fe-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e94fe-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="e94fe-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e94fe-165">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e94fe-165">Schema Name</span></span>  <br/> |<span data-ttu-id="e94fe-166">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e94fe-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="e94fe-167">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e94fe-167">Validation File</span></span>  <br/> |<span data-ttu-id="e94fe-168">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e94fe-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e94fe-169">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e94fe-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="e94fe-170">False</span><span class="sxs-lookup"><span data-stu-id="e94fe-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e94fe-171">Ver também</span><span class="sxs-lookup"><span data-stu-id="e94fe-171">See also</span></span>

- [<span data-ttu-id="e94fe-172">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e94fe-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

