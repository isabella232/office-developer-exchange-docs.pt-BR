---
title: Mensagem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Message
api_type:
- schema
ms.assetid: 2400b33c-43b2-4fc2-b6fb-275a99e0e810
description: O elemento Message representa uma mensagem de email do Microsoft Exchange.
ms.openlocfilehash: 510e97572e54f0ea0cb65fc7c75910e69cc0651f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467778"
---
# <a name="message"></a><span data-ttu-id="b5480-103">Mensagem</span><span class="sxs-lookup"><span data-stu-id="b5480-103">Message</span></span>

<span data-ttu-id="b5480-104">O elemento **Message** representa uma mensagem de email do Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5480-104">The **Message** element represents a Microsoft Exchange e-mail message.</span></span> 
  
```xml
<Message>
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
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
   <ReminderMessageData/>
</Message>
```

 <span data-ttu-id="b5480-105">**MessageType**</span><span class="sxs-lookup"><span data-stu-id="b5480-105">**MessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b5480-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b5480-106">Attributes and elements</span></span>

<span data-ttu-id="b5480-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b5480-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5480-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b5480-108">Attributes</span></span>

<span data-ttu-id="b5480-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b5480-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b5480-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b5480-110">Child elements</span></span>

|<span data-ttu-id="b5480-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b5480-111">**Element**</span></span>|<span data-ttu-id="b5480-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b5480-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5480-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="b5480-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="b5480-114">Contém o fluxo MIME (Multipurpose Internet Mail Extensions) nativo de um objeto representado no formato base64Binary.</span><span class="sxs-lookup"><span data-stu-id="b5480-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="b5480-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="b5480-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="b5480-116">Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5480-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="b5480-117">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5480-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="b5480-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="b5480-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="b5480-119">Representa o identificador da pasta pai que contém o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="b5480-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="b5480-120">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5480-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="b5480-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="b5480-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="b5480-122">Representa a classe de mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="b5480-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="b5480-123">Assunto</span><span class="sxs-lookup"><span data-stu-id="b5480-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="b5480-124">Representa o assunto de itens do repositório do Exchange e objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5480-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="b5480-125">O assunto está limitado a 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="b5480-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="b5480-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="b5480-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="b5480-127">Indica o nível de sensibilidade de um item.</span><span class="sxs-lookup"><span data-stu-id="b5480-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="b5480-128">Body</span><span class="sxs-lookup"><span data-stu-id="b5480-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="b5480-129">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="b5480-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="b5480-130">Anexos</span><span class="sxs-lookup"><span data-stu-id="b5480-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b5480-131">Contém os itens ou arquivos anexados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5480-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b5480-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="b5480-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="b5480-133">Representa a data e a hora em que um item foi recebido em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b5480-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="b5480-134">Tamanho</span><span class="sxs-lookup"><span data-stu-id="b5480-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="b5480-135">Representa o tamanho em bytes de um item.</span><span class="sxs-lookup"><span data-stu-id="b5480-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="b5480-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5480-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="b5480-137">Categorias</span><span class="sxs-lookup"><span data-stu-id="b5480-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b5480-138">Representa uma coleção de cadeias de caracteres que identificam a quais categorias um item da caixa de correio pertence.</span><span class="sxs-lookup"><span data-stu-id="b5480-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="b5480-139">Importance</span><span class="sxs-lookup"><span data-stu-id="b5480-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="b5480-140">Descreve a importância de um item.</span><span class="sxs-lookup"><span data-stu-id="b5480-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="b5480-141">Inresponderto</span><span class="sxs-lookup"><span data-stu-id="b5480-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="b5480-142">Representa o identificador do item para o qual este item é uma resposta.</span><span class="sxs-lookup"><span data-stu-id="b5480-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="b5480-143">Isenviado</span><span class="sxs-lookup"><span data-stu-id="b5480-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="b5480-144">Indica se um item foi enviado para a pasta padrão da pasta de saída.</span><span class="sxs-lookup"><span data-stu-id="b5480-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="b5480-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="b5480-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="b5480-146">Indica se um item ainda não foi enviado.</span><span class="sxs-lookup"><span data-stu-id="b5480-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="b5480-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="b5480-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="b5480-148">Indica se um usuário enviou um item para ele.</span><span class="sxs-lookup"><span data-stu-id="b5480-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="b5480-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="b5480-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="b5480-150">Indica se o item foi enviado anteriormente.</span><span class="sxs-lookup"><span data-stu-id="b5480-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="b5480-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="b5480-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="b5480-152">Indica se o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="b5480-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="b5480-153">Propriedadeinternetmessageheaders</span><span class="sxs-lookup"><span data-stu-id="b5480-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="b5480-154">Representa a coleção de todos os cabeçalhos de mensagens da Internet que estão contidos em um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b5480-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="b5480-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="b5480-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="b5480-156">Representa a data e a hora em que um item em uma caixa de correio foi enviado.</span><span class="sxs-lookup"><span data-stu-id="b5480-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="b5480-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="b5480-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="b5480-158">Representa a data e a hora em que um determinado item da caixa de correio foi criado.</span><span class="sxs-lookup"><span data-stu-id="b5480-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="b5480-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="b5480-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="b5480-160">Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5480-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b5480-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="b5480-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="b5480-162">Representa a data e a hora em que o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="b5480-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="b5480-163">Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="b5480-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="b5480-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="b5480-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="b5480-165">Indica se um lembrete foi definido para um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5480-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b5480-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="b5480-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="b5480-167">Representa o número de minutos antes de um evento quando um lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="b5480-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="b5480-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="b5480-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="b5480-169">Representa a cadeia de caracteres de exibição usada para o conteúdo da linha CC.</span><span class="sxs-lookup"><span data-stu-id="b5480-169">Represents the display string that is used for the contents of the CC line.</span></span> <span data-ttu-id="b5480-170">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários CC.</span><span class="sxs-lookup"><span data-stu-id="b5480-170">This is the concatenated string of all CC recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="b5480-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="b5480-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="b5480-172">Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa para.</span><span class="sxs-lookup"><span data-stu-id="b5480-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="b5480-173">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários.</span><span class="sxs-lookup"><span data-stu-id="b5480-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="b5480-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="b5480-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="b5480-175">Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo visível.</span><span class="sxs-lookup"><span data-stu-id="b5480-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="b5480-176">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5480-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="b5480-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="b5480-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="b5480-178">Identifica as propriedades estendidas em pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="b5480-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="b5480-179">Cultura</span><span class="sxs-lookup"><span data-stu-id="b5480-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="b5480-180">Representa a cultura de um determinado item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b5480-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="b5480-181">Sender</span><span class="sxs-lookup"><span data-stu-id="b5480-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="b5480-182">Identifica o remetente de um item.</span><span class="sxs-lookup"><span data-stu-id="b5480-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="b5480-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="b5480-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="b5480-184">Contém um conjunto de destinatários de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="b5480-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="b5480-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="b5480-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="b5480-186">Representa uma coleção de destinatários que receberão uma cópia da mensagem.</span><span class="sxs-lookup"><span data-stu-id="b5480-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="b5480-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="b5480-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="b5480-188">Representa uma coleção de destinatários para receber uma cópia oculta (Cco) de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="b5480-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="b5480-189">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="b5480-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="b5480-190">Indica se o remetente de um item solicita uma confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="b5480-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="b5480-191">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="b5480-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="b5480-192">Indica se o remetente de um item solicita uma confirmação de entrega.</span><span class="sxs-lookup"><span data-stu-id="b5480-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="b5480-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="b5480-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="b5480-194">Contém uma ID binária que representa o thread ao qual esta mensagem pertence.</span><span class="sxs-lookup"><span data-stu-id="b5480-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="b5480-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="b5480-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="b5480-196">Representa o identificador de conversa.</span><span class="sxs-lookup"><span data-stu-id="b5480-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="b5480-197">De</span><span class="sxs-lookup"><span data-stu-id="b5480-197">From</span></span>](from.md) <br/> |<span data-ttu-id="b5480-198">Representa o destinatário de quem a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="b5480-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="b5480-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="b5480-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="b5480-200">Representa o identificador de mensagem da Internet de um item.</span><span class="sxs-lookup"><span data-stu-id="b5480-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="b5480-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="b5480-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="b5480-202">Indica se uma mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="b5480-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="b5480-203">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="b5480-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="b5480-204">Indica se uma resposta a uma mensagem de email é solicitada.</span><span class="sxs-lookup"><span data-stu-id="b5480-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="b5480-205">References</span><span class="sxs-lookup"><span data-stu-id="b5480-205">References</span></span>](references.md) <br/> |<span data-ttu-id="b5480-206">Representa o cabeçalho da Usenet que é usado para correlacionar respostas com suas mensagens originais.</span><span class="sxs-lookup"><span data-stu-id="b5480-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="b5480-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="b5480-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="b5480-208">Identifica um conjunto de endereços para os quais as respostas devem ser enviadas.</span><span class="sxs-lookup"><span data-stu-id="b5480-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="b5480-209">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="b5480-209">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="b5480-210">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="b5480-210">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="b5480-211">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5480-211">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="b5480-212">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="b5480-212">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="b5480-213">Identifica o representante em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="b5480-213">Identifies the delegate in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="b5480-214">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="b5480-214">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="b5480-215">Identifica o principal em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="b5480-215">Identifies the principal in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="b5480-216">LastModified</span><span class="sxs-lookup"><span data-stu-id="b5480-216">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="b5480-217">Contém o nome de exibição do último usuário a modificar um item.</span><span class="sxs-lookup"><span data-stu-id="b5480-217">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="b5480-218">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="b5480-218">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="b5480-219">Indica quando um item foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b5480-219">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="b5480-220">Isassociated</span><span class="sxs-lookup"><span data-stu-id="b5480-220">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="b5480-221">Indica se o item está associado a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="b5480-221">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="b5480-222">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="b5480-222">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="b5480-223">Representa uma URL para concatenar ao ponto de extremidade do Microsoft Office Outlook Web App para ler um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="b5480-223">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="b5480-224">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="b5480-224">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="b5480-225">Representa uma URL para concatenar ao ponto de extremidade do Outlook Web App para editar um item no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="b5480-225">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="b5480-226">ConversationId</span><span class="sxs-lookup"><span data-stu-id="b5480-226">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="b5480-227">Contém o identificador de um item ou uma conversa.</span><span class="sxs-lookup"><span data-stu-id="b5480-227">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="b5480-228">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="b5480-228">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="b5480-229">Representa um fragmento HTML ou texto sem formatação que representa o corpo exclusivo desta conversa.</span><span class="sxs-lookup"><span data-stu-id="b5480-229">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="b5480-230">ReminderMessageData</span><span class="sxs-lookup"><span data-stu-id="b5480-230">ReminderMessageData</span></span>](remindermessagedata.md) <br/> |<span data-ttu-id="b5480-231">Contém os dados de uma mensagem de lembrete.</span><span class="sxs-lookup"><span data-stu-id="b5480-231">Contains the data for a reminder message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b5480-232">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b5480-232">Parent elements</span></span>

