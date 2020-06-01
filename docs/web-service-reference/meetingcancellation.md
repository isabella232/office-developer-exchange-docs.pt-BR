---
title: MeetingCancellation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingCancellation
api_type:
- schema
ms.assetid: a9c61f7f-2ecd-4b21-9dce-24d9f61aeeea
description: O elemento MeetingCancellation representa um cancelamento de reunião no repositório do Exchange.
ms.openlocfilehash: b0fca0a2dcbdf8685f7b9fb2197db1c3123d54b1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467526"
---
# <a name="meetingcancellation"></a><span data-ttu-id="745ca-103">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="745ca-103">MeetingCancellation</span></span>

<span data-ttu-id="745ca-104">O elemento **MeetingCancellation** representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="745ca-104">The **MeetingCancellation** element represents a meeting cancellation in the Exchange store.</span></span> 
  
```xml
<MeetingCancellation>
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
   <Importance/>
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
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ConversationIndex/>
   <ConversationTopic/>
   <From/>
   <InternetMessageId/>
   <IsRead/>
   <IsResponseRequested/>
   <References/>
   <ReplyTo/>
   <AssociatedCalendarItemId/>
   <IsDelegated/>
   <IsOutOfDate/>
   <HasBeenProcessed/>
   <ResponseType/>
</MeetingCancellation>
```

 <span data-ttu-id="745ca-105">**MeetingCancellationMessageType**</span><span class="sxs-lookup"><span data-stu-id="745ca-105">**MeetingCancellationMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="745ca-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="745ca-106">Attributes and elements</span></span>

<span data-ttu-id="745ca-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="745ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="745ca-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="745ca-108">Attributes</span></span>

<span data-ttu-id="745ca-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="745ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="745ca-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="745ca-110">Child elements</span></span>

