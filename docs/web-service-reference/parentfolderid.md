---
title: ParentFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 258f4b1f-367e-4c7d-9c29-eb775a2398c7
description: O elemento ParentFolderId representa o identificador da pasta pai que contém o item ou a pasta.
ms.openlocfilehash: 3f60e8adb62fbf464a58af4169fbcd83910877cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824687"
---
# <a name="parentfolderid"></a><span data-ttu-id="d1a8b-103">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="d1a8b-103">ParentFolderId</span></span>

<span data-ttu-id="d1a8b-104">O elemento **ParentFolderId** representa o identificador da pasta pai que contém o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-104">The **ParentFolderId** element represents the identifier of the parent folder that contains the item or folder.</span></span> 
  
```XML
<ParentFolderId Id="" ChangeKey=""/>
```

<span data-ttu-id="d1a8b-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="d1a8b-105">**FolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d1a8b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d1a8b-106">Attributes and elements</span></span>

<span data-ttu-id="d1a8b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1a8b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d1a8b-108">Attributes</span></span>

|<span data-ttu-id="d1a8b-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="d1a8b-109">**Attribute**</span></span>|<span data-ttu-id="d1a8b-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d1a8b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d1a8b-111">**ID de**</span><span class="sxs-lookup"><span data-stu-id="d1a8b-111">**Id**</span></span> <br/> |<span data-ttu-id="d1a8b-112">Contém uma cadeia de caracteres que identifica uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="d1a8b-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="d1a8b-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="d1a8b-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="d1a8b-115">Contém uma cadeia de caracteres que identifica uma versão de uma pasta que é identificada pelo atributo **Id** .</span><span class="sxs-lookup"><span data-stu-id="d1a8b-115">Contains a string that identifies a version of a folder that is identified by the **Id** attribute.</span></span> <span data-ttu-id="d1a8b-116">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-116">This attribute is optional.</span></span> <span data-ttu-id="d1a8b-117">Use este atributo para certificar-se de que a versão correta de uma pasta é usada.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d1a8b-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d1a8b-118">Child elements</span></span>

<span data-ttu-id="d1a8b-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d1a8b-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d1a8b-120">Parent elements</span></span>

|<span data-ttu-id="d1a8b-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d1a8b-121">**Element**</span></span>|<span data-ttu-id="d1a8b-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d1a8b-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1a8b-123">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="d1a8b-123">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="d1a8b-124">Representa uma pasta de calendário em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-124">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-125">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d1a8b-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d1a8b-126">Representa um item de calendário em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-126">Represents a calendar item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-127">Contato</span><span class="sxs-lookup"><span data-stu-id="d1a8b-127">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="d1a8b-128">Representa um item de contato em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-128">Represents a contact item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-129">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="d1a8b-129">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="d1a8b-130">Representa uma pasta de contatos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-130">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-131">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="d1a8b-131">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="d1a8b-132">Representa um evento no qual uma pasta ou um item é copiada.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-132">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-133">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="d1a8b-133">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="d1a8b-134">Representa um evento no qual uma pasta ou um item é criada.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-134">Represents an event in which an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-135">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="d1a8b-135">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="d1a8b-136">Representa um evento no qual uma pasta ou um item é excluída.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-136">Represents an event in which an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-137">DistributionList</span><span class="sxs-lookup"><span data-stu-id="d1a8b-137">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="d1a8b-138">Representa uma lista de distribuição particular em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-138">Represents a private distribution list in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-139">Folder</span><span class="sxs-lookup"><span data-stu-id="d1a8b-139">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="d1a8b-140">Representa uma pasta em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-140">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-141">1.1</span><span class="sxs-lookup"><span data-stu-id="d1a8b-141">Item</span></span>](item.md) <br/> |<span data-ttu-id="d1a8b-142">Representa um item genérico do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-142">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-143">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="d1a8b-143">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="d1a8b-144">Representa um único item para carregar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-144">Represents a single item to upload into a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-145">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="d1a8b-145">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="d1a8b-146">Representa o cancelamento da reunião em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-146">Represents a meeting cancellation in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-147">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="d1a8b-147">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="d1a8b-148">Representa uma mensagem de reunião em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-148">Represents a meeting message in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-149">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d1a8b-149">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d1a8b-150">Representa uma solicitação de reunião em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-150">Represents a meeting request in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-151">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="d1a8b-151">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="d1a8b-152">Representa uma resposta de reunião em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-152">Represents a meeting response in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-153">Mensagem</span><span class="sxs-lookup"><span data-stu-id="d1a8b-153">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d1a8b-154">Representa uma mensagem de email em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-154">Represents an e-mail message in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-155">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="d1a8b-155">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="d1a8b-156">Representa um evento no qual um item ou pasta é modificada.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-156">Represents an event in which an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-157">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="d1a8b-157">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="d1a8b-158">Representa um evento na qual um item ou pasta é movida de uma pasta pai para outra pasta pai.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-158">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-159">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="d1a8b-159">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="d1a8b-160">Representa um evento que é disparado por um novo item de email em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-160">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-161">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="d1a8b-161">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="d1a8b-162">Representa uma resposta de aceitar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-162">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-163">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="d1a8b-163">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="d1a8b-164">Representa um provisório responde a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-164">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-165">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="d1a8b-165">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="d1a8b-166">Representa uma resposta recusar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-166">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-167">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="d1a8b-167">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="d1a8b-168">Remove um item de armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-168">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-169">Task</span><span class="sxs-lookup"><span data-stu-id="d1a8b-169">Task</span></span>](task.md) <br/> |<span data-ttu-id="d1a8b-170">Representa um item de tarefa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-170">Represents a task item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-171">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="d1a8b-171">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="d1a8b-172">Contém uma resposta para o criador de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-172">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-173">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="d1a8b-173">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="d1a8b-174">Contém uma resposta a todos os destinatários identificados de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-174">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-175">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="d1a8b-175">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="d1a8b-176">Contém um item de armazenamento do Exchange para encaminhar para destinatários.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-176">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-177">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="d1a8b-177">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="d1a8b-178">Representa o objeto de resposta é usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-178">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-179">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="d1a8b-179">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="d1a8b-180">Representa uma pasta de tarefa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-180">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1a8b-181">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="d1a8b-181">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="d1a8b-182">Representa uma pasta de pesquisa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-182">Represents a search folder in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d1a8b-183">Comentários</span><span class="sxs-lookup"><span data-stu-id="d1a8b-183">Remarks</span></span>

<span data-ttu-id="d1a8b-184">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d1a8b-184">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1a8b-185">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d1a8b-185">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1a8b-186">Namespace</span><span class="sxs-lookup"><span data-stu-id="d1a8b-186">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d1a8b-187">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d1a8b-187">Schema Name</span></span>  <br/> |<span data-ttu-id="d1a8b-188">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d1a8b-188">Types schema</span></span>  <br/> |
|<span data-ttu-id="d1a8b-189">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d1a8b-189">Validation File</span></span>  <br/> |<span data-ttu-id="d1a8b-190">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d1a8b-190">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d1a8b-191">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d1a8b-191">Can be Empty</span></span>  <br/> |<span data-ttu-id="d1a8b-192">False</span><span class="sxs-lookup"><span data-stu-id="d1a8b-192">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d1a8b-193">Ver também</span><span class="sxs-lookup"><span data-stu-id="d1a8b-193">See also</span></span>

- [<span data-ttu-id="d1a8b-194">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d1a8b-194">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

