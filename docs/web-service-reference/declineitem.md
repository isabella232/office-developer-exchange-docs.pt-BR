---
title: DeclineItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeclineItem
api_type:
- schema
ms.assetid: 2d8d2389-924e-4d03-a324-35d56cf0d6b1
description: O elemento DeclineItem representa uma resposta de recusa a uma solicitação de reunião.
ms.openlocfilehash: a3fb2b62ea2fa895a664034d2150f46a3099f6c1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457428"
---
# <a name="declineitem"></a><span data-ttu-id="1834b-103">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="1834b-103">DeclineItem</span></span>

<span data-ttu-id="1834b-104">O elemento **DeclineItem** representa uma resposta de recusa a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="1834b-104">The **DeclineItem** element represents a Decline reply to a meeting request.</span></span> 
  
```xml
<DeclineItem>
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
</DeclineItem>
```

<span data-ttu-id="1834b-105">**DeclineItemType**</span><span class="sxs-lookup"><span data-stu-id="1834b-105">**DeclineItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1834b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1834b-106">Attributes and elements</span></span>

<span data-ttu-id="1834b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1834b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1834b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1834b-108">Attributes</span></span>

<span data-ttu-id="1834b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1834b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1834b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1834b-110">Child elements</span></span>

|<span data-ttu-id="1834b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1834b-111">**Element**</span></span>|<span data-ttu-id="1834b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1834b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1834b-113">ItemClass</span><span class="sxs-lookup"><span data-stu-id="1834b-113">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="1834b-114">Representa a classe de mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="1834b-114">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="1834b-115">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="1834b-115">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="1834b-116">Indica o nível de sensibilidade de um item.</span><span class="sxs-lookup"><span data-stu-id="1834b-116">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="1834b-117">Body</span><span class="sxs-lookup"><span data-stu-id="1834b-117">Body</span></span>](body.md) <br/> |<span data-ttu-id="1834b-118">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="1834b-118">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="1834b-119">Anexos</span><span class="sxs-lookup"><span data-stu-id="1834b-119">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1834b-120">Contém o item ou o arquivo anexado a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1834b-120">Contains the item or file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1834b-121">Propriedadeinternetmessageheaders</span><span class="sxs-lookup"><span data-stu-id="1834b-121">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="1834b-122">Representa o nome do cabeçalho da mensagem da Internet para um determinado cabeçalho dentro da coleção Headers.</span><span class="sxs-lookup"><span data-stu-id="1834b-122">Represents the Internet message header name for a given header within the headers collection.</span></span>  <br/> |
|[<span data-ttu-id="1834b-123">Sender</span><span class="sxs-lookup"><span data-stu-id="1834b-123">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="1834b-124">Identifica o remetente de um item.</span><span class="sxs-lookup"><span data-stu-id="1834b-124">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="1834b-125">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="1834b-125">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="1834b-126">Contém um conjunto de destinatários de um item.</span><span class="sxs-lookup"><span data-stu-id="1834b-126">Contains a set of recipients of an item.</span></span> <span data-ttu-id="1834b-127">Estes são os principais destinatários de um item.</span><span class="sxs-lookup"><span data-stu-id="1834b-127">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="1834b-128">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="1834b-128">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="1834b-129">Representa uma coleção de destinatários que receberão uma cópia da mensagem.</span><span class="sxs-lookup"><span data-stu-id="1834b-129">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="1834b-130">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="1834b-130">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="1834b-131">Representa uma coleção de destinatários para receber uma cópia oculta (Cco) de um email.</span><span class="sxs-lookup"><span data-stu-id="1834b-131">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="1834b-132">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="1834b-132">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="1834b-133">Indica se o remetente de um item solicita uma confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="1834b-133">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="1834b-134">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="1834b-134">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="1834b-135">Indica se o remetente de um item solicita uma confirmação de entrega.</span><span class="sxs-lookup"><span data-stu-id="1834b-135">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="1834b-136">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="1834b-136">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="1834b-137">Identifica o item ao qual o objeto Response se refere.</span><span class="sxs-lookup"><span data-stu-id="1834b-137">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="1834b-138">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="1834b-138">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="1834b-139">Identifica o representante em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="1834b-139">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="1834b-140">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="1834b-140">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="1834b-141">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="1834b-141">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="1834b-142">Identifica o principal em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="1834b-142">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="1834b-143">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="1834b-143">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="1834b-144">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="1834b-144">ProposedStart</span></span>](proposedstart.md) <br/> |<span data-ttu-id="1834b-145">Especifica a hora de início proposta da reunião.</span><span class="sxs-lookup"><span data-stu-id="1834b-145">Specifies the proposed start time of the meeting.</span></span>  <br/> |
|[<span data-ttu-id="1834b-146">ProposedEnd</span><span class="sxs-lookup"><span data-stu-id="1834b-146">ProposedEnd</span></span>](proposedend.md) <br/> |<span data-ttu-id="1834b-147">Especifica a hora de término proposta da reunião.</span><span class="sxs-lookup"><span data-stu-id="1834b-147">Specifies the proposed end time of the meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1834b-148">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1834b-148">Parent elements</span></span>

|<span data-ttu-id="1834b-149">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1834b-149">**Element**</span></span>|<span data-ttu-id="1834b-150">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1834b-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1834b-151">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="1834b-151">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="1834b-152">Descreve todos os itens que estão adjacentes a um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="1834b-152">Describes all items that are adjacent to a meeting time.</span></span><br/><br/><span data-ttu-id="1834b-153">A seguir estão algumas das expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="1834b-153">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="1834b-154">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="1834b-154">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="1834b-155">Descreve todos os itens que entram em conflito com um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="1834b-155">Describes all items that conflict with a meeting time.</span></span><br/><br/><span data-ttu-id="1834b-156">A seguir estão algumas das expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="1834b-156">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="1834b-157">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="1834b-157">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="1834b-158">Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1834b-158">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1834b-159">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="1834b-159">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="1834b-160">Contém uma matriz de itens a serem criados na pasta que é identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="1834b-160">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1834b-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="1834b-161">Remarks</span></span>

<span data-ttu-id="1834b-162">O esquema que descreve este elemento está localizado no diretório virtual do EWS do servidor Exchange que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="1834b-162">The schema that describes this element is located in the EWS virtual directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1834b-163">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1834b-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1834b-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="1834b-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1834b-165">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1834b-165">Schema Name</span></span>  <br/> |<span data-ttu-id="1834b-166">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1834b-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="1834b-167">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1834b-167">Validation File</span></span>  <br/> |<span data-ttu-id="1834b-168">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1834b-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1834b-169">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1834b-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="1834b-170">False</span><span class="sxs-lookup"><span data-stu-id="1834b-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1834b-171">Confira também</span><span class="sxs-lookup"><span data-stu-id="1834b-171">See also</span></span>

- [<span data-ttu-id="1834b-172">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1834b-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

