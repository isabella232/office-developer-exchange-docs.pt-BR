---
title: PostItem
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
description: O elemento PostItem representa um item de postagem no armazenamento do Exchange.
ms.openlocfilehash: 3fb6d6cfe334999c93ca0238547dd5aee8150a5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824866"
---
# <a name="postitem"></a><span data-ttu-id="7e0f4-103">PostItem</span><span class="sxs-lookup"><span data-stu-id="7e0f4-103">PostItem</span></span>

<span data-ttu-id="7e0f4-104">O elemento **PostItem** representa um item de postagem no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-104">The **PostItem** element represents a post item in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="7e0f4-105">**PostItemType**</span><span class="sxs-lookup"><span data-stu-id="7e0f4-105">**PostItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e0f4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7e0f4-106">Attributes and elements</span></span>

<span data-ttu-id="7e0f4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e0f4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7e0f4-108">Attributes</span></span>

<span data-ttu-id="7e0f4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e0f4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7e0f4-110">Child elements</span></span>

|<span data-ttu-id="7e0f4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7e0f4-111">**Element**</span></span>|<span data-ttu-id="7e0f4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e0f4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e0f4-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="7e0f4-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="7e0f4-114">Contém o fluxo de email extensões MIME (Multipurpose Internet) nativo de um objeto que é representado no formato base64Binary.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="7e0f4-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="7e0f4-116">Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="7e0f4-117">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="7e0f4-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="7e0f4-119">Representa o identificador da pasta pai que contém o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="7e0f4-120">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="7e0f4-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="7e0f4-122">Representa a classe de mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-123">Assunto</span><span class="sxs-lookup"><span data-stu-id="7e0f4-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="7e0f4-124">Representa o assunto para armazenar itens do Exchange e objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="7e0f4-125">O assunto é limitado a 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="7e0f4-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="7e0f4-127">Indica o nível de sensibilidade de um item.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-128">Corpo</span><span class="sxs-lookup"><span data-stu-id="7e0f4-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="7e0f4-129">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-130">Anexos</span><span class="sxs-lookup"><span data-stu-id="7e0f4-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7e0f4-131">Contém os itens ou arquivos que estejam anexados a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="7e0f4-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="7e0f4-133">Representa a data e hora em que um item em uma caixa de correio foi recebido.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-134">Size</span><span class="sxs-lookup"><span data-stu-id="7e0f4-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="7e0f4-135">Representa o tamanho em bytes de um item.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="7e0f4-136">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-137">Categorias</span><span class="sxs-lookup"><span data-stu-id="7e0f4-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7e0f4-138">Representa uma coleção de cadeias de caracteres que identificam as categorias para o qual um item na caixa de correio pertence.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-138">Represents a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-139">Importância</span><span class="sxs-lookup"><span data-stu-id="7e0f4-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="7e0f4-140">Descreve a importância de um item.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="7e0f4-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="7e0f4-142">Representa o identificador do item ao qual este item é uma resposta.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="7e0f4-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="7e0f4-144">Indica se um item foi enviado à pasta padrão caixa de saída.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="7e0f4-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="7e0f4-146">Indica se um item ainda não foi enviado.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="7e0f4-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="7e0f4-148">Indica se um usuário enviada a um item para si mesmo.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="7e0f4-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="7e0f4-150">Indica se o item anteriormente foi enviado.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="7e0f4-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="7e0f4-152">Indica se o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="7e0f4-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="7e0f4-154">Representa a coleção de todos os cabeçalhos de mensagem da Internet que estão contidos em um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-154">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="7e0f4-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="7e0f4-156">Representa a data e hora em que um item em uma caixa de correio foi enviado.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="7e0f4-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="7e0f4-158">Representa a data e hora em que um determinado item na caixa de correio foi criado.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="7e0f4-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="7e0f4-160">Contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="7e0f4-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="7e0f4-162">Representa a data e hora quando o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="7e0f4-163">Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="7e0f4-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="7e0f4-165">Indica se um lembrete tiver sido definido para um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="7e0f4-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="7e0f4-167">Representa o número de minutos antes de um evento, quando um lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="7e0f4-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="7e0f4-169">Representa a cadeia de caracteres de exibição que é usada para o conteúdo da caixa Cc.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="7e0f4-170">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição destinatários Cc.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="7e0f4-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="7e0f4-172">Representa a cadeia de caracteres de exibição que é usada para o conteúdo da caixa para.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="7e0f4-173">Esta é a cadeia de caracteres concatenada de todos os aos nomes de exibição do destinatário.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="7e0f4-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="7e0f4-175">Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-175">Represents a property that is set to **true** if an item has at least one attachment.</span></span> <span data-ttu-id="7e0f4-176">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="7e0f4-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="7e0f4-178">Identifica as propriedades estendidas em pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-179">Cultura</span><span class="sxs-lookup"><span data-stu-id="7e0f4-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="7e0f4-180">Representa a cultura de um determinado item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-181">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="7e0f4-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="7e0f4-182">Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-182">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="7e0f4-183">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-183">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-184">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="7e0f4-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="7e0f4-185">Contém o nome de exibição do último usuário para modificar um item.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="7e0f4-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="7e0f4-187">Indica quando um item da última modificação.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-188">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="7e0f4-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="7e0f4-189">Indica se o item está associado a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-190">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="7e0f4-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="7e0f4-191">Representa uma URL para concatenar no ponto de extremidade do Microsoft Office Outlook Web App para ler um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-192">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="7e0f4-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="7e0f4-193">Representa uma URL para concatenar no ponto de extremidade do Outlook Web App para editar um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="7e0f4-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="7e0f4-195">Contém o identificador de um item ou conversa.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="7e0f4-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="7e0f4-197">Representa um fragmento HTML ou texto sem formatação que representa um único corpo da conversa.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-198">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="7e0f4-198">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="7e0f4-199">Contém uma ID binária que representa o segmento ao qual esta mensagem pertence.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-199">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-200">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="7e0f4-200">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="7e0f4-201">Representa o identificador de conversa.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-201">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-202">From</span><span class="sxs-lookup"><span data-stu-id="7e0f4-202">From</span></span>](from.md) <br/> |<span data-ttu-id="7e0f4-203">Representa o endereço do qual o item de postagem foi enviado.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-203">Represents the address from which the post item was sent.</span></span> <span data-ttu-id="7e0f4-204">O elemento **de** só pode ser definido no momento da criação.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-204">The **From** element can only be set at creation time.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-205">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="7e0f4-205">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="7e0f4-206">Representa o identificador de mensagem da Internet de um item.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-206">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-207">Foi lido</span><span class="sxs-lookup"><span data-stu-id="7e0f4-207">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="7e0f4-208">Indica se uma mensagem foi lido.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-208">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-209">PostedTime</span><span class="sxs-lookup"><span data-stu-id="7e0f4-209">PostedTime</span></span>](postedtime.md) <br/> |<span data-ttu-id="7e0f4-210">Representa a hora em que um [PostItem](postitem.md) postado.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-210">Represents the time that a [PostItem](postitem.md) was posted.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-211">Referências</span><span class="sxs-lookup"><span data-stu-id="7e0f4-211">References</span></span>](references.md) <br/> |<span data-ttu-id="7e0f4-212">Representa o cabeçalho Usenet que é usado para associar respostas a mensagens originais.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-212">Represents the Usenet header that is used to associate replies with the original messages.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-213">Sender</span><span class="sxs-lookup"><span data-stu-id="7e0f4-213">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="7e0f4-214">Identifica o remetente de um item.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-214">Identifies the sender of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7e0f4-215">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7e0f4-215">Parent elements</span></span>

