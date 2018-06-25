---
title: Attachments
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
description: O elemento de anexos contém os itens ou arquivos que estejam anexados a um item no armazenamento do Exchange.
ms.openlocfilehash: 8aa5c0849122f5ca83485459fce5d0fea449c974
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751224"
---
# <a name="attachments"></a><span data-ttu-id="d9e2c-103">Attachments</span><span class="sxs-lookup"><span data-stu-id="d9e2c-103">Attachments</span></span>

<span data-ttu-id="d9e2c-104">O elemento de **anexos** contém os itens ou arquivos que estejam anexados a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-104">The **Attachments** element contains the items or files that are attached to an item in the Exchange store.</span></span> 
  
```xml
<Attachments>
   <ItemAttachment/>
   <FileAttachment/>
</Attachments>
```

 <span data-ttu-id="d9e2c-105">**ArrayOfAttachmentsType** e **NonEmptyArrayOfAttachmentsType**</span><span class="sxs-lookup"><span data-stu-id="d9e2c-105">**ArrayOfAttachmentsType** and **NonEmptyArrayOfAttachmentsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9e2c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d9e2c-106">Attributes and elements</span></span>

<span data-ttu-id="d9e2c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9e2c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d9e2c-108">Attributes</span></span>

<span data-ttu-id="d9e2c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9e2c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d9e2c-110">Child elements</span></span>

|<span data-ttu-id="d9e2c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d9e2c-111">**Element**</span></span>|<span data-ttu-id="d9e2c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d9e2c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9e2c-113">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="d9e2c-113">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="d9e2c-114">Representa um item do Exchange que está anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-114">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="d9e2c-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="d9e2c-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="d9e2c-116">Representa um arquivo anexado a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d9e2c-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d9e2c-117">Parent elements</span></span>

|<span data-ttu-id="d9e2c-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d9e2c-118">**Element**</span></span>|<span data-ttu-id="d9e2c-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d9e2c-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9e2c-120">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="d9e2c-120">CreateAttachment</span></span>](createattachment.md) <br/> |<span data-ttu-id="d9e2c-121">Define uma solicitação para criar um anexo a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-121">Defines a request to create an attachment to an item in the Exchange store.</span></span><br/><br/> <span data-ttu-id="d9e2c-122">Este é a expressão XPath para esse elemento:`/CreateAttachment`</span><span class="sxs-lookup"><span data-stu-id="d9e2c-122">The following is the XPath expression to this element:  `/CreateAttachment`</span></span> <br/> |
|[<span data-ttu-id="d9e2c-123">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="d9e2c-123">AcceptItem</span></span>](acceptitem.md) <br/> | <span data-ttu-id="d9e2c-124">Representa uma resposta de aceitar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-124">Represents an Accept reply to a meeting request.</span></span><br/><br/><span data-ttu-id="d9e2c-125">A seguir estão algumas das expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="d9e2c-125">The following are some of the XPath expressions to this element:</span></span><ul><li>`/CreateItem/Items`</li><li>`/MeetingRequest/ConflictingMeetings` </li><li>`/SetItemField/CalendarItem/ConflictingMeetings`</li><li>`/AppendToItemField/CalendarItem/ConflictingMeetings`</li><li>`/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings`</li><li>`/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li><li>`/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li></ul> |
|[<span data-ttu-id="d9e2c-126">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="d9e2c-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="d9e2c-127">Representa uma resposta recusar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d9e2c-128">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="d9e2c-128">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="d9e2c-129">Representa um provisório responde a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-129">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d9e2c-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="d9e2c-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="d9e2c-131">Remove um item de armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d9e2c-132">1.1</span><span class="sxs-lookup"><span data-stu-id="d9e2c-132">Item</span></span>](item.md) <br/> |<span data-ttu-id="d9e2c-133">Representa um item genérico do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-133">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="d9e2c-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="d9e2c-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="d9e2c-135">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d9e2c-136">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d9e2c-136">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d9e2c-137">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-137">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d9e2c-138">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="d9e2c-138">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="d9e2c-139">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-139">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d9e2c-140">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="d9e2c-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="d9e2c-141">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d9e2c-142">Mensagem</span><span class="sxs-lookup"><span data-stu-id="d9e2c-142">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d9e2c-143">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-143">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="d9e2c-144">Task</span><span class="sxs-lookup"><span data-stu-id="d9e2c-144">Task</span></span>](task.md) <br/> |<span data-ttu-id="d9e2c-145">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-145">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d9e2c-146">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d9e2c-146">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d9e2c-147">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-147">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d9e2c-148">Contato</span><span class="sxs-lookup"><span data-stu-id="d9e2c-148">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="d9e2c-149">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-149">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="d9e2c-150">DistributionList</span><span class="sxs-lookup"><span data-stu-id="d9e2c-150">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="d9e2c-151">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-151">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="d9e2c-152">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d9e2c-152">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md) <br/> |<span data-ttu-id="d9e2c-153">Contém o status e o resultado de uma única solicitação CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-153">Contains the status and result of a single CreateAttachment request.</span></span>  <br/> |
|[<span data-ttu-id="d9e2c-154">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d9e2c-154">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md) <br/> |<span data-ttu-id="d9e2c-155">Contém o status e o resultado de uma solicitação de GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-155">Contains the status and result of a GetAttachment request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d9e2c-156">Comentários</span><span class="sxs-lookup"><span data-stu-id="d9e2c-156">Remarks</span></span>

<span data-ttu-id="d9e2c-157">Os elementos de **anexos** ter os mesmos elementos filho, mas são baseados em diferentes tipos: **ArrayOfAttachmentsType** e **NonEmptyArrayOfAttachmentsType**.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-157">The **Attachments** elements have the same child elements but are based on different types: **ArrayOfAttachmentsType** and **NonEmptyArrayOfAttachmentsType**.</span></span> <span data-ttu-id="d9e2c-158">Os tipos definem se um elemento filho é necessário.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-158">The types define whether a child element is required.</span></span> <span data-ttu-id="d9e2c-159">O **ArrayOfAttachmentsType** é usado apenas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-159">The **ArrayOfAttachmentsType** is only used in the response message.</span></span> <span data-ttu-id="d9e2c-160">Também é importante observar que esses elementos ocorrerem em namespaces tipos e mensagens.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-160">It is also important to note that these elements occur in both the messages and types namespaces.</span></span> 
  
<span data-ttu-id="d9e2c-161">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d9e2c-161">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9e2c-162">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d9e2c-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9e2c-163">Namespace</span><span class="sxs-lookup"><span data-stu-id="d9e2c-163">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9e2c-164">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d9e2c-164">Schema Name</span></span>  <br/> |<span data-ttu-id="d9e2c-165">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d9e2c-165">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9e2c-166">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d9e2c-166">Validation File</span></span>  <br/> |<span data-ttu-id="d9e2c-167">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d9e2c-167">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9e2c-168">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d9e2c-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9e2c-169">False</span><span class="sxs-lookup"><span data-stu-id="d9e2c-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9e2c-170">Ver também</span><span class="sxs-lookup"><span data-stu-id="d9e2c-170">See also</span></span>

- [<span data-ttu-id="d9e2c-171">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d9e2c-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

