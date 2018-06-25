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
description: O elemento MeetingCancellation representa o cancelamento da reunião no armazenamento do Exchange.
ms.openlocfilehash: b68135e2743c675bed92c54172369c2ef21f1a6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824447"
---
# <a name="meetingcancellation"></a><span data-ttu-id="c1050-103">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="c1050-103">MeetingCancellation</span></span>

<span data-ttu-id="c1050-104">O elemento **MeetingCancellation** representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1050-104">The **MeetingCancellation** element represents a meeting cancellation in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="c1050-105">**MeetingCancellationMessageType**</span><span class="sxs-lookup"><span data-stu-id="c1050-105">**MeetingCancellationMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c1050-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c1050-106">Attributes and elements</span></span>

<span data-ttu-id="c1050-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c1050-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c1050-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c1050-108">Attributes</span></span>

<span data-ttu-id="c1050-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c1050-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c1050-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c1050-110">Child elements</span></span>

|<span data-ttu-id="c1050-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c1050-111">**Element**</span></span>|<span data-ttu-id="c1050-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c1050-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1050-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="c1050-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="c1050-114">Contém o fluxo MIME nativo de um objeto que é representado no formato base64Binary.</span><span class="sxs-lookup"><span data-stu-id="c1050-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="c1050-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="c1050-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="c1050-116">Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1050-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="c1050-117">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1050-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c1050-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="c1050-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="c1050-119">Representa o identificador da pasta pai que contém o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="c1050-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="c1050-120">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1050-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c1050-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="c1050-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="c1050-122">Representa a classe de mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="c1050-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="c1050-123">Assunto</span><span class="sxs-lookup"><span data-stu-id="c1050-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="c1050-124">Representa o assunto para armazenar itens do Exchange e objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="c1050-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="c1050-125">O assunto é limitado a 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="c1050-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="c1050-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="c1050-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="c1050-127">Indica o nível de sensibilidade de um item.</span><span class="sxs-lookup"><span data-stu-id="c1050-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="c1050-128">Corpo</span><span class="sxs-lookup"><span data-stu-id="c1050-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="c1050-129">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="c1050-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="c1050-130">Anexos</span><span class="sxs-lookup"><span data-stu-id="c1050-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c1050-131">Contém os itens ou arquivos que estejam anexados a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1050-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c1050-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="c1050-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="c1050-133">Representa a data e hora em que um item em uma caixa de correio foi recebido.</span><span class="sxs-lookup"><span data-stu-id="c1050-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="c1050-134">Size</span><span class="sxs-lookup"><span data-stu-id="c1050-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="c1050-135">Representa o tamanho em bytes de um item.</span><span class="sxs-lookup"><span data-stu-id="c1050-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="c1050-136">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1050-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c1050-137">Categorias</span><span class="sxs-lookup"><span data-stu-id="c1050-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c1050-138">Representa uma coleção de cadeias de caracteres que identificam a quais categorias de um item na caixa de correio pertence.</span><span class="sxs-lookup"><span data-stu-id="c1050-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="c1050-139">Importância</span><span class="sxs-lookup"><span data-stu-id="c1050-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="c1050-140">Descreve a importância de um item.</span><span class="sxs-lookup"><span data-stu-id="c1050-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="c1050-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="c1050-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="c1050-142">Representa o identificador do item ao qual este item é uma resposta.</span><span class="sxs-lookup"><span data-stu-id="c1050-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="c1050-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="c1050-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="c1050-144">Indica se um item foi enviado à pasta padrão caixa de saída.</span><span class="sxs-lookup"><span data-stu-id="c1050-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="c1050-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="c1050-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="c1050-146">Indica se um item ainda não foi enviado.</span><span class="sxs-lookup"><span data-stu-id="c1050-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="c1050-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="c1050-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="c1050-148">Indica se um usuário enviada a um item para si mesmo.</span><span class="sxs-lookup"><span data-stu-id="c1050-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="c1050-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="c1050-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="c1050-150">Indica se o item anteriormente foi enviado.</span><span class="sxs-lookup"><span data-stu-id="c1050-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="c1050-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="c1050-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="c1050-152">Indica se o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="c1050-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="c1050-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="c1050-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="c1050-154">Representa a coleção de todos os cabeçalhos de mensagem da Internet que está contido dentro de um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c1050-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c1050-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="c1050-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="c1050-156">Representa a data e hora em que um item em uma caixa de correio foi enviado.</span><span class="sxs-lookup"><span data-stu-id="c1050-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="c1050-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="c1050-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="c1050-158">Representa a data e hora em que um determinado item na caixa de correio foi criado.</span><span class="sxs-lookup"><span data-stu-id="c1050-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="c1050-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="c1050-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="c1050-160">Contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1050-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c1050-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="c1050-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="c1050-162">Representa a data e hora quando o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="c1050-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="c1050-163">Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="c1050-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="c1050-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="c1050-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="c1050-165">Indica se um lembrete tiver sido definido para um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1050-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c1050-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="c1050-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="c1050-167">Representa o número de minutos antes de um evento que um lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="c1050-167">Represents the number of minutes before an event that a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="c1050-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="c1050-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="c1050-169">Representa a cadeia de caracteres de exibição que é usada para o conteúdo da caixa Cc.</span><span class="sxs-lookup"><span data-stu-id="c1050-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="c1050-170">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição destinatários Cc.</span><span class="sxs-lookup"><span data-stu-id="c1050-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="c1050-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="c1050-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="c1050-172">Representa a cadeia de caracteres de exibição que é usada para o conteúdo da caixa para.</span><span class="sxs-lookup"><span data-stu-id="c1050-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="c1050-173">Esta é a cadeia de caracteres concatenada de todos os aos nomes de exibição do destinatário.</span><span class="sxs-lookup"><span data-stu-id="c1050-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="c1050-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="c1050-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="c1050-175">Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo visível.</span><span class="sxs-lookup"><span data-stu-id="c1050-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="c1050-176">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1050-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c1050-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="c1050-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="c1050-178">Identifica as propriedades estendidas em pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="c1050-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="c1050-179">Cultura</span><span class="sxs-lookup"><span data-stu-id="c1050-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="c1050-180">Representa a cultura de um determinado item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c1050-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c1050-181">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="c1050-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="c1050-182">Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="c1050-182">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="c1050-183">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1050-183">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c1050-184">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="c1050-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="c1050-185">Contém o nome de exibição do último usuário para modificar um item.</span><span class="sxs-lookup"><span data-stu-id="c1050-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="c1050-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="c1050-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="c1050-187">Indica quando um item da última modificação.</span><span class="sxs-lookup"><span data-stu-id="c1050-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="c1050-188">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="c1050-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="c1050-189">Indica se o item está associado a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="c1050-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="c1050-190">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="c1050-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="c1050-191">Representa uma URL para concatenar no ponto de extremidade do Microsoft Office Outlook Web App para ler um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="c1050-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="c1050-192">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="c1050-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="c1050-193">Representa uma URL para concatenar no ponto de extremidade do Outlook Web App para editar um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="c1050-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="c1050-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="c1050-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="c1050-195">Contém o identificador de um item ou conversa.</span><span class="sxs-lookup"><span data-stu-id="c1050-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="c1050-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="c1050-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="c1050-197">Representa um fragmento HTML ou texto sem formatação que representa um único corpo da conversa.</span><span class="sxs-lookup"><span data-stu-id="c1050-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="c1050-198">Sender</span><span class="sxs-lookup"><span data-stu-id="c1050-198">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="c1050-199">Identifica o remetente de um item.</span><span class="sxs-lookup"><span data-stu-id="c1050-199">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="c1050-200">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="c1050-200">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="c1050-201">Contém um conjunto de destinatários de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="c1050-201">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="c1050-202">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="c1050-202">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="c1050-203">Representa uma coleção dos destinatários que receberão uma cópia da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c1050-203">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="c1050-204">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="c1050-204">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="c1050-205">Representa uma coleção de destinatários para receber uma cópia oculta (Cco) de um email.</span><span class="sxs-lookup"><span data-stu-id="c1050-205">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="c1050-206">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="c1050-206">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="c1050-207">Indica se o remetente de um item solicita uma confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="c1050-207">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="c1050-208">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="c1050-208">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="c1050-209">Indica se o remetente de um item solicita uma confirmação de entrega.</span><span class="sxs-lookup"><span data-stu-id="c1050-209">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="c1050-210">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="c1050-210">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="c1050-211">Contém uma ID binária que representa o segmento ao qual esta mensagem pertence.</span><span class="sxs-lookup"><span data-stu-id="c1050-211">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="c1050-212">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="c1050-212">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="c1050-213">Representa o identificador de conversa.</span><span class="sxs-lookup"><span data-stu-id="c1050-213">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="c1050-214">From</span><span class="sxs-lookup"><span data-stu-id="c1050-214">From</span></span>](from.md) <br/> |<span data-ttu-id="c1050-215">Representa o destinatário de quem a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="c1050-215">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="c1050-216">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="c1050-216">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="c1050-217">Representa o identificador de mensagem da Internet de um item.</span><span class="sxs-lookup"><span data-stu-id="c1050-217">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="c1050-218">Foi lido</span><span class="sxs-lookup"><span data-stu-id="c1050-218">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="c1050-219">Indica se uma mensagem foi lido.</span><span class="sxs-lookup"><span data-stu-id="c1050-219">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="c1050-220">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="c1050-220">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="c1050-221">Indica se uma resposta a uma mensagem de email é solicitada.</span><span class="sxs-lookup"><span data-stu-id="c1050-221">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="c1050-222">Referências</span><span class="sxs-lookup"><span data-stu-id="c1050-222">References</span></span>](references.md) <br/> |<span data-ttu-id="c1050-223">Representa o cabeçalho de Usenet é usado para correlacionar respostas com suas mensagens originais.</span><span class="sxs-lookup"><span data-stu-id="c1050-223">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="c1050-224">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="c1050-224">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="c1050-225">Identifica um conjunto de endereços para o qual as respostas devem ser enviadas.</span><span class="sxs-lookup"><span data-stu-id="c1050-225">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="c1050-226">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="c1050-226">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="c1050-227">Representa o item de calendário que está associado um [MeetingMessage](meetingmessage.md).</span><span class="sxs-lookup"><span data-stu-id="c1050-227">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="c1050-228">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="c1050-228">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="c1050-229">Indica se uma reunião foi tratada por uma conta com acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="c1050-229">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="c1050-230">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="c1050-230">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="c1050-231">Indica se uma mensagem de reunião desatualizada.</span><span class="sxs-lookup"><span data-stu-id="c1050-231">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="c1050-232">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="c1050-232">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="c1050-233">Indica se uma mensagem de reunião item foi processada.</span><span class="sxs-lookup"><span data-stu-id="c1050-233">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="c1050-234">ResponseType</span><span class="sxs-lookup"><span data-stu-id="c1050-234">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="c1050-235">Representa o tipo de destinatário resposta recebida para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="c1050-235">Represents the type of recipient response received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="c1050-236">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="c1050-236">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="c1050-237">Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="c1050-237">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="c1050-238">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1050-238">This element is read-only.</span></span> <span data-ttu-id="c1050-239">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c1050-239">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="c1050-240">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="c1050-240">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="c1050-241">Identifica o delegado em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="c1050-241">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="c1050-242">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="c1050-242">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="c1050-243">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="c1050-243">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="c1050-244">Identifica a entidade em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="c1050-244">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="c1050-245">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="c1050-245">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="c1050-246">UID</span><span class="sxs-lookup"><span data-stu-id="c1050-246">UID</span></span>](uid.md) <br/> |<span data-ttu-id="c1050-247">Identifica um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="c1050-247">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c1050-248">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="c1050-248">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="c1050-249">Usado para identificar uma instância específica de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="c1050-249">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c1050-250">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="c1050-250">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="c1050-251">Indica a data e hora em que uma instância de um objeto iCalendar foi criada.</span><span class="sxs-lookup"><span data-stu-id="c1050-251">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c1050-252">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c1050-252">Parent elements</span></span>

