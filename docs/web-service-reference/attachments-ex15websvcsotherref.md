---
title: Anexos
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attachments
api_type:
- schema
ms.assetid: b470e614-34bb-44f0-8790-7ddbdcbbd29d
description: O elemento Attachments contém os itens ou arquivos anexados a um item no repositório do Exchange.
ms.openlocfilehash: a9f79cd79f19e6226703c99c53c91efed600f495
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461531"
---
# <a name="attachments"></a><span data-ttu-id="12289-103">Attachments</span><span class="sxs-lookup"><span data-stu-id="12289-103">Attachments</span></span>

<span data-ttu-id="12289-104">O elemento **Attachments** contém os itens ou arquivos anexados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12289-104">The **Attachments** element contains the items or files that are attached to an item in the Exchange store.</span></span> 
  
```xml
<Attachments>
   <ItemAttachment/>
   <FileAttachment/>
</Attachments>
```

 <span data-ttu-id="12289-105">**ArrayOfAttachmentsType** e **NonEmptyArrayOfAttachmentsType**</span><span class="sxs-lookup"><span data-stu-id="12289-105">**ArrayOfAttachmentsType** and **NonEmptyArrayOfAttachmentsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12289-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="12289-106">Attributes and elements</span></span>

<span data-ttu-id="12289-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="12289-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12289-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="12289-108">Attributes</span></span>

<span data-ttu-id="12289-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12289-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12289-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="12289-110">Child elements</span></span>

|<span data-ttu-id="12289-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="12289-111">**Element**</span></span>|<span data-ttu-id="12289-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="12289-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12289-113">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="12289-113">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="12289-114">Representa um item do Exchange anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12289-114">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="12289-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="12289-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="12289-116">Representa um arquivo anexado a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12289-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="12289-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="12289-117">Parent elements</span></span>

|<span data-ttu-id="12289-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="12289-118">**Element**</span></span>|<span data-ttu-id="12289-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="12289-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12289-120">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="12289-120">CreateAttachment</span></span>](createattachment.md) <br/> |<span data-ttu-id="12289-121">Define uma solicitação para criar um anexo a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12289-121">Defines a request to create an attachment to an item in the Exchange store.</span></span><br/><br/> <span data-ttu-id="12289-122">A seguir está a expressão XPath para este elemento:`/CreateAttachment`</span><span class="sxs-lookup"><span data-stu-id="12289-122">The following is the XPath expression to this element:  `/CreateAttachment`</span></span> <br/> |
|[<span data-ttu-id="12289-123">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="12289-123">AcceptItem</span></span>](acceptitem.md) <br/> | <span data-ttu-id="12289-124">Representa uma resposta de aceitação para uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="12289-124">Represents an Accept reply to a meeting request.</span></span><br/><br/><span data-ttu-id="12289-125">A seguir estão algumas das expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="12289-125">The following are some of the XPath expressions to this element:</span></span><ul><li>`/CreateItem/Items`</li><li>`/MeetingRequest/ConflictingMeetings` </li><li>`/SetItemField/CalendarItem/ConflictingMeetings`</li><li>`/AppendToItemField/CalendarItem/ConflictingMeetings`</li><li>`/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings`</li><li>`/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li><li>`/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li></ul> |
|[<span data-ttu-id="12289-126">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="12289-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="12289-127">Representa uma resposta de recusa a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="12289-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="12289-128">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="12289-128">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="12289-129">Representa uma resposta provisória a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="12289-129">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="12289-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="12289-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="12289-131">Remove um item do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12289-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="12289-132">Item</span><span class="sxs-lookup"><span data-stu-id="12289-132">Item</span></span>](item.md) <br/> |<span data-ttu-id="12289-133">Representa um item genérico do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12289-133">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="12289-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="12289-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="12289-135">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12289-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="12289-136">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="12289-136">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="12289-137">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12289-137">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="12289-138">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="12289-138">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="12289-139">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12289-139">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="12289-140">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="12289-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="12289-141">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12289-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="12289-142">Mensagem</span><span class="sxs-lookup"><span data-stu-id="12289-142">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="12289-143">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12289-143">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="12289-144">Tarefa</span><span class="sxs-lookup"><span data-stu-id="12289-144">Task</span></span>](task.md) <br/> |<span data-ttu-id="12289-145">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12289-145">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="12289-146">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="12289-146">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="12289-147">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12289-147">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="12289-148">Contato</span><span class="sxs-lookup"><span data-stu-id="12289-148">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="12289-149">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12289-149">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="12289-150">DistributionList</span><span class="sxs-lookup"><span data-stu-id="12289-150">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="12289-151">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="12289-151">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="12289-152">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="12289-152">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md) <br/> |<span data-ttu-id="12289-153">Contém o status e o resultado de uma única solicitação CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="12289-153">Contains the status and result of a single CreateAttachment request.</span></span>  <br/> |
|[<span data-ttu-id="12289-154">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="12289-154">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md) <br/> |<span data-ttu-id="12289-155">Contém o status e o resultado de uma solicitação GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="12289-155">Contains the status and result of a GetAttachment request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="12289-156">Comentários</span><span class="sxs-lookup"><span data-stu-id="12289-156">Remarks</span></span>

<span data-ttu-id="12289-157">Os elementos **Attachments** têm os mesmos elementos filho, mas são baseados em tipos diferentes: **ArrayOfAttachmentsType** e **NonEmptyArrayOfAttachmentsType**.</span><span class="sxs-lookup"><span data-stu-id="12289-157">The **Attachments** elements have the same child elements but are based on different types: **ArrayOfAttachmentsType** and **NonEmptyArrayOfAttachmentsType**.</span></span> <span data-ttu-id="12289-158">Os tipos definem se um elemento filho é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12289-158">The types define whether a child element is required.</span></span> <span data-ttu-id="12289-159">O **ArrayOfAttachmentsType** é usado apenas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="12289-159">The **ArrayOfAttachmentsType** is only used in the response message.</span></span> <span data-ttu-id="12289-160">Também é importante observar que esses elementos ocorrem nos namespaces de messages e Types.</span><span class="sxs-lookup"><span data-stu-id="12289-160">It is also important to note that these elements occur in both the messages and types namespaces.</span></span> 
  
<span data-ttu-id="12289-161">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="12289-161">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12289-162">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="12289-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12289-163">Namespace</span><span class="sxs-lookup"><span data-stu-id="12289-163">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="12289-164">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="12289-164">Schema Name</span></span>  <br/> |<span data-ttu-id="12289-165">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="12289-165">Types schema</span></span>  <br/> |
|<span data-ttu-id="12289-166">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="12289-166">Validation File</span></span>  <br/> |<span data-ttu-id="12289-167">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="12289-167">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="12289-168">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="12289-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="12289-169">False</span><span class="sxs-lookup"><span data-stu-id="12289-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12289-170">Confira também</span><span class="sxs-lookup"><span data-stu-id="12289-170">See also</span></span>

- [<span data-ttu-id="12289-171">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="12289-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

