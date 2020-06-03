---
title: Item de postagem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostItem
api_type:
- schema
ms.assetid: 7727ed84-9591-4a1c-bb04-12129926499b
description: O elemento PostItem representa um item de postagem no repositório do Exchange.
ms.openlocfilehash: 5fba1a9a6a3abc95ea2ce65cafa2b62bc7423f28
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528864"
---
# <a name="postitem"></a><span data-ttu-id="af11d-103">Item de postagem</span><span class="sxs-lookup"><span data-stu-id="af11d-103">PostItem</span></span>

<span data-ttu-id="af11d-104">O elemento **PostItem** representa um item de postagem no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="af11d-104">The **PostItem** element represents a post item in the Exchange store.</span></span> 
  
```xml
<PostItem>
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
   <ConversationIndex/>
   <ConversationTopic/>
   <From/>
   <InternetMessageId/>
   <IsRead/>
   <PostedTime/>
   <References/>
   <Sender/>
</PostItem>
```

 <span data-ttu-id="af11d-105">**PostItem**</span><span class="sxs-lookup"><span data-stu-id="af11d-105">**PostItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af11d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="af11d-106">Attributes and elements</span></span>

<span data-ttu-id="af11d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="af11d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af11d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="af11d-108">Attributes</span></span>

<span data-ttu-id="af11d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af11d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af11d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="af11d-110">Child elements</span></span>