|<span data-ttu-id="b5480-233">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b5480-233">**Element**</span></span>|<span data-ttu-id="b5480-234">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b5480-234">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5480-235">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="b5480-235">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="b5480-236">Descreve todos os itens de calendário adjacentes a um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="b5480-236">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="b5480-237">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="b5480-237">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="b5480-238">Identifica os dados a serem acrescentados a uma única propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b5480-238">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="b5480-239">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="b5480-239">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="b5480-240">Identifica todos os itens que entram em conflito com um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="b5480-240">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="b5480-241">Create (issync)</span><span class="sxs-lookup"><span data-stu-id="b5480-241">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="b5480-242">Identifica um único item a ser criado no armazenamento do cliente local.</span><span class="sxs-lookup"><span data-stu-id="b5480-242">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="b5480-243">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="b5480-243">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="b5480-244">Representa um item do Exchange anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5480-244">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="b5480-245">Itens</span><span class="sxs-lookup"><span data-stu-id="b5480-245">Items</span></span>](items.md) <br/> |<span data-ttu-id="b5480-246">Contém uma matriz de itens.</span><span class="sxs-lookup"><span data-stu-id="b5480-246">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="b5480-247">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="b5480-247">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="b5480-248">Contém uma matriz de itens a serem criados na pasta que é identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="b5480-248">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="b5480-249">Setitemfield</span><span class="sxs-lookup"><span data-stu-id="b5480-249">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="b5480-250">Representa uma atualização de uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b5480-250">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="b5480-251">Atualização (issync)</span><span class="sxs-lookup"><span data-stu-id="b5480-251">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="b5480-252">Identifica um único item a ser atualizado no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="b5480-252">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b5480-253">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b5480-253">Text value</span></span>

