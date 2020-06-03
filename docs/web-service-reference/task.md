---
title: Tarefa
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Task
api_type:
- schema
ms.assetid: 7c84927e-db28-4c5d-b0b5-cbcc2b88d869
description: O elemento Task representa uma tarefa no repositório do Exchange.
ms.openlocfilehash: 669f90dfa74cd085091e9836a1d31ca53bbf165e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458940"
---
# <a name="task"></a><span data-ttu-id="f6649-103">Tarefa</span><span class="sxs-lookup"><span data-stu-id="f6649-103">Task</span></span>

<span data-ttu-id="f6649-104">O elemento **Task** representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6649-104">The **Task** element represents a task in the Exchange store.</span></span> 
  
```xml
<Task>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <ActualWork/>
   <AssignedTime/>
   <BillingInformation/>
   <ChangeCount/>
   <Companies/>
   <CompleteDate/>
   <Contacts/>
   <DelegationState/>
   <Delegator/>
   <DueDate/>
   <IsAssignmentEditable/>
   <IsComplete/>
   <IsRecurring/>
   <IsTeamTask/>
   <Mileage/>
   <Owner/>
   <PercentComplete/>
   <Recurrence/>
   <StartDate/>
   <Status/>
   <StatusDescription/>
   <TotalWork/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</Task>
```

<span data-ttu-id="f6649-105">**TaskType**</span><span class="sxs-lookup"><span data-stu-id="f6649-105">**TaskType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f6649-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f6649-106">Attributes and elements</span></span>

<span data-ttu-id="f6649-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f6649-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6649-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f6649-108">Attributes</span></span>

<span data-ttu-id="f6649-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f6649-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6649-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f6649-110">Child elements</span></span>

