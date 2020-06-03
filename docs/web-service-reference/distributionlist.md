---
title: DistributionList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistributionList
api_type:
- schema
ms.assetid: f65aea01-e870-44a2-8571-fa6c001341cc
description: O elemento DistributionList representa uma lista de distribuição.
ms.openlocfilehash: 5eb97bef349ca02848f65fa58370b9c81c6653d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457001"
---
# <a name="distributionlist"></a><span data-ttu-id="9d415-103">DistributionList</span><span class="sxs-lookup"><span data-stu-id="9d415-103">DistributionList</span></span>

<span data-ttu-id="9d415-104">O elemento **DistributionList** representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9d415-104">The **DistributionList** element represents a distribution list.</span></span> 
  
```xml
<DistributionList>
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
   <DisplayName/>
   <FileAs/>
   <ContactSource/>
   <Members/>
</DistributionList>
```

 <span data-ttu-id="9d415-105">**DistributionListType**</span><span class="sxs-lookup"><span data-stu-id="9d415-105">**DistributionListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d415-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9d415-106">Attributes and elements</span></span>

<span data-ttu-id="9d415-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9d415-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d415-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9d415-108">Attributes</span></span>

<span data-ttu-id="9d415-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d415-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d415-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9d415-110">Child elements</span></span>