<span data-ttu-id="b5480-254">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b5480-254">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b5480-255">Comentários</span><span class="sxs-lookup"><span data-stu-id="b5480-255">Remarks</span></span>

<span data-ttu-id="b5480-256">Outro elemento de **mensagem** , [Message (disponibilidade)](message-availability.md) é usado pelas operações de disponibilidade para retornar mensagens de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="b5480-256">Another **Message** element, [Message (Availability)](message-availability.md) is used by the Availability operations to return OOF messages.</span></span> 
  
<span data-ttu-id="b5480-257">Os elementos da [mensagem](message-ex15websvcsotherref.md) representam mensagens de email e todos os outros itens que não são digitados com rigidez pelo esquema dos serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="b5480-257">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="b5480-258">Itens como IPM. O compartilhamento e o IPM. InfoPath são retornados como elementos de **mensagem** .</span><span class="sxs-lookup"><span data-stu-id="b5480-258">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="b5480-259">O Exchange 2010 não retorna o elemento de **Item** base nas respostas.</span><span class="sxs-lookup"><span data-stu-id="b5480-259">Exchange 2010 does not return the base **Item** element in responses.</span></span> 
  
<span data-ttu-id="b5480-260">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5480-260">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b5480-261">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b5480-261">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5480-262">Namespace</span><span class="sxs-lookup"><span data-stu-id="b5480-262">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b5480-263">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b5480-263">Schema Name</span></span>  <br/> |<span data-ttu-id="b5480-264">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b5480-264">Types schema</span></span>  <br/> |
|<span data-ttu-id="b5480-265">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b5480-265">Validation File</span></span>  <br/> |<span data-ttu-id="b5480-266">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b5480-266">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b5480-267">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b5480-267">Can be Empty</span></span>  <br/> |<span data-ttu-id="b5480-268">False</span><span class="sxs-lookup"><span data-stu-id="b5480-268">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b5480-269">Confira também</span><span class="sxs-lookup"><span data-stu-id="b5480-269">See also</span></span>



- [<span data-ttu-id="b5480-270">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b5480-270">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