|<span data-ttu-id="745ca-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="745ca-111">**Element**</span></span>|<span data-ttu-id="745ca-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="745ca-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="745ca-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="745ca-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="745ca-114">Contém o fluxo MIME nativo de um objeto que é representado no formato base64Binary.</span><span class="sxs-lookup"><span data-stu-id="745ca-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="745ca-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="745ca-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="745ca-116">Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="745ca-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="745ca-117">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="745ca-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="745ca-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="745ca-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="745ca-119">Representa o identificador da pasta pai que contém o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="745ca-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="745ca-120">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="745ca-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="745ca-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="745ca-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="745ca-122">Representa a classe de mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="745ca-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="745ca-123">Assunto</span><span class="sxs-lookup"><span data-stu-id="745ca-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="745ca-124">Representa o assunto de itens do repositório do Exchange e objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="745ca-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="745ca-125">O assunto está limitado a 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="745ca-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="745ca-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="745ca-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="745ca-127">Indica o nível de sensibilidade de um item.</span><span class="sxs-lookup"><span data-stu-id="745ca-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="745ca-128">Body</span><span class="sxs-lookup"><span data-stu-id="745ca-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="745ca-129">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="745ca-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="745ca-130">Anexos</span><span class="sxs-lookup"><span data-stu-id="745ca-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="745ca-131">Contém os itens ou arquivos anexados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="745ca-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="745ca-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="745ca-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="745ca-133">Representa a data e a hora em que um item foi recebido em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="745ca-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="745ca-134">Tamanho</span><span class="sxs-lookup"><span data-stu-id="745ca-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="745ca-135">Representa o tamanho em bytes de um item.</span><span class="sxs-lookup"><span data-stu-id="745ca-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="745ca-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="745ca-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="745ca-137">Categorias</span><span class="sxs-lookup"><span data-stu-id="745ca-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="745ca-138">Representa uma coleção de cadeias de caracteres que identificam a quais categorias um item da caixa de correio pertence.</span><span class="sxs-lookup"><span data-stu-id="745ca-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="745ca-139">Importance</span><span class="sxs-lookup"><span data-stu-id="745ca-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="745ca-140">Descreve a importância de um item.</span><span class="sxs-lookup"><span data-stu-id="745ca-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="745ca-141">Inresponderto</span><span class="sxs-lookup"><span data-stu-id="745ca-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="745ca-142">Representa o identificador do item para o qual este item é uma resposta.</span><span class="sxs-lookup"><span data-stu-id="745ca-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="745ca-143">Isenviado</span><span class="sxs-lookup"><span data-stu-id="745ca-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="745ca-144">Indica se um item foi enviado para a pasta padrão da pasta de saída.</span><span class="sxs-lookup"><span data-stu-id="745ca-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="745ca-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="745ca-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="745ca-146">Indica se um item ainda não foi enviado.</span><span class="sxs-lookup"><span data-stu-id="745ca-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="745ca-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="745ca-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="745ca-148">Indica se um usuário enviou um item para ele.</span><span class="sxs-lookup"><span data-stu-id="745ca-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="745ca-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="745ca-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="745ca-150">Indica se o item foi enviado anteriormente.</span><span class="sxs-lookup"><span data-stu-id="745ca-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="745ca-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="745ca-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="745ca-152">Indica se o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="745ca-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="745ca-153">Propriedadeinternetmessageheaders</span><span class="sxs-lookup"><span data-stu-id="745ca-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="745ca-154">Representa a coleção de todos os cabeçalhos de mensagens da Internet que estão contidos em um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="745ca-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="745ca-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="745ca-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="745ca-156">Representa a data e a hora em que um item em uma caixa de correio foi enviado.</span><span class="sxs-lookup"><span data-stu-id="745ca-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="745ca-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="745ca-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="745ca-158">Representa a data e a hora em que um determinado item da caixa de correio foi criado.</span><span class="sxs-lookup"><span data-stu-id="745ca-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="745ca-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="745ca-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="745ca-160">Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="745ca-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="745ca-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="745ca-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="745ca-162">Representa a data e a hora em que o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="745ca-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="745ca-163">Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="745ca-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="745ca-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="745ca-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="745ca-165">Indica se um lembrete foi definido para um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="745ca-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="745ca-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="745ca-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="745ca-167">Representa o número de minutos antes de um evento que um lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="745ca-167">Represents the number of minutes before an event that a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="745ca-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="745ca-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="745ca-169">Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa CC.</span><span class="sxs-lookup"><span data-stu-id="745ca-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="745ca-170">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários CC.</span><span class="sxs-lookup"><span data-stu-id="745ca-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="745ca-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="745ca-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="745ca-172">Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa para.</span><span class="sxs-lookup"><span data-stu-id="745ca-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="745ca-173">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários.</span><span class="sxs-lookup"><span data-stu-id="745ca-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="745ca-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="745ca-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="745ca-175">Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo visível.</span><span class="sxs-lookup"><span data-stu-id="745ca-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="745ca-176">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="745ca-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="745ca-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="745ca-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="745ca-178">Identifica as propriedades estendidas em pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="745ca-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="745ca-179">Cultura</span><span class="sxs-lookup"><span data-stu-id="745ca-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="745ca-180">Representa a cultura de um determinado item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="745ca-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="745ca-181">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="745ca-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="745ca-182">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="745ca-182">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="745ca-183">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="745ca-183">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="745ca-184">LastModified</span><span class="sxs-lookup"><span data-stu-id="745ca-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="745ca-185">Contém o nome de exibição do último usuário a modificar um item.</span><span class="sxs-lookup"><span data-stu-id="745ca-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="745ca-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="745ca-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="745ca-187">Indica quando um item foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="745ca-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="745ca-188">Isassociated</span><span class="sxs-lookup"><span data-stu-id="745ca-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="745ca-189">Indica se o item está associado a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="745ca-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="745ca-190">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="745ca-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="745ca-191">Representa uma URL para concatenar ao ponto de extremidade do Microsoft Office Outlook Web App para ler um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="745ca-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="745ca-192">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="745ca-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="745ca-193">Representa uma URL para concatenar ao ponto de extremidade do Outlook Web App para editar um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="745ca-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="745ca-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="745ca-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="745ca-195">Contém o identificador de um item ou uma conversa.</span><span class="sxs-lookup"><span data-stu-id="745ca-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="745ca-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="745ca-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="745ca-197">Representa um fragmento HTML ou texto sem formatação que representa o corpo exclusivo desta conversa.</span><span class="sxs-lookup"><span data-stu-id="745ca-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="745ca-198">Sender</span><span class="sxs-lookup"><span data-stu-id="745ca-198">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="745ca-199">Identifica o remetente de um item.</span><span class="sxs-lookup"><span data-stu-id="745ca-199">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="745ca-200">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="745ca-200">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="745ca-201">Contém um conjunto de destinatários de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="745ca-201">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="745ca-202">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="745ca-202">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="745ca-203">Representa uma coleção de destinatários que receberão uma cópia da mensagem.</span><span class="sxs-lookup"><span data-stu-id="745ca-203">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="745ca-204">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="745ca-204">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="745ca-205">Representa uma coleção de destinatários para receber uma cópia oculta (Cco) de um email.</span><span class="sxs-lookup"><span data-stu-id="745ca-205">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="745ca-206">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="745ca-206">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="745ca-207">Indica se o remetente de um item solicita uma confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="745ca-207">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="745ca-208">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="745ca-208">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="745ca-209">Indica se o remetente de um item solicita uma confirmação de entrega.</span><span class="sxs-lookup"><span data-stu-id="745ca-209">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="745ca-210">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="745ca-210">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="745ca-211">Contém uma ID binária que representa o thread ao qual esta mensagem pertence.</span><span class="sxs-lookup"><span data-stu-id="745ca-211">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="745ca-212">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="745ca-212">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="745ca-213">Representa o identificador de conversa.</span><span class="sxs-lookup"><span data-stu-id="745ca-213">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="745ca-214">De</span><span class="sxs-lookup"><span data-stu-id="745ca-214">From</span></span>](from.md) <br/> |<span data-ttu-id="745ca-215">Representa o destinatário de quem a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="745ca-215">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="745ca-216">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="745ca-216">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="745ca-217">Representa o identificador de mensagem da Internet de um item.</span><span class="sxs-lookup"><span data-stu-id="745ca-217">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="745ca-218">IsRead</span><span class="sxs-lookup"><span data-stu-id="745ca-218">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="745ca-219">Indica se uma mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="745ca-219">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="745ca-220">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="745ca-220">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="745ca-221">Indica se uma resposta a uma mensagem de email é solicitada.</span><span class="sxs-lookup"><span data-stu-id="745ca-221">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="745ca-222">References</span><span class="sxs-lookup"><span data-stu-id="745ca-222">References</span></span>](references.md) <br/> |<span data-ttu-id="745ca-223">Representa o cabeçalho da Usenet que é usado para correlacionar respostas com suas mensagens originais.</span><span class="sxs-lookup"><span data-stu-id="745ca-223">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="745ca-224">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="745ca-224">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="745ca-225">Identifica um conjunto de endereços para os quais as respostas devem ser enviadas.</span><span class="sxs-lookup"><span data-stu-id="745ca-225">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="745ca-226">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="745ca-226">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="745ca-227">Representa o item de calendário associado a um [MeetingMessage](meetingmessage.md).</span><span class="sxs-lookup"><span data-stu-id="745ca-227">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="745ca-228">IsDelegated foi removida</span><span class="sxs-lookup"><span data-stu-id="745ca-228">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="745ca-229">Indica se uma reunião foi tratada por uma conta com acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="745ca-229">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="745ca-230">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="745ca-230">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="745ca-231">Indica se uma mensagem de reunião está desatualizada.</span><span class="sxs-lookup"><span data-stu-id="745ca-231">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="745ca-232">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="745ca-232">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="745ca-233">Indica se um item de mensagem de reunião foi processado.</span><span class="sxs-lookup"><span data-stu-id="745ca-233">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="745ca-234">ResponseType</span><span class="sxs-lookup"><span data-stu-id="745ca-234">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="745ca-235">Representa o tipo de resposta de destinatário recebido para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="745ca-235">Represents the type of recipient response received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="745ca-236">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="745ca-236">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="745ca-237">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="745ca-237">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="745ca-238">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="745ca-238">This element is read-only.</span></span> <span data-ttu-id="745ca-239">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="745ca-239">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="745ca-240">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="745ca-240">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="745ca-241">Identifica o representante em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="745ca-241">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="745ca-242">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="745ca-242">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="745ca-243">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="745ca-243">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="745ca-244">Identifica o principal em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="745ca-244">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="745ca-245">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="745ca-245">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="745ca-246">UID</span><span class="sxs-lookup"><span data-stu-id="745ca-246">UID</span></span>](uid.md) <br/> |<span data-ttu-id="745ca-247">Identifica um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="745ca-247">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="745ca-248">RecurrenceType</span><span class="sxs-lookup"><span data-stu-id="745ca-248">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="745ca-249">Usada para identificar uma instância específica de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="745ca-249">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="745ca-250">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="745ca-250">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="745ca-251">Indica a data e a hora em que uma instância de um objeto iCalendar foi criada.</span><span class="sxs-lookup"><span data-stu-id="745ca-251">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="745ca-252">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="745ca-252">Parent elements</span></span>