|<span data-ttu-id="c1050-253">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c1050-253">**Element**</span></span>|<span data-ttu-id="c1050-254">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c1050-254">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1050-255">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="c1050-255">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="c1050-256">Identifica todos os itens de calendário que são adjacentes para um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="c1050-256">Identifies all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="c1050-257">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="c1050-257">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="c1050-258">Identifica os dados a serem acrescentados a uma única propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="c1050-258">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="c1050-259">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="c1050-259">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="c1050-260">Identifica todos os itens que estão em conflito com um tempo de reunião.</span><span class="sxs-lookup"><span data-stu-id="c1050-260">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="c1050-261">Criar (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="c1050-261">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="c1050-262">Identifica um único item para criar no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="c1050-262">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="c1050-263">Items</span><span class="sxs-lookup"><span data-stu-id="c1050-263">Items</span></span>](items.md) <br/> |<span data-ttu-id="c1050-264">Contém uma matriz de itens.</span><span class="sxs-lookup"><span data-stu-id="c1050-264">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="c1050-265">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="c1050-265">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="c1050-266">Contém uma matriz de itens para criar.</span><span class="sxs-lookup"><span data-stu-id="c1050-266">Contains an array of items to create.</span></span>  <br/> |
|[<span data-ttu-id="c1050-267">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="c1050-267">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="c1050-268">Representa um item do Exchange que está anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1050-268">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="c1050-269">SetItemField</span><span class="sxs-lookup"><span data-stu-id="c1050-269">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="c1050-270">Representa uma atualização para uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="c1050-270">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="c1050-271">Atualização (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="c1050-271">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="c1050-272">Identifica um único item a ser atualizado no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="c1050-272">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c1050-273">Text value</span><span class="sxs-lookup"><span data-stu-id="c1050-273">Text value</span></span>

<span data-ttu-id="c1050-274">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c1050-274">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c1050-275">Comentários</span><span class="sxs-lookup"><span data-stu-id="c1050-275">Remarks</span></span>

<span data-ttu-id="c1050-276">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1050-276">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c1050-277">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c1050-277">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c1050-278">Namespace</span><span class="sxs-lookup"><span data-stu-id="c1050-278">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c1050-279">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c1050-279">Schema Name</span></span>  <br/> |<span data-ttu-id="c1050-280">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c1050-280">Types schema</span></span>  <br/> |
|<span data-ttu-id="c1050-281">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c1050-281">Validation File</span></span>  <br/> |<span data-ttu-id="c1050-282">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c1050-282">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c1050-283">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c1050-283">Can be Empty</span></span>  <br/> |<span data-ttu-id="c1050-284">False</span><span class="sxs-lookup"><span data-stu-id="c1050-284">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c1050-285">Ver também</span><span class="sxs-lookup"><span data-stu-id="c1050-285">See also</span></span>



- [<span data-ttu-id="c1050-286">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c1050-286">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

