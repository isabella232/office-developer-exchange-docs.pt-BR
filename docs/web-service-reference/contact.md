---
title: Contato
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contact
api_type:
- schema
ms.assetid: 66bfff50-7a91-4d81-b6a0-610b9962f677
description: O elemento Contact representa um item de contato no repositório do Exchange.
ms.openlocfilehash: b5b4af211815dbbd09449ca2f3c6b6b2dfba6f93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44445647"
---
# <a name="contact"></a><span data-ttu-id="fc244-103">Contato</span><span class="sxs-lookup"><span data-stu-id="fc244-103">Contact</span></span>

<span data-ttu-id="fc244-104">O elemento **Contact** representa um item de contato no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc244-104">The **Contact** element represents a contact item in the Exchange store.</span></span> 
  
```XML
<Contact>
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
   <FileAs/>
   <FileAsMapping/>
   <DisplayName/>
   <GivenName/>
   <Initials/>
   <MiddleName/>
   <Nickname/>
   <CompleteName/>
   <CompanyName/>
   <EmailAddresses/>
   <PhysicalAddresses/>
   <PhoneNumbers/>
   <AssistantName/>
   <Birthday/>
   <BusinessHomePage/>
   <Children/>
   <Companies/>
   <ContactSource/>
   <Department/>
   <Generation/>
   <ImAddresses/>
   <JobTitle/>
   <Manager/>
   <Mileage/>
   <OfficeLocation/>
   <PostalAddressIndex/>
   <Profession/>
   <SpouseName/>
   <Surname/>
   <WeddingAnniversary/>
   <HasPicture/>
   <PhoneticFullName/>
   <PhoneticFirstName/>
   <PhoneticLastName/>
   <Alias/>
   <Notes/>
   <Photo/>
   <UserSMIMECertificate/>
   <MSExchangeCertificate/>
   <DirectoryId/>
   <ManagerMailbox/>
   <DirectReports/>
</Contact>
```

 <span data-ttu-id="fc244-105">**ContactItemType**</span><span class="sxs-lookup"><span data-stu-id="fc244-105">**ContactItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc244-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fc244-106">Attributes and elements</span></span>

<span data-ttu-id="fc244-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fc244-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc244-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fc244-108">Attributes</span></span>

<span data-ttu-id="fc244-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc244-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc244-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fc244-110">Child elements</span></span>