|<span data-ttu-id="745ca-253">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="745ca-253">**Element**</span></span>|<span data-ttu-id="745ca-254">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="745ca-254">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="745ca-255">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="745ca-255">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="745ca-256">Identifica todos os itens de calendário adjacentes a um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="745ca-256">Identifies all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="745ca-257">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="745ca-257">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="745ca-258">Identifica os dados a serem acrescentados a uma única propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="745ca-258">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="745ca-259">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="745ca-259">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="745ca-260">Identifica todos os itens que entram em conflito com um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="745ca-260">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="745ca-261">Create (issync)</span><span class="sxs-lookup"><span data-stu-id="745ca-261">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="745ca-262">Identifica um único item a ser criado no armazenamento do cliente local.</span><span class="sxs-lookup"><span data-stu-id="745ca-262">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="745ca-263">Itens</span><span class="sxs-lookup"><span data-stu-id="745ca-263">Items</span></span>](items.md) <br/> |<span data-ttu-id="745ca-264">Contém uma matriz de itens.</span><span class="sxs-lookup"><span data-stu-id="745ca-264">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="745ca-265">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="745ca-265">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="745ca-266">Contém uma matriz de itens a serem criados.</span><span class="sxs-lookup"><span data-stu-id="745ca-266">Contains an array of items to create.</span></span>  <br/> |
|[<span data-ttu-id="745ca-267">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="745ca-267">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="745ca-268">Representa um item do Exchange anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="745ca-268">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="745ca-269">Setitemfield</span><span class="sxs-lookup"><span data-stu-id="745ca-269">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="745ca-270">Representa uma atualização de uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="745ca-270">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="745ca-271">Atualização (issync)</span><span class="sxs-lookup"><span data-stu-id="745ca-271">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="745ca-272">Identifica um único item a ser atualizado no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="745ca-272">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="745ca-273">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="745ca-273">Text value</span></span>

<span data-ttu-id="745ca-274">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="745ca-274">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="745ca-275">Comentários</span><span class="sxs-lookup"><span data-stu-id="745ca-275">Remarks</span></span>

<span data-ttu-id="745ca-276">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="745ca-276">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="745ca-277">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="745ca-277">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="745ca-278">Namespace</span><span class="sxs-lookup"><span data-stu-id="745ca-278">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="745ca-279">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="745ca-279">Schema Name</span></span>  <br/> |<span data-ttu-id="745ca-280">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="745ca-280">Types schema</span></span>  <br/> |
|<span data-ttu-id="745ca-281">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="745ca-281">Validation File</span></span>  <br/> |<span data-ttu-id="745ca-282">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="745ca-282">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="745ca-283">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="745ca-283">Can be Empty</span></span>  <br/> |<span data-ttu-id="745ca-284">False</span><span class="sxs-lookup"><span data-stu-id="745ca-284">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="745ca-285">Confira também</span><span class="sxs-lookup"><span data-stu-id="745ca-285">See also</span></span>



- [<span data-ttu-id="745ca-286">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="745ca-286">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

