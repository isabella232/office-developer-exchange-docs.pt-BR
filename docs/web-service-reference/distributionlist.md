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
ms.openlocfilehash: 5edcc83eef6a5b16470e6c290aacd057ceecceb1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751903"
---
# <a name="distributionlist"></a><span data-ttu-id="e8178-103">DistributionList</span><span class="sxs-lookup"><span data-stu-id="e8178-103">DistributionList</span></span>

<span data-ttu-id="e8178-104">O elemento **DistributionList** representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e8178-104">The **DistributionList** element represents a distribution list.</span></span> 
  
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

 <span data-ttu-id="e8178-105">**DistributionListType**</span><span class="sxs-lookup"><span data-stu-id="e8178-105">**DistributionListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8178-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e8178-106">Attributes and elements</span></span>

<span data-ttu-id="e8178-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e8178-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8178-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e8178-108">Attributes</span></span>

<span data-ttu-id="e8178-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e8178-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8178-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e8178-110">Child elements</span></span>

|<span data-ttu-id="e8178-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e8178-111">**Element**</span></span>|<span data-ttu-id="e8178-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e8178-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8178-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="e8178-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="e8178-114">Contém o fluxo MIME nativo de um objeto representado no formato base64Binary.</span><span class="sxs-lookup"><span data-stu-id="e8178-114">Contains the native MIME stream of an object represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="e8178-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="e8178-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="e8178-116">Contém o identificador e alterar a chave exclusiva de um item de lista de distribuição no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8178-116">Contains the unique identifier and change key of a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e8178-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="e8178-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="e8178-118">Representa o identificador da pasta pai que contém o item de lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e8178-118">Represents the identifier of the parent folder that contains the distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="e8178-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="e8178-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="e8178-120">Representa a classe de mensagem de um item de lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e8178-120">Represents the message class of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="e8178-121">Assunto</span><span class="sxs-lookup"><span data-stu-id="e8178-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="e8178-122">Representa o assunto para armazenar itens do Exchange e objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8178-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="e8178-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="e8178-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="e8178-124">Contém o status de sensibilidade de um item lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e8178-124">Contains the status for a distribution list item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="e8178-125">Corpo</span><span class="sxs-lookup"><span data-stu-id="e8178-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="e8178-126">Representa o conteúdo real do corpo de um item de lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e8178-126">Represents the actual body content of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="e8178-127">Anexos</span><span class="sxs-lookup"><span data-stu-id="e8178-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e8178-128">Contém os itens ou arquivos que estejam anexados a um item de lista de distribuição no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8178-128">Contains the items or files that are attached to a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e8178-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="e8178-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="e8178-130">Representa a data e hora em que um item de lista de distribuição em uma caixa de correio foi recebido.</span><span class="sxs-lookup"><span data-stu-id="e8178-130">Represents the date and time that a distribution list item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="e8178-131">Size</span><span class="sxs-lookup"><span data-stu-id="e8178-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="e8178-132">Representa o tamanho, em bytes, de um item de lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e8178-132">Represents the size, in bytes, of a distribution list item.</span></span> <span data-ttu-id="e8178-133">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e8178-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="e8178-134">Categorias</span><span class="sxs-lookup"><span data-stu-id="e8178-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e8178-135">Representa uma coleção de cadeias de caracteres que identificam a quais categorias de um item de lista de distribuição na caixa de correio pertence.</span><span class="sxs-lookup"><span data-stu-id="e8178-135">Represents a collection of strings that identify to which categories a distribution list item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="e8178-136">Importância</span><span class="sxs-lookup"><span data-stu-id="e8178-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="e8178-137">Descreve a importância de um item de lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e8178-137">Describes the importance of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="e8178-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="e8178-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="e8178-139">Representa o identificador do item que este item é uma resposta.</span><span class="sxs-lookup"><span data-stu-id="e8178-139">Represents the identifier of the item which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="e8178-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="e8178-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="e8178-141">Indica se um item foi enviado à pasta padrão caixa de saída.</span><span class="sxs-lookup"><span data-stu-id="e8178-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="e8178-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="e8178-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="e8178-143">Indica se um item ainda não foi enviado.</span><span class="sxs-lookup"><span data-stu-id="e8178-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="e8178-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="e8178-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="e8178-145">Indica se um usuário enviada a um item para si mesma.</span><span class="sxs-lookup"><span data-stu-id="e8178-145">Indicates whether a user sent an item to itself.</span></span>  <br/> |
|[<span data-ttu-id="e8178-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="e8178-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="e8178-147">Indica se o item anteriormente foi enviado.</span><span class="sxs-lookup"><span data-stu-id="e8178-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="e8178-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="e8178-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="e8178-149">Indica se o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="e8178-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="e8178-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="e8178-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="e8178-151">Representa a coleção de todos os cabeçalhos de mensagem de Internet contida em um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e8178-151">Represents the collection of all Internet message headers contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e8178-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="e8178-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="e8178-153">Representa a data e hora em que um item em uma caixa de correio foi enviado.</span><span class="sxs-lookup"><span data-stu-id="e8178-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="e8178-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="e8178-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="e8178-155">Representa a data e hora em que um determinado item na caixa de correio foi criado.</span><span class="sxs-lookup"><span data-stu-id="e8178-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="e8178-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="e8178-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="e8178-157">Contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8178-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e8178-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="e8178-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="e8178-159">Representa a data e hora quando o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="e8178-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="e8178-160">Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="e8178-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="e8178-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="e8178-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="e8178-162">Indica se um lembrete tiver sido definido para um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8178-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e8178-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="e8178-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="e8178-164">Representa o número de minutos antes de um evento, quando um lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="e8178-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="e8178-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="e8178-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="e8178-166">Representa a cadeia de caracteres de exibição que é usada para o conteúdo da linha Cc.</span><span class="sxs-lookup"><span data-stu-id="e8178-166">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="e8178-167">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição destinatários Cc.</span><span class="sxs-lookup"><span data-stu-id="e8178-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="e8178-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="e8178-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="e8178-169">Representa a cadeia de caracteres de exibição que é usada para o conteúdo da linha para.</span><span class="sxs-lookup"><span data-stu-id="e8178-169">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="e8178-170">Esta é a cadeia de caracteres concatenada de todos os aos nomes de exibição do destinatário.</span><span class="sxs-lookup"><span data-stu-id="e8178-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="e8178-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="e8178-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="e8178-172">Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo visível.</span><span class="sxs-lookup"><span data-stu-id="e8178-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="e8178-173">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e8178-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="e8178-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="e8178-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="e8178-175">Identifica as propriedades estendidas em um item de lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e8178-175">Identifies extended properties on a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="e8178-176">Cultura</span><span class="sxs-lookup"><span data-stu-id="e8178-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="e8178-177">Representa a cultura para um item de lista de distribuição em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e8178-177">Represents the culture for a distribution list item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e8178-178">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="e8178-178">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="e8178-179">Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="e8178-179">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="e8178-180">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e8178-180">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="e8178-181">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="e8178-181">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="e8178-182">Contém o nome de exibição do último usuário para modificar um item.</span><span class="sxs-lookup"><span data-stu-id="e8178-182">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="e8178-183">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="e8178-183">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="e8178-184">Indica quando um item da última modificação.</span><span class="sxs-lookup"><span data-stu-id="e8178-184">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="e8178-185">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="e8178-185">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="e8178-186">Indica se o item está associado a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="e8178-186">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="e8178-187">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="e8178-187">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="e8178-188">Representa uma URL para concatenar no ponto de extremidade do Microsoft Office Outlook Web App para ler um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="e8178-188">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="e8178-189">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="e8178-189">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="e8178-190">Representa uma URL para concatenar no ponto de extremidade do Outlook Web App para editar um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="e8178-190">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="e8178-191">ConversationId</span><span class="sxs-lookup"><span data-stu-id="e8178-191">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="e8178-192">Contém o identificador de um item ou conversa.</span><span class="sxs-lookup"><span data-stu-id="e8178-192">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="e8178-193">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="e8178-193">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="e8178-194">Representa um fragmento HTML ou texto sem formatação que representa um único corpo da conversa.</span><span class="sxs-lookup"><span data-stu-id="e8178-194">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="e8178-195">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="e8178-195">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="e8178-196">Define o nome de exibição de uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e8178-196">Defines the display name of a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="e8178-197">FileAs</span><span class="sxs-lookup"><span data-stu-id="e8178-197">FileAs</span></span>](fileas.md) <br/> |<span data-ttu-id="e8178-198">Representa como uma lista de distribuição é arquivada na pasta Contatos.</span><span class="sxs-lookup"><span data-stu-id="e8178-198">Represents how a distribution list is filed in the Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="e8178-199">ContactSource</span><span class="sxs-lookup"><span data-stu-id="e8178-199">ContactSource</span></span>](contactsource.md) <br/> |<span data-ttu-id="e8178-200">Descreve como se o contato está localizado no armazenamento do Exchange ou nos serviços de domínio Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="e8178-200">Describes whether the contact is located in the Exchange store or in Active Directory Domain Services (AD DS).</span></span>  <br/> |
|[<span data-ttu-id="e8178-201">Membros (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="e8178-201">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="e8178-202">Contém uma lista de membros da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e8178-202">Contains a list of members of the distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e8178-203">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e8178-203">Parent elements</span></span>

|<span data-ttu-id="e8178-204">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e8178-204">**Element**</span></span>|<span data-ttu-id="e8178-205">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e8178-205">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8178-206">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="e8178-206">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="e8178-207">Descreve todos os itens de calendário que são adjacentes para um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="e8178-207">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="e8178-208">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="e8178-208">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="e8178-209">Identifica os dados a serem acrescentados a uma única propriedade de uma lista de distribuição durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e8178-209">Identifies data to append to a single property of a distribution list during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="e8178-210">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="e8178-210">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="e8178-211">Identifica todos os itens que estão em conflito com um tempo de reunião.</span><span class="sxs-lookup"><span data-stu-id="e8178-211">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="e8178-212">Criar (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="e8178-212">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="e8178-213">Identifica uma lista de distribuição para criar no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="e8178-213">Identifies a single distribution list to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="e8178-214">Atualização (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="e8178-214">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="e8178-215">Identifica uma lista de distribuição a ser atualizado no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="e8178-215">Identifies a single distribution list to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="e8178-216">Items</span><span class="sxs-lookup"><span data-stu-id="e8178-216">Items</span></span>](items.md) <br/> |<span data-ttu-id="e8178-217">Contém uma matriz de itens.</span><span class="sxs-lookup"><span data-stu-id="e8178-217">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="e8178-218">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="e8178-218">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="e8178-219">Contém uma matriz de itens para criar a pasta identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="e8178-219">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="e8178-220">SetItemField</span><span class="sxs-lookup"><span data-stu-id="e8178-220">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="e8178-221">Representa uma atualização para uma única propriedade de um item de lista de distribuição em uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e8178-221">Represents an update to a single property of a distribution list item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e8178-222">Text value</span><span class="sxs-lookup"><span data-stu-id="e8178-222">Text value</span></span>

<span data-ttu-id="e8178-223">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e8178-223">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e8178-224">Comentários</span><span class="sxs-lookup"><span data-stu-id="e8178-224">Remarks</span></span>

<span data-ttu-id="e8178-225">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8178-225">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8178-226">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e8178-226">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8178-227">Namespace</span><span class="sxs-lookup"><span data-stu-id="e8178-227">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e8178-228">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e8178-228">Schema Name</span></span>  <br/> |<span data-ttu-id="e8178-229">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e8178-229">Types schema</span></span>  <br/> |
|<span data-ttu-id="e8178-230">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e8178-230">Validation File</span></span>  <br/> |<span data-ttu-id="e8178-231">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e8178-231">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e8178-232">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e8178-232">Can be Empty</span></span>  <br/> |<span data-ttu-id="e8178-233">False</span><span class="sxs-lookup"><span data-stu-id="e8178-233">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8178-234">Ver também</span><span class="sxs-lookup"><span data-stu-id="e8178-234">See also</span></span>

- [<span data-ttu-id="e8178-235">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e8178-235">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

