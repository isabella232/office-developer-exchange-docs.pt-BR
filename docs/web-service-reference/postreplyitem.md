---
title: PostReplyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostReplyItem
api_type:
- schema
ms.assetid: e5d93d63-0a3b-470f-9a94-2d57284c6745
description: O elemento PostReplyItem contém uma resposta a um item de postagem. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 4104e79449acc6e358b729cf2de769d28dac52bd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461678"
---
# <a name="postreplyitem"></a><span data-ttu-id="717d7-104">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="717d7-104">PostReplyItem</span></span>

<span data-ttu-id="717d7-105">O elemento **PostReplyItem** contém uma resposta a um item de postagem.</span><span class="sxs-lookup"><span data-stu-id="717d7-105">The **PostReplyItem** element contains a reply to a post item.</span></span> <span data-ttu-id="717d7-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="717d7-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PostReplyItem>
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
   <EffectiveRights/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
   <NewBodyContent/>
</PostReplyItem>
```

 <span data-ttu-id="717d7-107">**PostReplyItemType**</span><span class="sxs-lookup"><span data-stu-id="717d7-107">**PostReplyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="717d7-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="717d7-108">Attributes and elements</span></span>

<span data-ttu-id="717d7-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="717d7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="717d7-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="717d7-110">Attributes</span></span>

<span data-ttu-id="717d7-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="717d7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="717d7-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="717d7-112">Child elements</span></span>

|<span data-ttu-id="717d7-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="717d7-113">**Element**</span></span>|<span data-ttu-id="717d7-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="717d7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="717d7-115">MimeContent</span><span class="sxs-lookup"><span data-stu-id="717d7-115">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="717d7-116">Contém o fluxo MIME (Multipurpose Internet Mail Extensions) nativo de um objeto representado no formato base64Binary.</span><span class="sxs-lookup"><span data-stu-id="717d7-116">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="717d7-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="717d7-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="717d7-118">Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="717d7-118">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="717d7-119">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="717d7-119">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="717d7-120">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="717d7-120">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="717d7-121">Representa o identificador da pasta pai que contém o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="717d7-121">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="717d7-122">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="717d7-122">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="717d7-123">ItemClass</span><span class="sxs-lookup"><span data-stu-id="717d7-123">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="717d7-124">Representa a classe de mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="717d7-124">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="717d7-125">Assunto</span><span class="sxs-lookup"><span data-stu-id="717d7-125">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="717d7-126">Representa o assunto de itens do repositório do Exchange e objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="717d7-126">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="717d7-127">O assunto está limitado a 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="717d7-127">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="717d7-128">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="717d7-128">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="717d7-129">Indica o nível de sensibilidade de um item.</span><span class="sxs-lookup"><span data-stu-id="717d7-129">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="717d7-130">Body</span><span class="sxs-lookup"><span data-stu-id="717d7-130">Body</span></span>](body.md) <br/> |<span data-ttu-id="717d7-131">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="717d7-131">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="717d7-132">Anexos</span><span class="sxs-lookup"><span data-stu-id="717d7-132">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="717d7-133">Contém os itens ou arquivos anexados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="717d7-133">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="717d7-134">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="717d7-134">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="717d7-135">Representa a data e a hora em que um item foi recebido em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="717d7-135">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="717d7-136">Tamanho</span><span class="sxs-lookup"><span data-stu-id="717d7-136">Size</span></span>](size.md) <br/> |<span data-ttu-id="717d7-137">Representa o tamanho em bytes de um item.</span><span class="sxs-lookup"><span data-stu-id="717d7-137">Represents the size in bytes of an item.</span></span> <span data-ttu-id="717d7-138">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="717d7-138">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="717d7-139">Categorias</span><span class="sxs-lookup"><span data-stu-id="717d7-139">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="717d7-140">Representa uma coleção de cadeias de caracteres que identificam as categorias às quais um item da caixa de correio pertence.</span><span class="sxs-lookup"><span data-stu-id="717d7-140">Represents a collection of strings that identify categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="717d7-141">Importance</span><span class="sxs-lookup"><span data-stu-id="717d7-141">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="717d7-142">Descreve a importância de um item.</span><span class="sxs-lookup"><span data-stu-id="717d7-142">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="717d7-143">Inresponderto</span><span class="sxs-lookup"><span data-stu-id="717d7-143">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="717d7-144">Representa o identificador do item para o qual este item é uma resposta.</span><span class="sxs-lookup"><span data-stu-id="717d7-144">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="717d7-145">Isenviado</span><span class="sxs-lookup"><span data-stu-id="717d7-145">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="717d7-146">Indica se um item foi enviado para a pasta padrão da pasta de saída.</span><span class="sxs-lookup"><span data-stu-id="717d7-146">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="717d7-147">IsDraft</span><span class="sxs-lookup"><span data-stu-id="717d7-147">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="717d7-148">Indica se um item ainda não foi enviado.</span><span class="sxs-lookup"><span data-stu-id="717d7-148">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="717d7-149">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="717d7-149">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="717d7-150">Indica se um usuário enviou um item para ele.</span><span class="sxs-lookup"><span data-stu-id="717d7-150">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="717d7-151">IsResend</span><span class="sxs-lookup"><span data-stu-id="717d7-151">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="717d7-152">Indica se o item foi enviado anteriormente.</span><span class="sxs-lookup"><span data-stu-id="717d7-152">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="717d7-153">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="717d7-153">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="717d7-154">Indica se o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="717d7-154">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="717d7-155">Propriedadeinternetmessageheaders</span><span class="sxs-lookup"><span data-stu-id="717d7-155">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="717d7-156">Representa a coleção de todos os cabeçalhos de mensagens da Internet contidos em um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="717d7-156">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="717d7-157">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="717d7-157">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="717d7-158">Representa a data e a hora em que um item em uma caixa de correio foi enviado.</span><span class="sxs-lookup"><span data-stu-id="717d7-158">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="717d7-159">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="717d7-159">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="717d7-160">Representa a data e a hora em que um determinado item da caixa de correio foi criado.</span><span class="sxs-lookup"><span data-stu-id="717d7-160">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="717d7-161">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="717d7-161">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="717d7-162">Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="717d7-162">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="717d7-163">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="717d7-163">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="717d7-164">Representa a data e a hora em que o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="717d7-164">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="717d7-165">Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="717d7-165">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="717d7-166">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="717d7-166">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="717d7-167">Indica se um lembrete foi definido para um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="717d7-167">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="717d7-168">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="717d7-168">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="717d7-169">Representa o número de minutos antes de um evento quando um lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="717d7-169">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="717d7-170">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="717d7-170">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="717d7-171">Representa a cadeia de caracteres de exibição usada para o conteúdo da linha CC.</span><span class="sxs-lookup"><span data-stu-id="717d7-171">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="717d7-172">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários CC.</span><span class="sxs-lookup"><span data-stu-id="717d7-172">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="717d7-173">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="717d7-173">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="717d7-174">Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa para.</span><span class="sxs-lookup"><span data-stu-id="717d7-174">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="717d7-175">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários.</span><span class="sxs-lookup"><span data-stu-id="717d7-175">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="717d7-176">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="717d7-176">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="717d7-177">Representa uma propriedade que será definida como **true** se um item tiver um anexo.</span><span class="sxs-lookup"><span data-stu-id="717d7-177">Represents a property that is set to **true** if an item has an attachment.</span></span> <span data-ttu-id="717d7-178">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="717d7-178">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="717d7-179">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="717d7-179">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="717d7-180">Identifica as propriedades estendidas em pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="717d7-180">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="717d7-181">Cultura</span><span class="sxs-lookup"><span data-stu-id="717d7-181">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="717d7-182">Representa a cultura de um determinado item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="717d7-182">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="717d7-183">Sender</span><span class="sxs-lookup"><span data-stu-id="717d7-183">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="717d7-184">Identifica o remetente de um item.</span><span class="sxs-lookup"><span data-stu-id="717d7-184">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="717d7-185">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="717d7-185">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="717d7-186">Contém um conjunto de destinatários de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="717d7-186">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="717d7-187">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="717d7-187">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="717d7-188">Representa uma coleção de destinatários que receberão uma cópia da mensagem.</span><span class="sxs-lookup"><span data-stu-id="717d7-188">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="717d7-189">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="717d7-189">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="717d7-190">Representa uma coleção de destinatários para receber uma cópia oculta (Cco) de um email.</span><span class="sxs-lookup"><span data-stu-id="717d7-190">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="717d7-191">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="717d7-191">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="717d7-192">Indica se o remetente de um item solicita uma confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="717d7-192">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="717d7-193">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="717d7-193">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="717d7-194">Indica se o remetente de um item solicita uma confirmação de entrega.</span><span class="sxs-lookup"><span data-stu-id="717d7-194">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="717d7-195">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="717d7-195">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="717d7-196">Contém uma ID binária que representa o thread ao qual esta mensagem pertence.</span><span class="sxs-lookup"><span data-stu-id="717d7-196">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="717d7-197">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="717d7-197">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="717d7-198">Representa o identificador de conversa.</span><span class="sxs-lookup"><span data-stu-id="717d7-198">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="717d7-199">De</span><span class="sxs-lookup"><span data-stu-id="717d7-199">From</span></span>](from.md) <br/> |<span data-ttu-id="717d7-200">Representa o endereço a partir do qual a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="717d7-200">Represents the address from which the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="717d7-201">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="717d7-201">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="717d7-202">Representa o identificador de mensagem da Internet de um item.</span><span class="sxs-lookup"><span data-stu-id="717d7-202">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="717d7-203">IsRead</span><span class="sxs-lookup"><span data-stu-id="717d7-203">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="717d7-204">Indica se uma mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="717d7-204">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="717d7-205">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="717d7-205">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="717d7-206">Indica se uma resposta a uma mensagem de email é solicitada.</span><span class="sxs-lookup"><span data-stu-id="717d7-206">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="717d7-207">References</span><span class="sxs-lookup"><span data-stu-id="717d7-207">References</span></span>](references.md) <br/> |<span data-ttu-id="717d7-208">Representa o cabeçalho da Usenet que é usado para associar respostas com suas mensagens originais.</span><span class="sxs-lookup"><span data-stu-id="717d7-208">Represents the Usenet header that is used to associate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="717d7-209">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="717d7-209">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="717d7-210">Identifica um conjunto de endereços para os quais as respostas devem ser enviadas.</span><span class="sxs-lookup"><span data-stu-id="717d7-210">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="717d7-211">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="717d7-211">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="717d7-212">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="717d7-212">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="717d7-213">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="717d7-213">This element is read-only.</span></span> <span data-ttu-id="717d7-214">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="717d7-214">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="717d7-215">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="717d7-215">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="717d7-216">Identifica o representante em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="717d7-216">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="717d7-217">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="717d7-217">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="717d7-218">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="717d7-218">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="717d7-219">Identifica o principal em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="717d7-219">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="717d7-220">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="717d7-220">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="717d7-221">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="717d7-221">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="717d7-222">Representa o novo conteúdo do corpo de um item de postagem.</span><span class="sxs-lookup"><span data-stu-id="717d7-222">Represents the new body content of a post item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="717d7-223">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="717d7-223">Parent elements</span></span>

|<span data-ttu-id="717d7-224">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="717d7-224">**Element**</span></span>|<span data-ttu-id="717d7-225">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="717d7-225">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="717d7-226">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="717d7-226">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="717d7-227">Descreve todos os itens que estão adjacentes a um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="717d7-227">Describes all items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="717d7-228">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="717d7-228">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="717d7-229">Descreve todos os itens que entram em conflito com um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="717d7-229">Describes all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="717d7-230">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="717d7-230">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="717d7-231">Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="717d7-231">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="717d7-232">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="717d7-232">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="717d7-233">Contém uma matriz de itens a serem criados na pasta que é identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="717d7-233">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="717d7-234">Comentários</span><span class="sxs-lookup"><span data-stu-id="717d7-234">Remarks</span></span>

<span data-ttu-id="717d7-235">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="717d7-235">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="717d7-236">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="717d7-236">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="717d7-237">Namespace</span><span class="sxs-lookup"><span data-stu-id="717d7-237">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="717d7-238">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="717d7-238">Schema Name</span></span>  <br/> |<span data-ttu-id="717d7-239">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="717d7-239">Types schema</span></span>  <br/> |
|<span data-ttu-id="717d7-240">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="717d7-240">Validation File</span></span>  <br/> |<span data-ttu-id="717d7-241">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="717d7-241">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="717d7-242">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="717d7-242">Can be Empty</span></span>  <br/> |<span data-ttu-id="717d7-243">False</span><span class="sxs-lookup"><span data-stu-id="717d7-243">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="717d7-244">Confira também</span><span class="sxs-lookup"><span data-stu-id="717d7-244">See also</span></span>



- [<span data-ttu-id="717d7-245">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="717d7-245">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