|<span data-ttu-id="7e0f4-216">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7e0f4-216">**Element**</span></span>|<span data-ttu-id="7e0f4-217">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e0f4-217">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e0f4-218">SetItemField</span><span class="sxs-lookup"><span data-stu-id="7e0f4-218">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="7e0f4-219">Representa uma atualização para uma única propriedade de um item em uma operação UpdateItem.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-219">Represents an update to a single property of an item in an UpdateItem operation.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-220">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="7e0f4-220">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="7e0f4-221">Identifica os dados a serem acrescentados a uma única propriedade de um item ou pasta durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="7e0f4-221">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-222">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="7e0f4-222">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="7e0f4-223">Representa um item do Exchange que está anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-223">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-224">Criar (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="7e0f4-224">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="7e0f4-225">Identifica um único item para criar no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-225">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-226">Atualização (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="7e0f4-226">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="7e0f4-227">Identifica um único item a ser atualizado no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-227">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-228">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="7e0f4-228">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="7e0f4-229">Retornados em respostas [SyncFolderItems](syncfolderitems.md) quando um item foi lido.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-229">Returned in [SyncFolderItems](syncfolderitems.md) responses when an item has been read.</span></span> <span data-ttu-id="7e0f4-230">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-230">This property is read-only.</span></span> <span data-ttu-id="7e0f4-231">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-231">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-232">Items</span><span class="sxs-lookup"><span data-stu-id="7e0f4-232">Items</span></span>](items.md) <br/> |<span data-ttu-id="7e0f4-233">Contém uma matriz de itens.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-233">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-234">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="7e0f4-234">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="7e0f4-235">Identifica todos os itens que estão em conflito com um tempo de reunião.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-235">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="7e0f4-236">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="7e0f4-236">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="7e0f4-237">Descreve todos os itens de calendário que são adjacentes para um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-237">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7e0f4-238">Text value</span><span class="sxs-lookup"><span data-stu-id="7e0f4-238">Text value</span></span>

<span data-ttu-id="7e0f4-239">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-239">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7e0f4-240">Comentários</span><span class="sxs-lookup"><span data-stu-id="7e0f4-240">Remarks</span></span>

<span data-ttu-id="7e0f4-241">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e0f4-241">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e0f4-242">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7e0f4-242">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e0f4-243">Namespace</span><span class="sxs-lookup"><span data-stu-id="7e0f4-243">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e0f4-244">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7e0f4-244">Schema Name</span></span>  <br/> |<span data-ttu-id="7e0f4-245">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7e0f4-245">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e0f4-246">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7e0f4-246">Validation File</span></span>  <br/> |<span data-ttu-id="7e0f4-247">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e0f4-247">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e0f4-248">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7e0f4-248">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e0f4-249">False</span><span class="sxs-lookup"><span data-stu-id="7e0f4-249">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e0f4-250">Ver também</span><span class="sxs-lookup"><span data-stu-id="7e0f4-250">See also</span></span>



- [<span data-ttu-id="7e0f4-251">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7e0f4-251">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