|<span data-ttu-id="af11d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="af11d-111">**Element**</span></span>|<span data-ttu-id="af11d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="af11d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af11d-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="af11d-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="af11d-114">Contém o fluxo MIME (Multipurpose Internet Mail Extensions) nativo de um objeto representado no formato base64Binary.</span><span class="sxs-lookup"><span data-stu-id="af11d-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="af11d-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="af11d-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="af11d-116">Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="af11d-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="af11d-117">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af11d-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="af11d-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="af11d-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="af11d-119">Representa o identificador da pasta pai que contém o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="af11d-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="af11d-120">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af11d-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="af11d-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="af11d-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="af11d-122">Representa a classe de mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="af11d-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="af11d-123">Assunto</span><span class="sxs-lookup"><span data-stu-id="af11d-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="af11d-124">Representa o assunto de itens do repositório do Exchange e objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="af11d-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="af11d-125">O assunto está limitado a 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="af11d-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="af11d-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="af11d-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="af11d-127">Indica o nível de sensibilidade de um item.</span><span class="sxs-lookup"><span data-stu-id="af11d-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="af11d-128">Body</span><span class="sxs-lookup"><span data-stu-id="af11d-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="af11d-129">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="af11d-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="af11d-130">Anexos</span><span class="sxs-lookup"><span data-stu-id="af11d-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="af11d-131">Contém os itens ou arquivos anexados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="af11d-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="af11d-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="af11d-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="af11d-133">Representa a data e a hora em que um item foi recebido em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="af11d-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="af11d-134">Tamanho</span><span class="sxs-lookup"><span data-stu-id="af11d-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="af11d-135">Representa o tamanho em bytes de um item.</span><span class="sxs-lookup"><span data-stu-id="af11d-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="af11d-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af11d-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="af11d-137">Categorias</span><span class="sxs-lookup"><span data-stu-id="af11d-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="af11d-138">Representa uma coleção de cadeias de caracteres que identificam as categorias às quais um item na caixa de correio pertence.</span><span class="sxs-lookup"><span data-stu-id="af11d-138">Represents a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="af11d-139">Importance</span><span class="sxs-lookup"><span data-stu-id="af11d-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="af11d-140">Descreve a importância de um item.</span><span class="sxs-lookup"><span data-stu-id="af11d-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="af11d-141">Inresponderto</span><span class="sxs-lookup"><span data-stu-id="af11d-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="af11d-142">Representa o identificador do item para o qual este item é uma resposta.</span><span class="sxs-lookup"><span data-stu-id="af11d-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="af11d-143">Isenviado</span><span class="sxs-lookup"><span data-stu-id="af11d-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="af11d-144">Indica se um item foi enviado para a pasta padrão da pasta de saída.</span><span class="sxs-lookup"><span data-stu-id="af11d-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="af11d-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="af11d-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="af11d-146">Indica se um item ainda não foi enviado.</span><span class="sxs-lookup"><span data-stu-id="af11d-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="af11d-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="af11d-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="af11d-148">Indica se um usuário enviou um item para ele.</span><span class="sxs-lookup"><span data-stu-id="af11d-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="af11d-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="af11d-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="af11d-150">Indica se o item foi enviado anteriormente.</span><span class="sxs-lookup"><span data-stu-id="af11d-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="af11d-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="af11d-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="af11d-152">Indica se o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="af11d-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="af11d-153">Propriedadeinternetmessageheaders</span><span class="sxs-lookup"><span data-stu-id="af11d-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="af11d-154">Representa a coleção de todos os cabeçalhos de mensagens da Internet contidos em um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="af11d-154">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="af11d-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="af11d-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="af11d-156">Representa a data e a hora em que um item em uma caixa de correio foi enviado.</span><span class="sxs-lookup"><span data-stu-id="af11d-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="af11d-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="af11d-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="af11d-158">Representa a data e a hora em que um determinado item da caixa de correio foi criado.</span><span class="sxs-lookup"><span data-stu-id="af11d-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="af11d-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="af11d-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="af11d-160">Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="af11d-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="af11d-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="af11d-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="af11d-162">Representa a data e a hora em que o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="af11d-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="af11d-163">Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="af11d-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="af11d-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="af11d-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="af11d-165">Indica se um lembrete foi definido para um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="af11d-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="af11d-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="af11d-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="af11d-167">Representa o número de minutos antes de um evento quando um lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="af11d-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="af11d-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="af11d-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="af11d-169">Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa CC.</span><span class="sxs-lookup"><span data-stu-id="af11d-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="af11d-170">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários CC.</span><span class="sxs-lookup"><span data-stu-id="af11d-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="af11d-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="af11d-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="af11d-172">Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa para.</span><span class="sxs-lookup"><span data-stu-id="af11d-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="af11d-173">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários.</span><span class="sxs-lookup"><span data-stu-id="af11d-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="af11d-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="af11d-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="af11d-175">Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="af11d-175">Represents a property that is set to **true** if an item has at least one attachment.</span></span> <span data-ttu-id="af11d-176">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af11d-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="af11d-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="af11d-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="af11d-178">Identifica as propriedades estendidas em pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="af11d-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="af11d-179">Cultura</span><span class="sxs-lookup"><span data-stu-id="af11d-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="af11d-180">Representa a cultura de um determinado item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="af11d-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="af11d-181">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="af11d-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="af11d-182">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="af11d-182">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="af11d-183">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af11d-183">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="af11d-184">LastModified</span><span class="sxs-lookup"><span data-stu-id="af11d-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="af11d-185">Contém o nome de exibição do último usuário a modificar um item.</span><span class="sxs-lookup"><span data-stu-id="af11d-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="af11d-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="af11d-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="af11d-187">Indica quando um item foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="af11d-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="af11d-188">Isassociated</span><span class="sxs-lookup"><span data-stu-id="af11d-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="af11d-189">Indica se o item está associado a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="af11d-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="af11d-190">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="af11d-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="af11d-191">Representa uma URL para concatenar ao ponto de extremidade do Microsoft Office Outlook Web App para ler um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="af11d-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="af11d-192">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="af11d-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="af11d-193">Representa uma URL para concatenar ao ponto de extremidade do Outlook Web App para editar um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="af11d-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="af11d-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="af11d-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="af11d-195">Contém o identificador de um item ou uma conversa.</span><span class="sxs-lookup"><span data-stu-id="af11d-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="af11d-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="af11d-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="af11d-197">Representa um fragmento HTML ou texto sem formatação que representa o corpo exclusivo desta conversa.</span><span class="sxs-lookup"><span data-stu-id="af11d-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="af11d-198">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="af11d-198">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="af11d-199">Contém uma ID binária que representa o thread ao qual esta mensagem pertence.</span><span class="sxs-lookup"><span data-stu-id="af11d-199">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="af11d-200">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="af11d-200">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="af11d-201">Representa o identificador de conversa.</span><span class="sxs-lookup"><span data-stu-id="af11d-201">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="af11d-202">De</span><span class="sxs-lookup"><span data-stu-id="af11d-202">From</span></span>](from.md) <br/> |<span data-ttu-id="af11d-203">Representa o endereço a partir do qual o item de postagem foi enviado.</span><span class="sxs-lookup"><span data-stu-id="af11d-203">Represents the address from which the post item was sent.</span></span> <span data-ttu-id="af11d-204">O elemento **from** só pode ser definido no momento da criação.</span><span class="sxs-lookup"><span data-stu-id="af11d-204">The **From** element can only be set at creation time.</span></span>  <br/> |
|[<span data-ttu-id="af11d-205">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="af11d-205">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="af11d-206">Representa o identificador de mensagem da Internet de um item.</span><span class="sxs-lookup"><span data-stu-id="af11d-206">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="af11d-207">IsRead</span><span class="sxs-lookup"><span data-stu-id="af11d-207">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="af11d-208">Indica se uma mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="af11d-208">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="af11d-209">Postadotime</span><span class="sxs-lookup"><span data-stu-id="af11d-209">PostedTime</span></span>](postedtime.md) <br/> |<span data-ttu-id="af11d-210">Representa o horário de lançamento de um [Item](postitem.md) .</span><span class="sxs-lookup"><span data-stu-id="af11d-210">Represents the time that a [PostItem](postitem.md) was posted.</span></span>  <br/> |
|[<span data-ttu-id="af11d-211">References</span><span class="sxs-lookup"><span data-stu-id="af11d-211">References</span></span>](references.md) <br/> |<span data-ttu-id="af11d-212">Representa o cabeçalho da Usenet que é usado para associar respostas com as mensagens originais.</span><span class="sxs-lookup"><span data-stu-id="af11d-212">Represents the Usenet header that is used to associate replies with the original messages.</span></span>  <br/> |
|[<span data-ttu-id="af11d-213">Sender</span><span class="sxs-lookup"><span data-stu-id="af11d-213">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="af11d-214">Identifica o remetente de um item.</span><span class="sxs-lookup"><span data-stu-id="af11d-214">Identifies the sender of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="af11d-215">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="af11d-215">Parent elements</span></span>

|<span data-ttu-id="af11d-216">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="af11d-216">**Element**</span></span>|<span data-ttu-id="af11d-217">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="af11d-217">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af11d-218">Setitemfield</span><span class="sxs-lookup"><span data-stu-id="af11d-218">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="af11d-219">Representa uma atualização de uma única propriedade de um item em uma operação UpdateItem.</span><span class="sxs-lookup"><span data-stu-id="af11d-219">Represents an update to a single property of an item in an UpdateItem operation.</span></span>  <br/> |
|[<span data-ttu-id="af11d-220">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="af11d-220">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="af11d-221">Identifica os dados a serem acrescentados a uma única propriedade de um item ou pasta durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="af11d-221">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="af11d-222">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="af11d-222">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="af11d-223">Representa um item do Exchange anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="af11d-223">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="af11d-224">Create (issync)</span><span class="sxs-lookup"><span data-stu-id="af11d-224">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="af11d-225">Identifica um único item a ser criado no armazenamento do cliente local.</span><span class="sxs-lookup"><span data-stu-id="af11d-225">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="af11d-226">Atualização (issync)</span><span class="sxs-lookup"><span data-stu-id="af11d-226">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="af11d-227">Identifica um único item a ser atualizado no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="af11d-227">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="af11d-228">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="af11d-228">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="af11d-229">Retornado em respostas [SyncFolderItems](syncfolderitems.md) quando um item foi lido.</span><span class="sxs-lookup"><span data-stu-id="af11d-229">Returned in [SyncFolderItems](syncfolderitems.md) responses when an item has been read.</span></span> <span data-ttu-id="af11d-230">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af11d-230">This property is read-only.</span></span> <span data-ttu-id="af11d-231">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="af11d-231">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="af11d-232">Itens</span><span class="sxs-lookup"><span data-stu-id="af11d-232">Items</span></span>](items.md) <br/> |<span data-ttu-id="af11d-233">Contém uma matriz de itens.</span><span class="sxs-lookup"><span data-stu-id="af11d-233">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="af11d-234">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="af11d-234">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="af11d-235">Identifica todos os itens que entram em conflito com um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="af11d-235">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="af11d-236">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="af11d-236">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="af11d-237">Descreve todos os itens de calendário adjacentes a um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="af11d-237">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="af11d-238">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="af11d-238">Text value</span></span>

<span data-ttu-id="af11d-239">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="af11d-239">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="af11d-240">Comentários</span><span class="sxs-lookup"><span data-stu-id="af11d-240">Remarks</span></span>

<span data-ttu-id="af11d-241">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="af11d-241">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af11d-242">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="af11d-242">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af11d-243">Namespace</span><span class="sxs-lookup"><span data-stu-id="af11d-243">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="af11d-244">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="af11d-244">Schema Name</span></span>  <br/> |<span data-ttu-id="af11d-245">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="af11d-245">Types schema</span></span>  <br/> |
|<span data-ttu-id="af11d-246">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="af11d-246">Validation File</span></span>  <br/> |<span data-ttu-id="af11d-247">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="af11d-247">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="af11d-248">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="af11d-248">Can be Empty</span></span>  <br/> |<span data-ttu-id="af11d-249">False</span><span class="sxs-lookup"><span data-stu-id="af11d-249">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af11d-250">Confira também</span><span class="sxs-lookup"><span data-stu-id="af11d-250">See also</span></span>



- [<span data-ttu-id="af11d-251">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="af11d-251">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