|<span data-ttu-id="f6649-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f6649-111">**Element**</span></span>|<span data-ttu-id="f6649-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f6649-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6649-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="f6649-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="f6649-114">Contém o fluxo MIME (Multipurpose Internet Mail Extensions) nativo de um objeto representado no formato base64Binary.</span><span class="sxs-lookup"><span data-stu-id="f6649-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="f6649-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="f6649-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="f6649-116">Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6649-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6649-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="f6649-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="f6649-118">Representa o identificador da pasta pai que contém o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="f6649-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="f6649-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="f6649-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="f6649-120">Representa a classe de mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="f6649-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="f6649-121">Assunto</span><span class="sxs-lookup"><span data-stu-id="f6649-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="f6649-122">Representa o assunto de itens do repositório do Exchange e objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="f6649-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="f6649-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="f6649-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="f6649-124">Contém o status da sensibilidade de um item.</span><span class="sxs-lookup"><span data-stu-id="f6649-124">Contains the status for an item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="f6649-125">Body</span><span class="sxs-lookup"><span data-stu-id="f6649-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="f6649-126">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="f6649-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="f6649-127">Anexos</span><span class="sxs-lookup"><span data-stu-id="f6649-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f6649-128">Contém os itens ou arquivos anexados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6649-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6649-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="f6649-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="f6649-130">Representa a data e a hora em que um item foi recebido em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f6649-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="f6649-131">Tamanho</span><span class="sxs-lookup"><span data-stu-id="f6649-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="f6649-132">Representa o tamanho, em bytes, de um item.</span><span class="sxs-lookup"><span data-stu-id="f6649-132">Represents the size, in bytes, of an item.</span></span> <span data-ttu-id="f6649-133">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f6649-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f6649-134">Categorias</span><span class="sxs-lookup"><span data-stu-id="f6649-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f6649-135">Representa uma coleção de cadeias de caracteres que identificam a quais categorias um item da caixa de correio pertence.</span><span class="sxs-lookup"><span data-stu-id="f6649-135">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="f6649-136">Importance</span><span class="sxs-lookup"><span data-stu-id="f6649-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="f6649-137">Descreve a importância de um item.</span><span class="sxs-lookup"><span data-stu-id="f6649-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="f6649-138">Inresponderto</span><span class="sxs-lookup"><span data-stu-id="f6649-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="f6649-139">Representa o identificador do item para o qual este item é uma resposta.</span><span class="sxs-lookup"><span data-stu-id="f6649-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="f6649-140">Isenviado</span><span class="sxs-lookup"><span data-stu-id="f6649-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="f6649-141">Indica se um item foi enviado para a pasta padrão da pasta de saída.</span><span class="sxs-lookup"><span data-stu-id="f6649-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="f6649-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="f6649-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="f6649-143">Indica se um item ainda não foi enviado.</span><span class="sxs-lookup"><span data-stu-id="f6649-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="f6649-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="f6649-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="f6649-145">Indica se um usuário enviou um item para ele.</span><span class="sxs-lookup"><span data-stu-id="f6649-145">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="f6649-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="f6649-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="f6649-147">Indica se o item foi enviado anteriormente.</span><span class="sxs-lookup"><span data-stu-id="f6649-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="f6649-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="f6649-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="f6649-149">Indica se o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="f6649-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="f6649-150">Propriedadeinternetmessageheaders</span><span class="sxs-lookup"><span data-stu-id="f6649-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="f6649-151">Representa a coleção de todos os cabeçalhos de mensagens da Internet contidos em um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f6649-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f6649-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="f6649-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="f6649-153">Representa a data e a hora em que um item em uma caixa de correio foi enviado.</span><span class="sxs-lookup"><span data-stu-id="f6649-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="f6649-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="f6649-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="f6649-155">Representa a data e a hora em que um determinado item da caixa de correio foi criado.</span><span class="sxs-lookup"><span data-stu-id="f6649-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="f6649-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="f6649-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="f6649-157">Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6649-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6649-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="f6649-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="f6649-159">Representa a data e a hora em que o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="f6649-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="f6649-160">Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="f6649-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="f6649-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="f6649-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="f6649-162">Indica se um lembrete foi definido para um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6649-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6649-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="f6649-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="f6649-164">Representa o número de minutos antes de um evento quando um lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="f6649-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="f6649-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="f6649-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="f6649-166">Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa CC.</span><span class="sxs-lookup"><span data-stu-id="f6649-166">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="f6649-167">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários CC.</span><span class="sxs-lookup"><span data-stu-id="f6649-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="f6649-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="f6649-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="f6649-169">Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa para.</span><span class="sxs-lookup"><span data-stu-id="f6649-169">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="f6649-170">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários.</span><span class="sxs-lookup"><span data-stu-id="f6649-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="f6649-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="f6649-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="f6649-172">Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo visível.</span><span class="sxs-lookup"><span data-stu-id="f6649-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="f6649-173">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f6649-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f6649-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="f6649-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="f6649-175">Identifica as propriedades estendidas em pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="f6649-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="f6649-176">Cultura</span><span class="sxs-lookup"><span data-stu-id="f6649-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="f6649-177">Representa a cultura de um determinado item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f6649-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f6649-178">ActualWork</span><span class="sxs-lookup"><span data-stu-id="f6649-178">ActualWork</span></span>](actualwork.md) <br/> |<span data-ttu-id="f6649-179">Representa o tempo real gasto em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="f6649-179">Represents the actual amount of time that is spent on a task.</span></span>  <br/> |
|[<span data-ttu-id="f6649-180">AssignedTime</span><span class="sxs-lookup"><span data-stu-id="f6649-180">AssignedTime</span></span>](assignedtime.md) <br/> |<span data-ttu-id="f6649-181">Representa a hora em que uma tarefa é atribuída a um contato.</span><span class="sxs-lookup"><span data-stu-id="f6649-181">Represents the time when a task is assigned to a contact.</span></span>  <br/> |
|[<span data-ttu-id="f6649-182">BillingInformation</span><span class="sxs-lookup"><span data-stu-id="f6649-182">BillingInformation</span></span>](billinginformation.md) <br/> |<span data-ttu-id="f6649-183">Contém informações de cobrança de uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="f6649-183">Holds billing information for a task.</span></span>  <br/> |
|[<span data-ttu-id="f6649-184">ChangeCount</span><span class="sxs-lookup"><span data-stu-id="f6649-184">ChangeCount</span></span>](changecount.md) <br/> |<span data-ttu-id="f6649-185">Especifica a versão da tarefa.</span><span class="sxs-lookup"><span data-stu-id="f6649-185">Specifies the version of the task.</span></span>  <br/> |
|[<span data-ttu-id="f6649-186">Companies</span><span class="sxs-lookup"><span data-stu-id="f6649-186">Companies</span></span>](companies.md) <br/> |<span data-ttu-id="f6649-187">Representa a coleção de empresas que estão associadas a um contato ou a uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="f6649-187">Represents the collection of companies that are associated with a contact or task.</span></span>  <br/> |
|[<span data-ttu-id="f6649-188">Concluído</span><span class="sxs-lookup"><span data-stu-id="f6649-188">CompleteDate</span></span>](completedate.md) <br/> |<span data-ttu-id="f6649-189">Representa a data na qual uma tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="f6649-189">Represents the date on which a task is completed.</span></span>  <br/> |
|[<span data-ttu-id="f6649-190">Contatos</span><span class="sxs-lookup"><span data-stu-id="f6649-190">Contacts</span></span>](contacts-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f6649-191">Contém uma lista de contatos que estão associados a uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="f6649-191">Contains a list of contacts that are associated with a task.</span></span>  <br/> |
|[<span data-ttu-id="f6649-192">DelegationState</span><span class="sxs-lookup"><span data-stu-id="f6649-192">DelegationState</span></span>](delegationstate.md) <br/> |<span data-ttu-id="f6649-193">Representa o status de uma tarefa delegada.</span><span class="sxs-lookup"><span data-stu-id="f6649-193">Represents the status of a delegated task.</span></span>  <br/> |
|[<span data-ttu-id="f6649-194">Delegator</span><span class="sxs-lookup"><span data-stu-id="f6649-194">Delegator</span></span>](delegator.md) <br/> |<span data-ttu-id="f6649-195">Contém o nome do delegante que atribuiu a tarefa.</span><span class="sxs-lookup"><span data-stu-id="f6649-195">Contains the name of the delegator who assigned the task.</span></span>  <br/> |
|[<span data-ttu-id="f6649-196">DueDate</span><span class="sxs-lookup"><span data-stu-id="f6649-196">DueDate</span></span>](duedate.md) <br/> |<span data-ttu-id="f6649-197">Representa a data de vencimento de um item de tarefa.</span><span class="sxs-lookup"><span data-stu-id="f6649-197">Represents the date when a task item is due.</span></span>  <br/> |
|[<span data-ttu-id="f6649-198">IsAssignmentEditable</span><span class="sxs-lookup"><span data-stu-id="f6649-198">IsAssignmentEditable</span></span>](isassignmenteditable.md) <br/> |<span data-ttu-id="f6649-199">Indica se a tarefa é editável ou não.</span><span class="sxs-lookup"><span data-stu-id="f6649-199">Indicates whether the task is editable or not.</span></span>  <br/> |
|[<span data-ttu-id="f6649-200">IsComplete</span><span class="sxs-lookup"><span data-stu-id="f6649-200">IsComplete</span></span>](iscomplete.md) <br/> |<span data-ttu-id="f6649-201">Indica se a tarefa foi concluída ou não.</span><span class="sxs-lookup"><span data-stu-id="f6649-201">Indicates whether the task has been completed or not.</span></span>  <br/> |
|[<span data-ttu-id="f6649-202">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="f6649-202">IsRecurring</span></span>](isrecurring.md) <br/> |<span data-ttu-id="f6649-203">Indica se uma tarefa faz parte de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="f6649-203">Indicates whether a task is part of a recurring item.</span></span> <span data-ttu-id="f6649-204">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f6649-204">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f6649-205">IsTeamTask</span><span class="sxs-lookup"><span data-stu-id="f6649-205">IsTeamTask</span></span>](isteamtask.md) <br/> |<span data-ttu-id="f6649-206">Indica se a tarefa pertence a uma equipe ou não.</span><span class="sxs-lookup"><span data-stu-id="f6649-206">Indicates whether the task is owned by a team or not.</span></span>  <br/> |
|[<span data-ttu-id="f6649-207">Mileage</span><span class="sxs-lookup"><span data-stu-id="f6649-207">Mileage</span></span>](mileage.md) <br/> |<span data-ttu-id="f6649-208">Representa a quilometragem de um item de tarefa.</span><span class="sxs-lookup"><span data-stu-id="f6649-208">Represents mileage for a task item.</span></span>  <br/> |
|[<span data-ttu-id="f6649-209">Owner</span><span class="sxs-lookup"><span data-stu-id="f6649-209">Owner</span></span>](owner.md) <br/> |<span data-ttu-id="f6649-210">Representa o proprietário de uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="f6649-210">Represents the owner of a task.</span></span>  <br/> |
|[<span data-ttu-id="f6649-211">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="f6649-211">PercentComplete</span></span>](percentcomplete.md) <br/> |<span data-ttu-id="f6649-212">Descreve o status de conclusão de uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="f6649-212">Describes the completion status of a task.</span></span>  <br/> |
|[<span data-ttu-id="f6649-213">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="f6649-213">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="f6649-214">Contém informações de recorrência para tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="f6649-214">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="f6649-215">StartDate</span><span class="sxs-lookup"><span data-stu-id="f6649-215">StartDate</span></span>](startdate.md) <br/> |<span data-ttu-id="f6649-216">Representa a data de início de um item de tarefa.</span><span class="sxs-lookup"><span data-stu-id="f6649-216">Represents the start date of a task item.</span></span>  <br/> |
|[<span data-ttu-id="f6649-217">Status</span><span class="sxs-lookup"><span data-stu-id="f6649-217">Status</span></span>](status.md) <br/> |<span data-ttu-id="f6649-218">Representa o status de um item de tarefa.</span><span class="sxs-lookup"><span data-stu-id="f6649-218">Represents the status of a task item.</span></span>  <br/> |
|[<span data-ttu-id="f6649-219">StatusDescription</span><span class="sxs-lookup"><span data-stu-id="f6649-219">StatusDescription</span></span>](statusdescription.md) <br/> |<span data-ttu-id="f6649-220">Contém uma explicação sobre o status da tarefa.</span><span class="sxs-lookup"><span data-stu-id="f6649-220">Contains an explanation of the task status.</span></span>  <br/> |
|[<span data-ttu-id="f6649-221">TotalWork</span><span class="sxs-lookup"><span data-stu-id="f6649-221">TotalWork</span></span>](totalwork.md) <br/> |<span data-ttu-id="f6649-222">Contém uma descrição de quanto trabalho está associado a um item.</span><span class="sxs-lookup"><span data-stu-id="f6649-222">Contains a description of how much work is associated with an item.</span></span>  <br/> |
|[<span data-ttu-id="f6649-223">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="f6649-223">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="f6649-224">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="f6649-224">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="f6649-225">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f6649-225">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f6649-226">LastModified</span><span class="sxs-lookup"><span data-stu-id="f6649-226">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="f6649-227">Contém o nome de exibição do último usuário a modificar um item.</span><span class="sxs-lookup"><span data-stu-id="f6649-227">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="f6649-228">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="f6649-228">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="f6649-229">Indica quando um item foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f6649-229">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="f6649-230">Isassociated</span><span class="sxs-lookup"><span data-stu-id="f6649-230">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="f6649-231">Indica se o item está associado a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="f6649-231">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="f6649-232">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="f6649-232">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="f6649-233">Representa uma URL para concatenar ao ponto de extremidade do Microsoft Office Outlook Web App para ler um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="f6649-233">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="f6649-234">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="f6649-234">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="f6649-235">Representa uma URL para concatenar ao ponto de extremidade do Outlook Web App para editar um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="f6649-235">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="f6649-236">ConversationId</span><span class="sxs-lookup"><span data-stu-id="f6649-236">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="f6649-237">Contém o identificador de um item ou uma conversa.</span><span class="sxs-lookup"><span data-stu-id="f6649-237">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="f6649-238">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="f6649-238">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="f6649-239">Representa um fragmento HTML ou texto sem formatação que representa o corpo exclusivo desta conversa.</span><span class="sxs-lookup"><span data-stu-id="f6649-239">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f6649-240">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f6649-240">Parent elements</span></span>

|<span data-ttu-id="f6649-241">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f6649-241">**Element**</span></span>|<span data-ttu-id="f6649-242">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f6649-242">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6649-243">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="f6649-243">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="f6649-244">Descreve todos os itens de calendário adjacentes a um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="f6649-244">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="f6649-245">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="f6649-245">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="f6649-246">Identifica os dados a serem acrescentados a uma única propriedade de um item/pasta durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f6649-246">Identifies data to append to a single property of an item/folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="f6649-247">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="f6649-247">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="f6649-248">Identifica todos os itens que entram em conflito com um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="f6649-248">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="f6649-249">Create (issync)</span><span class="sxs-lookup"><span data-stu-id="f6649-249">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="f6649-250">Identifica um único item a ser criado no armazenamento do cliente local.</span><span class="sxs-lookup"><span data-stu-id="f6649-250">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="f6649-251">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="f6649-251">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="f6649-252">Representa um item do Exchange anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6649-252">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="f6649-253">Itens</span><span class="sxs-lookup"><span data-stu-id="f6649-253">Items</span></span>](items.md) <br/> |<span data-ttu-id="f6649-254">Contém uma matriz de itens.</span><span class="sxs-lookup"><span data-stu-id="f6649-254">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="f6649-255">Setitemfield</span><span class="sxs-lookup"><span data-stu-id="f6649-255">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="f6649-256">Representa uma atualização de uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f6649-256">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="f6649-257">Atualização (issync)</span><span class="sxs-lookup"><span data-stu-id="f6649-257">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="f6649-258">Identifica um único item a ser atualizado no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="f6649-258">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f6649-259">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f6649-259">Text value</span></span>

<span data-ttu-id="f6649-260">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f6649-260">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f6649-261">Comentários</span><span class="sxs-lookup"><span data-stu-id="f6649-261">Remarks</span></span>

<span data-ttu-id="f6649-262">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6649-262">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6649-263">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f6649-263">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6649-264">Namespace</span><span class="sxs-lookup"><span data-stu-id="f6649-264">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f6649-265">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f6649-265">Schema name</span></span>  <br/> |<span data-ttu-id="f6649-266">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f6649-266">Types schema</span></span>  <br/> |
|<span data-ttu-id="f6649-267">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f6649-267">Validation file</span></span>  <br/> |<span data-ttu-id="f6649-268">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f6649-268">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f6649-269">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f6649-269">Can be empty</span></span>  <br/> |<span data-ttu-id="f6649-270">False</span><span class="sxs-lookup"><span data-stu-id="f6649-270">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6649-271">Confira também</span><span class="sxs-lookup"><span data-stu-id="f6649-271">See also</span></span>

- [<span data-ttu-id="f6649-272">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f6649-272">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="f6649-273">Criando tarefas</span><span class="sxs-lookup"><span data-stu-id="f6649-273">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
- [<span data-ttu-id="f6649-274">Excluir tarefas</span><span class="sxs-lookup"><span data-stu-id="f6649-274">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