|<span data-ttu-id="fc244-111">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="fc244-111">**Element name**</span></span>|<span data-ttu-id="fc244-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc244-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc244-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="fc244-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="fc244-114">Contém o fluxo MIME (Multipurpose Internet Mail Extensions) nativo de um objeto representado no formato base64Binary.</span><span class="sxs-lookup"><span data-stu-id="fc244-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="fc244-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="fc244-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="fc244-116">Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc244-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fc244-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="fc244-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="fc244-118">Representa o identificador da pasta pai que contém o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="fc244-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="fc244-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="fc244-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="fc244-120">Representa a classe de mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="fc244-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="fc244-121">Assunto</span><span class="sxs-lookup"><span data-stu-id="fc244-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="fc244-122">Representa o assunto de itens do repositório do Exchange e objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="fc244-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="fc244-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="fc244-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="fc244-124">Indica o nível de sensibilidade de um item.</span><span class="sxs-lookup"><span data-stu-id="fc244-124">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="fc244-125">Body</span><span class="sxs-lookup"><span data-stu-id="fc244-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="fc244-126">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="fc244-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="fc244-127">Anexos</span><span class="sxs-lookup"><span data-stu-id="fc244-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="fc244-128">Contém os itens ou arquivos anexados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc244-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fc244-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="fc244-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="fc244-130">Representa a data e a hora em que um item foi recebido em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fc244-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="fc244-131">Tamanho</span><span class="sxs-lookup"><span data-stu-id="fc244-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="fc244-132">Representa o tamanho em bytes de um item.</span><span class="sxs-lookup"><span data-stu-id="fc244-132">Represents the size in bytes of an item.</span></span> <span data-ttu-id="fc244-133">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc244-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="fc244-134">Categorias</span><span class="sxs-lookup"><span data-stu-id="fc244-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="fc244-135">Representa uma coleção de cadeias de caracteres que identificam a quais categorias um item da caixa de correio pertence.</span><span class="sxs-lookup"><span data-stu-id="fc244-135">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="fc244-136">Importance</span><span class="sxs-lookup"><span data-stu-id="fc244-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="fc244-137">Descreve a importância de um item.</span><span class="sxs-lookup"><span data-stu-id="fc244-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="fc244-138">Inresponderto</span><span class="sxs-lookup"><span data-stu-id="fc244-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="fc244-139">Representa o identificador do item para o qual este item é uma resposta.</span><span class="sxs-lookup"><span data-stu-id="fc244-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="fc244-140">Isenviado</span><span class="sxs-lookup"><span data-stu-id="fc244-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="fc244-141">Indica se um item foi enviado para a pasta padrão da pasta de saída.</span><span class="sxs-lookup"><span data-stu-id="fc244-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="fc244-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="fc244-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="fc244-143">Indica se um item ainda não foi enviado.</span><span class="sxs-lookup"><span data-stu-id="fc244-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="fc244-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="fc244-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="fc244-145">Indica se um usuário enviou um item para si mesmo.</span><span class="sxs-lookup"><span data-stu-id="fc244-145">Indicates whether a user sent an item to himself or herself.</span></span>  <br/> |
|[<span data-ttu-id="fc244-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="fc244-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="fc244-147">Indica se o item foi enviado anteriormente.</span><span class="sxs-lookup"><span data-stu-id="fc244-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="fc244-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="fc244-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="fc244-149">Indica se o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="fc244-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="fc244-150">Propriedadeinternetmessageheaders</span><span class="sxs-lookup"><span data-stu-id="fc244-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="fc244-151">Representa a coleção de todos os cabeçalhos de mensagens da Internet contidos em um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fc244-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="fc244-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="fc244-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="fc244-153">Representa a data e a hora em que um item em uma caixa de correio foi enviado.</span><span class="sxs-lookup"><span data-stu-id="fc244-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="fc244-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="fc244-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="fc244-155">Representa a data e a hora em que um determinado item da caixa de correio foi criado.</span><span class="sxs-lookup"><span data-stu-id="fc244-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="fc244-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="fc244-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="fc244-157">Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc244-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fc244-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="fc244-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="fc244-159">Representa a data e a hora em que o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="fc244-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="fc244-160">Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="fc244-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="fc244-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="fc244-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="fc244-162">Indica se um lembrete foi definido para um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc244-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fc244-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="fc244-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="fc244-164">Representa o número de minutos antes de um evento quando um lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="fc244-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="fc244-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="fc244-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="fc244-166">Representa a cadeia de caracteres de exibição usada para o conteúdo da linha CC.</span><span class="sxs-lookup"><span data-stu-id="fc244-166">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="fc244-167">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários CC.</span><span class="sxs-lookup"><span data-stu-id="fc244-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="fc244-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="fc244-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="fc244-169">Representa a cadeia de caracteres de exibição usada para o conteúdo da linha para.</span><span class="sxs-lookup"><span data-stu-id="fc244-169">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="fc244-170">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários.</span><span class="sxs-lookup"><span data-stu-id="fc244-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="fc244-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="fc244-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="fc244-172">Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo visível.</span><span class="sxs-lookup"><span data-stu-id="fc244-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="fc244-173">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc244-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="fc244-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="fc244-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="fc244-175">Identifica as propriedades estendidas em pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="fc244-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="fc244-176">Cultura</span><span class="sxs-lookup"><span data-stu-id="fc244-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="fc244-177">Representa a cultura de um determinado item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fc244-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="fc244-178">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="fc244-178">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="fc244-179">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="fc244-179">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="fc244-180">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc244-180">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="fc244-181">LastModified</span><span class="sxs-lookup"><span data-stu-id="fc244-181">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="fc244-182">Contém o nome de exibição do último usuário a modificar um item.</span><span class="sxs-lookup"><span data-stu-id="fc244-182">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="fc244-183">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="fc244-183">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="fc244-184">Indica quando um item foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fc244-184">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="fc244-185">Isassociated</span><span class="sxs-lookup"><span data-stu-id="fc244-185">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="fc244-186">Indica se o item está associado a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="fc244-186">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="fc244-187">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="fc244-187">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="fc244-188">Representa uma URL para concatenar ao ponto de extremidade do Microsoft Office Outlook Web App para ler um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="fc244-188">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="fc244-189">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="fc244-189">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="fc244-190">Representa uma URL para concatenar ao ponto de extremidade do Outlook Web App para editar um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="fc244-190">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="fc244-191">ConversationId</span><span class="sxs-lookup"><span data-stu-id="fc244-191">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="fc244-192">Contém o identificador de um item ou uma conversa.</span><span class="sxs-lookup"><span data-stu-id="fc244-192">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="fc244-193">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="fc244-193">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="fc244-194">Representa um fragmento HTML ou texto sem formatação que representa o corpo exclusivo desta conversa.</span><span class="sxs-lookup"><span data-stu-id="fc244-194">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="fc244-195">FileAs</span><span class="sxs-lookup"><span data-stu-id="fc244-195">FileAs</span></span>](fileas.md) <br/> |<span data-ttu-id="fc244-196">Representa como um contato é arquivado na pasta contatos.</span><span class="sxs-lookup"><span data-stu-id="fc244-196">Represents how a contact is filed in the Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="fc244-197">FileAsMapping</span><span class="sxs-lookup"><span data-stu-id="fc244-197">FileAsMapping</span></span>](fileasmapping.md) <br/> |<span data-ttu-id="fc244-198">Define como construir o que é exibido para um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-198">Defines how to construct what is displayed for a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-199">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="fc244-199">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="fc244-200">Define o nome de exibição de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-200">Defines the display name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-201">GivenName</span><span class="sxs-lookup"><span data-stu-id="fc244-201">GivenName</span></span>](givenname.md) <br/> |<span data-ttu-id="fc244-202">Contém o nome fornecido de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-202">Contains a contact's given name.</span></span>  <br/> |
|[<span data-ttu-id="fc244-203">Iniciais</span><span class="sxs-lookup"><span data-stu-id="fc244-203">Initials</span></span>](initials.md) <br/> |<span data-ttu-id="fc244-204">Representa as iniciais de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-204">Represents the initials of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-205">MiddleName</span><span class="sxs-lookup"><span data-stu-id="fc244-205">MiddleName</span></span>](middlename.md) <br/> |<span data-ttu-id="fc244-206">Representa o nome do meio de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-206">Represents the middle name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-207">Apelido</span><span class="sxs-lookup"><span data-stu-id="fc244-207">Nickname</span></span>](nickname.md) <br/> |<span data-ttu-id="fc244-208">Representa o apelido de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-208">Represents the nickname of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-209">CompleteName</span><span class="sxs-lookup"><span data-stu-id="fc244-209">CompleteName</span></span>](completename.md) <br/> |<span data-ttu-id="fc244-210">Representa o nome completo de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-210">Represents the complete name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-211">CompanyName</span><span class="sxs-lookup"><span data-stu-id="fc244-211">CompanyName</span></span>](companyname.md) <br/> |<span data-ttu-id="fc244-212">Representa o nome da empresa que está associada a um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-212">Represents the company name that is associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-213">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="fc244-213">EmailAddresses</span></span>](emailaddresses.md) <br/> |<span data-ttu-id="fc244-214">Representa uma coleção de endereços de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-214">Represents a collection of e-mail addresses for a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-215">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="fc244-215">PhysicalAddresses</span></span>](physicaladdresses.md) <br/> |<span data-ttu-id="fc244-216">Contém uma coleção de endereços físicos associados a um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-216">Contains a collection of physical addresses that are associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-217">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="fc244-217">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="fc244-218">Representa uma coleção de números de telefone de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-218">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-219">AssistantName</span><span class="sxs-lookup"><span data-stu-id="fc244-219">AssistantName</span></span>](assistantname.md) <br/> |<span data-ttu-id="fc244-220">Representa um assistente para um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-220">Represents an assistant to a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-221">Aniversário</span><span class="sxs-lookup"><span data-stu-id="fc244-221">Birthday</span></span>](birthday.md) <br/> |<span data-ttu-id="fc244-222">Representa a data de nascimento de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-222">Represents the birth date of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-223">BusinessHomePage</span><span class="sxs-lookup"><span data-stu-id="fc244-223">BusinessHomePage</span></span>](businesshomepage.md) <br/> |<span data-ttu-id="fc244-224">Representa a Home Page (endereço da Web) do contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-224">Represents the Home page (Web address) for the contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-225">Filhos</span><span class="sxs-lookup"><span data-stu-id="fc244-225">Children</span></span>](children.md) <br/> |<span data-ttu-id="fc244-226">Contém os nomes dos filhos de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-226">Contains the names of a contact's children.</span></span>  <br/> |
|[<span data-ttu-id="fc244-227">Companies</span><span class="sxs-lookup"><span data-stu-id="fc244-227">Companies</span></span>](companies.md) <br/> |<span data-ttu-id="fc244-228">Representa a coleção de empresas que estão associadas a um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-228">Represents the collection of companies that are associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-229">Contato</span><span class="sxs-lookup"><span data-stu-id="fc244-229">ContactSource</span></span>](contactsource.md) <br/> |<span data-ttu-id="fc244-230">Descreve se o contato está localizado no repositório do Exchange ou no serviço de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fc244-230">Describes whether the contact is located in the Exchange store or the Active Directory directory service.</span></span>  <br/> |
|[<span data-ttu-id="fc244-231">Departamento</span><span class="sxs-lookup"><span data-stu-id="fc244-231">Department</span></span>](department.md) <br/> |<span data-ttu-id="fc244-232">Representa o departamento do contato no trabalho.</span><span class="sxs-lookup"><span data-stu-id="fc244-232">Represents the contact's department at work.</span></span>  <br/> |
|[<span data-ttu-id="fc244-233">Várias</span><span class="sxs-lookup"><span data-stu-id="fc244-233">Generation</span></span>](generation.md) <br/> |<span data-ttu-id="fc244-234">Representa uma abreviatura de geração que segue o nome completo de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-234">Represents a generational abbreviation that follows the full name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-235">Imendereços</span><span class="sxs-lookup"><span data-stu-id="fc244-235">ImAddresses</span></span>](imaddresses.md) <br/> |<span data-ttu-id="fc244-236">Representa uma coleção de endereços de mensagens instantâneas de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-236">Represents a collection of instant messaging addresses for a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-237">JobTitle</span><span class="sxs-lookup"><span data-stu-id="fc244-237">JobTitle</span></span>](jobtitle.md) <br/> |<span data-ttu-id="fc244-238">Representa o cargo de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-238">Represents the job title of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-239">Manager</span><span class="sxs-lookup"><span data-stu-id="fc244-239">Manager</span></span>](manager.md) <br/> |<span data-ttu-id="fc244-240">Representa o gerente de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-240">Represents a contact's manager.</span></span>  <br/> |
|[<span data-ttu-id="fc244-241">Mileage</span><span class="sxs-lookup"><span data-stu-id="fc244-241">Mileage</span></span>](mileage.md) <br/> |<span data-ttu-id="fc244-242">Representa a quilometragem de um item de contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-242">Represents mileage for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="fc244-243">OfficeLocation</span><span class="sxs-lookup"><span data-stu-id="fc244-243">OfficeLocation</span></span>](officelocation.md) <br/> |<span data-ttu-id="fc244-244">Representa o local do escritório de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-244">Represents the office location of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-245">PostalAddressIndex</span><span class="sxs-lookup"><span data-stu-id="fc244-245">PostalAddressIndex</span></span>](postaladdressindex.md) <br/> |<span data-ttu-id="fc244-246">Representa os tipos de exibição de endereços físicos.</span><span class="sxs-lookup"><span data-stu-id="fc244-246">Represents the display types for physical addresses.</span></span>  <br/> |
|[<span data-ttu-id="fc244-247">Profissão</span><span class="sxs-lookup"><span data-stu-id="fc244-247">Profession</span></span>](profession.md) <br/> |<span data-ttu-id="fc244-248">Representa a profissão de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-248">Represents the profession of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-249">Maridoname</span><span class="sxs-lookup"><span data-stu-id="fc244-249">SpouseName</span></span>](spousename.md) <br/> |<span data-ttu-id="fc244-250">Representa o nome do cônjuge/parceiro de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-250">Represents the name of a contact's spouse/partner.</span></span>  <br/> |
|[<span data-ttu-id="fc244-251">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="fc244-251">Surname</span></span>](surname.md) <br/> |<span data-ttu-id="fc244-252">Representa o sobrenome de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-252">Represents the surname of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-253">WeddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="fc244-253">WeddingAnniversary</span></span>](weddinganniversary.md) <br/> |<span data-ttu-id="fc244-254">Contém o aniversário de casamento de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-254">Contains the wedding anniversary of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-255">HasPicture</span><span class="sxs-lookup"><span data-stu-id="fc244-255">HasPicture</span></span>](haspicture.md) <br/> |<span data-ttu-id="fc244-256">Indica se o item de contato tem um anexo de arquivo que representa a imagem do contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-256">Indicates whether the contact item has a file attachment that represents the contact's picture.</span></span>  <br/> |
|[<span data-ttu-id="fc244-257">PhoneticFullName</span><span class="sxs-lookup"><span data-stu-id="fc244-257">PhoneticFullName</span></span>](phoneticfullname.md) <br/> |<span data-ttu-id="fc244-258">Contém o nome completo de um contato, incluindo o nome e o sobrenome, grafo foneticamente.</span><span class="sxs-lookup"><span data-stu-id="fc244-258">Contains the full name of a contact, including the first and last name, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="fc244-259">PhoneticFirstName</span><span class="sxs-lookup"><span data-stu-id="fc244-259">PhoneticFirstName</span></span>](phoneticfirstname.md) <br/> |<span data-ttu-id="fc244-260">Contém o primeiro nome de um contato, escrito foneticamente.</span><span class="sxs-lookup"><span data-stu-id="fc244-260">Contains the first name of a contact, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="fc244-261">PhoneticLastName</span><span class="sxs-lookup"><span data-stu-id="fc244-261">PhoneticLastName</span></span>](phoneticlastname.md) <br/> |<span data-ttu-id="fc244-262">Contém o sobrenome de um contato, escrito foneticamente.</span><span class="sxs-lookup"><span data-stu-id="fc244-262">Contains the last name of a contact, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="fc244-263">Alias</span><span class="sxs-lookup"><span data-stu-id="fc244-263">Alias</span></span>](alias.md) <br/> |<span data-ttu-id="fc244-264">Contém o alias de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-264">Contains the email alias of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-265">Observações (contato)</span><span class="sxs-lookup"><span data-stu-id="fc244-265">Notes (Contact)</span></span>](notes-contact.md) <br/> |<span data-ttu-id="fc244-266">Contém informações de contato suplementares.</span><span class="sxs-lookup"><span data-stu-id="fc244-266">Contains supplementary contact information.</span></span>  <br/> |
|[<span data-ttu-id="fc244-267">Foto</span><span class="sxs-lookup"><span data-stu-id="fc244-267">Photo</span></span>](photo.md) <br/> |<span data-ttu-id="fc244-268">Contém um valor que codifica a foto de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-268">Contains a value that encodes the photo of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-269">UserSMIMECertificate</span><span class="sxs-lookup"><span data-stu-id="fc244-269">UserSMIMECertificate</span></span>](usersmimecertificate.md) <br/> |<span data-ttu-id="fc244-270">Contém um valor que codifica o certificado SMIME de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-270">Contains a value that encodes the SMIME certificate of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-271">MSExchangeCertificate</span><span class="sxs-lookup"><span data-stu-id="fc244-271">MSExchangeCertificate</span></span>](msexchangecertificate.md) <br/> |<span data-ttu-id="fc244-272">Contém um valor que codifica o certificado do Microsoft Exchange de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-272">Contains a value that encodes the Microsoft Exchange certificate of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-273">Directoryid</span><span class="sxs-lookup"><span data-stu-id="fc244-273">DirectoryId</span></span>](directoryid.md) <br/> |<span data-ttu-id="fc244-274">Contém a ID de diretório de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-274">Contains the directory ID of a contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-275">ManagerMailbox</span><span class="sxs-lookup"><span data-stu-id="fc244-275">ManagerMailbox</span></span>](managermailbox.md) <br/> |<span data-ttu-id="fc244-276">Contém informações SMTP que identificam a caixa de correio do gerente do contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-276">Contains SMTP information that identifies the manager mailbox of the contact.</span></span>  <br/> |
|[<span data-ttu-id="fc244-277">DirectReports</span><span class="sxs-lookup"><span data-stu-id="fc244-277">DirectReports</span></span>](directreports.md) <br/> |<span data-ttu-id="fc244-278">Contém informações SMTP que identificam os subordinados diretos de um contato.</span><span class="sxs-lookup"><span data-stu-id="fc244-278">Contains SMTP information that identifies the direct reports of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fc244-279">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fc244-279">Parent elements</span></span>

