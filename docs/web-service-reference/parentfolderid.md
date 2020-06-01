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
ms.openlocfilehash: 3bad638aa21019472df8f487f1e065d2e725e750
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465748"
---
# <a name="parentfolderid"></a><span data-ttu-id="d60c0-103">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="d60c0-103">ParentFolderId</span></span>

<span data-ttu-id="d60c0-104">O elemento **ParentFolderId** representa o identificador da pasta pai que contém o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="d60c0-104">The **ParentFolderId** element represents the identifier of the parent folder that contains the item or folder.</span></span> 
  
```XML
<ParentFolderId Id="" ChangeKey=""/>
```

<span data-ttu-id="d60c0-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="d60c0-105">**FolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d60c0-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d60c0-106">Attributes and elements</span></span>

<span data-ttu-id="d60c0-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d60c0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d60c0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d60c0-108">Attributes</span></span>

|<span data-ttu-id="d60c0-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="d60c0-109">**Attribute**</span></span>|<span data-ttu-id="d60c0-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d60c0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d60c0-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="d60c0-111">**Id**</span></span> <br/> |<span data-ttu-id="d60c0-112">Contém uma cadeia de caracteres que identifica uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d60c0-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="d60c0-113">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="d60c0-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="d60c0-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="d60c0-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="d60c0-115">Contém uma cadeia de caracteres que identifica uma versão de uma pasta identificada pelo atributo **ID** .</span><span class="sxs-lookup"><span data-stu-id="d60c0-115">Contains a string that identifies a version of a folder that is identified by the **Id** attribute.</span></span> <span data-ttu-id="d60c0-116">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="d60c0-116">This attribute is optional.</span></span> <span data-ttu-id="d60c0-117">Use este atributo para certificar-se de que a versão correta de uma pasta é usada.</span><span class="sxs-lookup"><span data-stu-id="d60c0-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d60c0-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d60c0-118">Child elements</span></span>

<span data-ttu-id="d60c0-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d60c0-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d60c0-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d60c0-120">Parent elements</span></span>

|<span data-ttu-id="d60c0-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d60c0-121">**Element**</span></span>|<span data-ttu-id="d60c0-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d60c0-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d60c0-123">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="d60c0-123">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="d60c0-124">Representa uma pasta de calendário em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-124">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-125">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d60c0-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d60c0-126">Representa um item de calendário em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-126">Represents a calendar item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-127">Contato</span><span class="sxs-lookup"><span data-stu-id="d60c0-127">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="d60c0-128">Representa um item de contato em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-128">Represents a contact item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-129">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="d60c0-129">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="d60c0-130">Representa uma pasta contatos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-130">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-131">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="d60c0-131">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="d60c0-132">Representa um evento no qual um item ou pasta é copiado.</span><span class="sxs-lookup"><span data-stu-id="d60c0-132">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-133">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="d60c0-133">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="d60c0-134">Representa um evento no qual um item ou pasta é criado.</span><span class="sxs-lookup"><span data-stu-id="d60c0-134">Represents an event in which an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-135">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="d60c0-135">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="d60c0-136">Representa um evento no qual um item ou pasta é excluído.</span><span class="sxs-lookup"><span data-stu-id="d60c0-136">Represents an event in which an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-137">DistributionList</span><span class="sxs-lookup"><span data-stu-id="d60c0-137">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="d60c0-138">Representa uma lista de distribuição privada em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-138">Represents a private distribution list in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-139">Folder</span><span class="sxs-lookup"><span data-stu-id="d60c0-139">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="d60c0-140">Representa uma pasta em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-140">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-141">Item</span><span class="sxs-lookup"><span data-stu-id="d60c0-141">Item</span></span>](item.md) <br/> |<span data-ttu-id="d60c0-142">Representa um item genérico do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d60c0-142">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-143">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="d60c0-143">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="d60c0-144">Representa um único item a ser carregado em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-144">Represents a single item to upload into a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-145">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="d60c0-145">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="d60c0-146">Representa um cancelamento de reunião em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-146">Represents a meeting cancellation in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-147">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="d60c0-147">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="d60c0-148">Representa uma mensagem de reunião em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-148">Represents a meeting message in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-149">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d60c0-149">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d60c0-150">Representa uma solicitação de reunião em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-150">Represents a meeting request in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-151">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="d60c0-151">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="d60c0-152">Representa uma resposta de reunião em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-152">Represents a meeting response in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-153">Message</span><span class="sxs-lookup"><span data-stu-id="d60c0-153">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d60c0-154">Representa uma mensagem de email em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-154">Represents an e-mail message in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-155">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="d60c0-155">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="d60c0-156">Representa um evento no qual um item ou pasta é modificado.</span><span class="sxs-lookup"><span data-stu-id="d60c0-156">Represents an event in which an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-157">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="d60c0-157">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="d60c0-158">Representa um evento no qual um item ou pasta é movido de uma pasta pai para outra pasta pai.</span><span class="sxs-lookup"><span data-stu-id="d60c0-158">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-159">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="d60c0-159">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="d60c0-160">Representa um evento que é disparado por um novo item de email em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-160">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-161">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="d60c0-161">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="d60c0-162">Representa uma resposta de aceitação para uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="d60c0-162">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-163">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="d60c0-163">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="d60c0-164">Representa uma resposta provisória a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="d60c0-164">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-165">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="d60c0-165">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="d60c0-166">Representa uma resposta de recusa a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="d60c0-166">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-167">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="d60c0-167">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="d60c0-168">Remove um item do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d60c0-168">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-169">Tarefa</span><span class="sxs-lookup"><span data-stu-id="d60c0-169">Task</span></span>](task.md) <br/> |<span data-ttu-id="d60c0-170">Representa um item de tarefa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-170">Represents a task item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-171">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="d60c0-171">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="d60c0-172">Contém uma resposta para o criador de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d60c0-172">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-173">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="d60c0-173">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="d60c0-174">Contém uma resposta a todos os destinatários identificados de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d60c0-174">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-175">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="d60c0-175">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="d60c0-176">Contém um item de repositório do Exchange para encaminhar aos destinatários.</span><span class="sxs-lookup"><span data-stu-id="d60c0-176">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-177">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="d60c0-177">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="d60c0-178">Representa o objeto Response que é usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="d60c0-178">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-179">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="d60c0-179">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="d60c0-180">Representa uma pasta de tarefas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-180">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d60c0-181">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="d60c0-181">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="d60c0-182">Representa uma pasta de pesquisa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d60c0-182">Represents a search folder in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d60c0-183">Comentários</span><span class="sxs-lookup"><span data-stu-id="d60c0-183">Remarks</span></span>

<span data-ttu-id="d60c0-184">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d60c0-184">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d60c0-185">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d60c0-185">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d60c0-186">Namespace</span><span class="sxs-lookup"><span data-stu-id="d60c0-186">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d60c0-187">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d60c0-187">Schema Name</span></span>  <br/> |<span data-ttu-id="d60c0-188">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d60c0-188">Types schema</span></span>  <br/> |
|<span data-ttu-id="d60c0-189">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d60c0-189">Validation File</span></span>  <br/> |<span data-ttu-id="d60c0-190">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d60c0-190">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d60c0-191">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d60c0-191">Can be Empty</span></span>  <br/> |<span data-ttu-id="d60c0-192">False</span><span class="sxs-lookup"><span data-stu-id="d60c0-192">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d60c0-193">Confira também</span><span class="sxs-lookup"><span data-stu-id="d60c0-193">See also</span></span>

- [<span data-ttu-id="d60c0-194">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d60c0-194">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