|<span data-ttu-id="9d415-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9d415-111">**Element**</span></span>|<span data-ttu-id="9d415-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d415-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d415-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="9d415-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="9d415-114">Contém o fluxo MIME nativo de um objeto representado no formato base64Binary.</span><span class="sxs-lookup"><span data-stu-id="9d415-114">Contains the native MIME stream of an object represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="9d415-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="9d415-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="9d415-116">Contém o identificador exclusivo e a chave de alteração de um item de lista de distribuição no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d415-116">Contains the unique identifier and change key of a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9d415-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="9d415-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="9d415-118">Representa o identificador da pasta pai que contém o item de lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9d415-118">Represents the identifier of the parent folder that contains the distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="9d415-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="9d415-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="9d415-120">Representa a classe de mensagem de um item de lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9d415-120">Represents the message class of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="9d415-121">Assunto</span><span class="sxs-lookup"><span data-stu-id="9d415-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="9d415-122">Representa o assunto de itens do repositório do Exchange e objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="9d415-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="9d415-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="9d415-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="9d415-124">Contém o status da confidencialidade de um item de lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9d415-124">Contains the status for a distribution list item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="9d415-125">Body</span><span class="sxs-lookup"><span data-stu-id="9d415-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="9d415-126">Representa o conteúdo real do corpo de um item de lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9d415-126">Represents the actual body content of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="9d415-127">Anexos</span><span class="sxs-lookup"><span data-stu-id="9d415-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9d415-128">Contém os itens ou arquivos anexados a um item de lista de distribuição no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d415-128">Contains the items or files that are attached to a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9d415-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="9d415-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="9d415-130">Representa a data e a hora em que um item de lista de distribuição foi recebido em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9d415-130">Represents the date and time that a distribution list item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="9d415-131">Tamanho</span><span class="sxs-lookup"><span data-stu-id="9d415-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="9d415-132">Representa o tamanho, em bytes, de um item de lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9d415-132">Represents the size, in bytes, of a distribution list item.</span></span> <span data-ttu-id="9d415-133">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9d415-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="9d415-134">Categorias</span><span class="sxs-lookup"><span data-stu-id="9d415-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9d415-135">Representa uma coleção de cadeias de caracteres que identificam a quais categorias um item de lista de distribuição pertence à caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9d415-135">Represents a collection of strings that identify to which categories a distribution list item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="9d415-136">Importance</span><span class="sxs-lookup"><span data-stu-id="9d415-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="9d415-137">Descreve a importância de um item de lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9d415-137">Describes the importance of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="9d415-138">Inresponderto</span><span class="sxs-lookup"><span data-stu-id="9d415-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="9d415-139">Representa o identificador do item em que este item é uma resposta.</span><span class="sxs-lookup"><span data-stu-id="9d415-139">Represents the identifier of the item which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="9d415-140">Isenviado</span><span class="sxs-lookup"><span data-stu-id="9d415-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="9d415-141">Indica se um item foi enviado para a pasta padrão da pasta de saída.</span><span class="sxs-lookup"><span data-stu-id="9d415-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="9d415-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="9d415-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="9d415-143">Indica se um item ainda não foi enviado.</span><span class="sxs-lookup"><span data-stu-id="9d415-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="9d415-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="9d415-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="9d415-145">Indica se um usuário enviou um item para si mesmo.</span><span class="sxs-lookup"><span data-stu-id="9d415-145">Indicates whether a user sent an item to itself.</span></span>  <br/> |
|[<span data-ttu-id="9d415-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="9d415-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="9d415-147">Indica se o item foi enviado anteriormente.</span><span class="sxs-lookup"><span data-stu-id="9d415-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="9d415-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="9d415-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="9d415-149">Indica se o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="9d415-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="9d415-150">Propriedadeinternetmessageheaders</span><span class="sxs-lookup"><span data-stu-id="9d415-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="9d415-151">Representa a coleção de todos os cabeçalhos de mensagens da Internet contidos em um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9d415-151">Represents the collection of all Internet message headers contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9d415-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="9d415-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="9d415-153">Representa a data e a hora em que um item em uma caixa de correio foi enviado.</span><span class="sxs-lookup"><span data-stu-id="9d415-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="9d415-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="9d415-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="9d415-155">Representa a data e a hora em que um determinado item da caixa de correio foi criado.</span><span class="sxs-lookup"><span data-stu-id="9d415-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="9d415-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="9d415-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="9d415-157">Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d415-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9d415-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="9d415-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="9d415-159">Representa a data e a hora em que o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="9d415-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="9d415-160">Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="9d415-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="9d415-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="9d415-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="9d415-162">Indica se um lembrete foi definido para um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d415-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9d415-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="9d415-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="9d415-164">Representa o número de minutos antes de um evento quando um lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="9d415-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="9d415-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="9d415-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="9d415-166">Representa a cadeia de caracteres de exibição usada para o conteúdo da linha CC.</span><span class="sxs-lookup"><span data-stu-id="9d415-166">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="9d415-167">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários CC.</span><span class="sxs-lookup"><span data-stu-id="9d415-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="9d415-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="9d415-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="9d415-169">Representa a cadeia de caracteres de exibição usada para o conteúdo da linha para.</span><span class="sxs-lookup"><span data-stu-id="9d415-169">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="9d415-170">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários.</span><span class="sxs-lookup"><span data-stu-id="9d415-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="9d415-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="9d415-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="9d415-172">Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo visível.</span><span class="sxs-lookup"><span data-stu-id="9d415-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="9d415-173">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9d415-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="9d415-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="9d415-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="9d415-175">Identifica as propriedades estendidas em um item de lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9d415-175">Identifies extended properties on a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="9d415-176">Cultura</span><span class="sxs-lookup"><span data-stu-id="9d415-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="9d415-177">Representa a cultura de um item de lista de distribuição em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9d415-177">Represents the culture for a distribution list item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9d415-178">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="9d415-178">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="9d415-179">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="9d415-179">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="9d415-180">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9d415-180">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="9d415-181">LastModified</span><span class="sxs-lookup"><span data-stu-id="9d415-181">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="9d415-182">Contém o nome de exibição do último usuário a modificar um item.</span><span class="sxs-lookup"><span data-stu-id="9d415-182">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="9d415-183">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="9d415-183">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="9d415-184">Indica quando um item foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9d415-184">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="9d415-185">Isassociated</span><span class="sxs-lookup"><span data-stu-id="9d415-185">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="9d415-186">Indica se o item está associado a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="9d415-186">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="9d415-187">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="9d415-187">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="9d415-188">Representa uma URL para concatenar ao ponto de extremidade do Microsoft Office Outlook Web App para ler um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="9d415-188">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="9d415-189">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="9d415-189">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="9d415-190">Representa uma URL para concatenar ao ponto de extremidade do Outlook Web App para editar um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="9d415-190">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="9d415-191">ConversationId</span><span class="sxs-lookup"><span data-stu-id="9d415-191">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="9d415-192">Contém o identificador de um item ou uma conversa.</span><span class="sxs-lookup"><span data-stu-id="9d415-192">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="9d415-193">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="9d415-193">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="9d415-194">Representa um fragmento HTML ou texto sem formatação que representa o corpo exclusivo desta conversa.</span><span class="sxs-lookup"><span data-stu-id="9d415-194">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="9d415-195">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="9d415-195">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="9d415-196">Define o nome de exibição de uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9d415-196">Defines the display name of a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="9d415-197">FileAs</span><span class="sxs-lookup"><span data-stu-id="9d415-197">FileAs</span></span>](fileas.md) <br/> |<span data-ttu-id="9d415-198">Representa como uma lista de distribuição é arquivada na pasta contatos.</span><span class="sxs-lookup"><span data-stu-id="9d415-198">Represents how a distribution list is filed in the Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="9d415-199">Contato</span><span class="sxs-lookup"><span data-stu-id="9d415-199">ContactSource</span></span>](contactsource.md) <br/> |<span data-ttu-id="9d415-200">Descreve se o contato está localizado no repositório do Exchange ou nos serviços de domínio do Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="9d415-200">Describes whether the contact is located in the Exchange store or in Active Directory Domain Services (AD DS).</span></span>  <br/> |
|[<span data-ttu-id="9d415-201">Membros (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="9d415-201">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="9d415-202">Contém uma lista de membros da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="9d415-202">Contains a list of members of the distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d415-203">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9d415-203">Parent elements</span></span>

|<span data-ttu-id="9d415-204">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9d415-204">**Element**</span></span>|<span data-ttu-id="9d415-205">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d415-205">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d415-206">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="9d415-206">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="9d415-207">Descreve todos os itens de calendário adjacentes a um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="9d415-207">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="9d415-208">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="9d415-208">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="9d415-209">Identifica os dados a serem acrescentados a uma única propriedade de uma lista de distribuição durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9d415-209">Identifies data to append to a single property of a distribution list during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="9d415-210">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="9d415-210">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="9d415-211">Identifica todos os itens que entram em conflito com um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="9d415-211">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="9d415-212">Create (issync)</span><span class="sxs-lookup"><span data-stu-id="9d415-212">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="9d415-213">Identifica uma única lista de distribuição a ser criada no armazenamento do cliente local.</span><span class="sxs-lookup"><span data-stu-id="9d415-213">Identifies a single distribution list to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="9d415-214">Atualização (issync)</span><span class="sxs-lookup"><span data-stu-id="9d415-214">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="9d415-215">Identifica uma única lista de distribuição a ser atualizada no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="9d415-215">Identifies a single distribution list to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="9d415-216">Itens</span><span class="sxs-lookup"><span data-stu-id="9d415-216">Items</span></span>](items.md) <br/> |<span data-ttu-id="9d415-217">Contém uma matriz de itens.</span><span class="sxs-lookup"><span data-stu-id="9d415-217">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="9d415-218">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="9d415-218">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="9d415-219">Contém uma matriz de itens a serem criados na pasta identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="9d415-219">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="9d415-220">Setitemfield</span><span class="sxs-lookup"><span data-stu-id="9d415-220">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="9d415-221">Representa uma atualização de uma única propriedade de um item de lista de distribuição em uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9d415-221">Represents an update to a single property of a distribution list item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9d415-222">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="9d415-222">Text value</span></span>

<span data-ttu-id="9d415-223">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9d415-223">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9d415-224">Comentários</span><span class="sxs-lookup"><span data-stu-id="9d415-224">Remarks</span></span>

<span data-ttu-id="9d415-225">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d415-225">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d415-226">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9d415-226">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d415-227">Namespace</span><span class="sxs-lookup"><span data-stu-id="9d415-227">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9d415-228">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9d415-228">Schema Name</span></span>  <br/> |<span data-ttu-id="9d415-229">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9d415-229">Types schema</span></span>  <br/> |
|<span data-ttu-id="9d415-230">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9d415-230">Validation File</span></span>  <br/> |<span data-ttu-id="9d415-231">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9d415-231">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9d415-232">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9d415-232">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d415-233">False</span><span class="sxs-lookup"><span data-stu-id="9d415-233">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d415-234">Confira também</span><span class="sxs-lookup"><span data-stu-id="9d415-234">See also</span></span>

- [<span data-ttu-id="9d415-235">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9d415-235">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