|<span data-ttu-id="fc244-280">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="fc244-280">**Element name**</span></span>|<span data-ttu-id="fc244-281">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc244-281">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc244-282">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="fc244-282">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="fc244-283">Descreve todos os itens de calendário adjacentes a um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="fc244-283">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="fc244-284">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="fc244-284">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="fc244-285">Identifica os dados a serem acrescentados a uma única propriedade de um item ou pasta durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="fc244-285">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="fc244-286">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="fc244-286">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="fc244-287">Identifica todos os itens que entram em conflito com um horário de reunião</span><span class="sxs-lookup"><span data-stu-id="fc244-287">Identifies all items that conflict with a meeting time</span></span>  <br/> |
|[<span data-ttu-id="fc244-288">Create (issync)</span><span class="sxs-lookup"><span data-stu-id="fc244-288">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="fc244-289">Identifica uma única pasta a ser criada no armazenamento do cliente local.</span><span class="sxs-lookup"><span data-stu-id="fc244-289">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="fc244-290">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="fc244-290">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="fc244-291">Representa um item do Exchange anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc244-291">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="fc244-292">Itens</span><span class="sxs-lookup"><span data-stu-id="fc244-292">Items</span></span>](items.md) <br/> |<span data-ttu-id="fc244-293">Contém uma matriz de itens.</span><span class="sxs-lookup"><span data-stu-id="fc244-293">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="fc244-294">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="fc244-294">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="fc244-295">Contém uma matriz de itens a serem criados na pasta que é identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="fc244-295">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="fc244-296">Resolução</span><span class="sxs-lookup"><span data-stu-id="fc244-296">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="fc244-297">Contém uma única entidade resolvida.</span><span class="sxs-lookup"><span data-stu-id="fc244-297">Contains a single resolved entity.</span></span>  <br/> |
|[<span data-ttu-id="fc244-298">Setitemfield</span><span class="sxs-lookup"><span data-stu-id="fc244-298">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="fc244-299">Representa uma atualização de uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="fc244-299">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="fc244-300">Atualização (issync)</span><span class="sxs-lookup"><span data-stu-id="fc244-300">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="fc244-301">Identifica um único item a ser atualizado no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="fc244-301">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fc244-302">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="fc244-302">Text value</span></span>

<span data-ttu-id="fc244-303">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fc244-303">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fc244-304">Comentários</span><span class="sxs-lookup"><span data-stu-id="fc244-304">Remarks</span></span>

<span data-ttu-id="fc244-305">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc244-305">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc244-306">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fc244-306">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc244-307">Namespace</span><span class="sxs-lookup"><span data-stu-id="fc244-307">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fc244-308">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fc244-308">Schema name</span></span>  <br/> |<span data-ttu-id="fc244-309">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="fc244-309">Types schema</span></span>  <br/> |
|<span data-ttu-id="fc244-310">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fc244-310">Validation file</span></span>  <br/> |<span data-ttu-id="fc244-311">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fc244-311">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fc244-312">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="fc244-312">Can be empty</span></span>  <br/> |<span data-ttu-id="fc244-313">False</span><span class="sxs-lookup"><span data-stu-id="fc244-313">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc244-314">Confira também</span><span class="sxs-lookup"><span data-stu-id="fc244-314">See also</span></span>



- [<span data-ttu-id="fc244-315">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fc244-315">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="fc244-316">Criando contatos (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="fc244-316">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="fc244-317">Atualizando contatos</span><span class="sxs-lookup"><span data-stu-id="fc244-317">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="fc244-318">Excluindo contatos</span><span class="sxs-lookup"><span data-stu-id="fc244-318">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

