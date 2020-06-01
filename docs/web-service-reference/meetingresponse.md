---
title: MeetingResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingResponse
api_type:
- schema
ms.assetid: 9f798e79-dafd-4d4d-9967-95fd8e5c0502
description: O elemento MeetingResponse representa uma resposta de reunião no repositório do Exchange.
ms.openlocfilehash: ff999a671c0321586fbc2adae6cbb5c1ad117ebf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467694"
---
# <a name="meetingresponse"></a><span data-ttu-id="1e71d-103">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="1e71d-103">MeetingResponse</span></span>

<span data-ttu-id="1e71d-104">O elemento **MeetingResponse** representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e71d-104">The **MeetingResponse** element represents a meeting response in the Exchange store.</span></span> 
  
```xml
<MeetingResponse>
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
   <AssociatedCalendarItemId/>
   <IsDelegated/>
   <IsOutOfDate/>
   <HasBeenProcessed/>
   <ResponseType/>
   <EffectiveRights/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
</MeetingResponse>
```

 <span data-ttu-id="1e71d-105">**MeetingResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1e71d-105">**MeetingResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1e71d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1e71d-106">Attributes and elements</span></span>

<span data-ttu-id="1e71d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1e71d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e71d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1e71d-108">Attributes</span></span>

<span data-ttu-id="1e71d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1e71d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1e71d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1e71d-110">Child elements</span></span>

|<span data-ttu-id="1e71d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1e71d-111">**Element**</span></span>|<span data-ttu-id="1e71d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1e71d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e71d-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="1e71d-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="1e71d-114">Contém o fluxo MIME nativo de um objeto que é representado no formato base64Binary.</span><span class="sxs-lookup"><span data-stu-id="1e71d-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="1e71d-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="1e71d-116">Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e71d-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="1e71d-117">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e71d-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="1e71d-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="1e71d-119">Representa o identificador da pasta pai que contém o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="1e71d-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="1e71d-120">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e71d-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="1e71d-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="1e71d-122">Representa a classe de mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="1e71d-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-123">Assunto</span><span class="sxs-lookup"><span data-stu-id="1e71d-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="1e71d-124">Representa o assunto de itens do repositório do Exchange e objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="1e71d-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="1e71d-125">O assunto está limitado a 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="1e71d-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="1e71d-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="1e71d-127">Indica o nível de sensibilidade de um item.</span><span class="sxs-lookup"><span data-stu-id="1e71d-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-128">Body</span><span class="sxs-lookup"><span data-stu-id="1e71d-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="1e71d-129">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="1e71d-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-130">Anexos</span><span class="sxs-lookup"><span data-stu-id="1e71d-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1e71d-131">Contém os itens ou arquivos anexados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e71d-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="1e71d-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="1e71d-133">Representa os dados e a hora em que um item foi recebido em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="1e71d-133">Represents the data and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-134">Tamanho</span><span class="sxs-lookup"><span data-stu-id="1e71d-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="1e71d-135">Representa o tamanho em bytes de um item.</span><span class="sxs-lookup"><span data-stu-id="1e71d-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="1e71d-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e71d-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-137">Categorias</span><span class="sxs-lookup"><span data-stu-id="1e71d-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1e71d-138">Representa uma coleção de cadeias de caracteres que identificam a quais categorias um item da caixa de correio pertence.</span><span class="sxs-lookup"><span data-stu-id="1e71d-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-139">Importance</span><span class="sxs-lookup"><span data-stu-id="1e71d-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="1e71d-140">Descreve a importância de um item.</span><span class="sxs-lookup"><span data-stu-id="1e71d-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-141">Inresponderto</span><span class="sxs-lookup"><span data-stu-id="1e71d-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="1e71d-142">Representa o identificador do item para o qual este item é uma resposta.</span><span class="sxs-lookup"><span data-stu-id="1e71d-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-143">Isenviado</span><span class="sxs-lookup"><span data-stu-id="1e71d-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="1e71d-144">Indica se um item foi enviado para a pasta padrão da pasta de saída.</span><span class="sxs-lookup"><span data-stu-id="1e71d-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="1e71d-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="1e71d-146">Indica se um item ainda não foi enviado.</span><span class="sxs-lookup"><span data-stu-id="1e71d-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="1e71d-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="1e71d-148">Indica se um usuário enviou um item para ele.</span><span class="sxs-lookup"><span data-stu-id="1e71d-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="1e71d-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="1e71d-150">Indica se o item foi enviado anteriormente.</span><span class="sxs-lookup"><span data-stu-id="1e71d-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="1e71d-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="1e71d-152">Indica se o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="1e71d-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-153">Propriedadeinternetmessageheaders</span><span class="sxs-lookup"><span data-stu-id="1e71d-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="1e71d-154">Representa a coleção de todos os cabeçalhos de mensagens da Internet que estão contidos em um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="1e71d-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="1e71d-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="1e71d-156">Representa a data e a hora em que um item em uma caixa de correio foi enviado.</span><span class="sxs-lookup"><span data-stu-id="1e71d-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="1e71d-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="1e71d-158">Representa a data e a hora em que um determinado item da caixa de correio foi criado.</span><span class="sxs-lookup"><span data-stu-id="1e71d-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="1e71d-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="1e71d-160">Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e71d-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="1e71d-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="1e71d-162">Representa a data e a hora em que o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="1e71d-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="1e71d-163">Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="1e71d-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="1e71d-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="1e71d-165">Indica se um lembrete foi definido para um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e71d-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="1e71d-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="1e71d-167">Representa o número de minutos antes de um evento quando um lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="1e71d-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="1e71d-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="1e71d-169">Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa CC.</span><span class="sxs-lookup"><span data-stu-id="1e71d-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="1e71d-170">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários CC.</span><span class="sxs-lookup"><span data-stu-id="1e71d-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="1e71d-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="1e71d-172">Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa para.</span><span class="sxs-lookup"><span data-stu-id="1e71d-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="1e71d-173">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários.</span><span class="sxs-lookup"><span data-stu-id="1e71d-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="1e71d-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="1e71d-175">Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo visível.</span><span class="sxs-lookup"><span data-stu-id="1e71d-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="1e71d-176">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e71d-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="1e71d-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="1e71d-178">Identifica as propriedades estendidas em pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="1e71d-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-179">Cultura</span><span class="sxs-lookup"><span data-stu-id="1e71d-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="1e71d-180">Representa a cultura de um determinado item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="1e71d-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-181">Sender</span><span class="sxs-lookup"><span data-stu-id="1e71d-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="1e71d-182">Identifica o remetente de um item.</span><span class="sxs-lookup"><span data-stu-id="1e71d-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="1e71d-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="1e71d-184">Contém um conjunto de destinatários de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="1e71d-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="1e71d-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="1e71d-186">Representa uma coleção de destinatários que receberão uma cópia da mensagem.</span><span class="sxs-lookup"><span data-stu-id="1e71d-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="1e71d-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="1e71d-188">Representa uma coleção de destinatários para receber uma cópia oculta (Cco) de um email.</span><span class="sxs-lookup"><span data-stu-id="1e71d-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-189">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="1e71d-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="1e71d-190">Indica se o remetente de um item solicita uma confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="1e71d-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-191">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="1e71d-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="1e71d-192">Indica se o remetente de um item solicita uma confirmação de entrega.</span><span class="sxs-lookup"><span data-stu-id="1e71d-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="1e71d-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="1e71d-194">Contém uma ID binária que representa o thread ao qual esta mensagem pertence.</span><span class="sxs-lookup"><span data-stu-id="1e71d-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="1e71d-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="1e71d-196">Representa o identificador de conversa.</span><span class="sxs-lookup"><span data-stu-id="1e71d-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-197">De</span><span class="sxs-lookup"><span data-stu-id="1e71d-197">From</span></span>](from.md) <br/> |<span data-ttu-id="1e71d-198">Representa o destinatário de quem a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="1e71d-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="1e71d-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="1e71d-200">Representa o identificador de mensagem da Internet de um item.</span><span class="sxs-lookup"><span data-stu-id="1e71d-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="1e71d-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="1e71d-202">Indica se uma mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="1e71d-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-203">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="1e71d-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="1e71d-204">Indica se uma resposta a uma mensagem de email é solicitada.</span><span class="sxs-lookup"><span data-stu-id="1e71d-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-205">References</span><span class="sxs-lookup"><span data-stu-id="1e71d-205">References</span></span>](references.md) <br/> |<span data-ttu-id="1e71d-206">Representa o cabeçalho da Usenet que é usado para correlacionar respostas com suas mensagens originais.</span><span class="sxs-lookup"><span data-stu-id="1e71d-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="1e71d-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="1e71d-208">Identifica um conjunto de endereços para os quais as respostas devem ser enviadas.</span><span class="sxs-lookup"><span data-stu-id="1e71d-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-209">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="1e71d-209">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="1e71d-210">Representa o item de calendário associado a um [MeetingMessage](meetingmessage.md).</span><span class="sxs-lookup"><span data-stu-id="1e71d-210">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="1e71d-211">IsDelegated foi removida</span><span class="sxs-lookup"><span data-stu-id="1e71d-211">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="1e71d-212">Indica se uma reunião foi tratada por uma conta com acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="1e71d-212">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-213">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="1e71d-213">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="1e71d-214">Indica se uma mensagem de reunião está desatualizada.</span><span class="sxs-lookup"><span data-stu-id="1e71d-214">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-215">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="1e71d-215">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="1e71d-216">Indica se um item de mensagem de reunião foi processado.</span><span class="sxs-lookup"><span data-stu-id="1e71d-216">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-217">ResponseType</span><span class="sxs-lookup"><span data-stu-id="1e71d-217">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="1e71d-218">Representa o tipo de resposta de destinatário recebido para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="1e71d-218">Represents the type of recipient response that is received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-219">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="1e71d-219">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="1e71d-220">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="1e71d-220">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="1e71d-221">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e71d-221">This element is read-only.</span></span> <span data-ttu-id="1e71d-222">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="1e71d-222">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="1e71d-223">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="1e71d-223">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="1e71d-224">Identifica o representante em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="1e71d-224">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="1e71d-225">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="1e71d-225">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-226">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="1e71d-226">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="1e71d-227">Identifica o principal em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="1e71d-227">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="1e71d-228">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="1e71d-228">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-229">UID</span><span class="sxs-lookup"><span data-stu-id="1e71d-229">UID</span></span>](uid.md) <br/> |<span data-ttu-id="1e71d-230">Identifica um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="1e71d-230">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-231">RecurrenceType</span><span class="sxs-lookup"><span data-stu-id="1e71d-231">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="1e71d-232">Usada para identificar uma instância específica de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="1e71d-232">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-233">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="1e71d-233">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="1e71d-234">Indica a data e a hora em que uma instância de um objeto iCalendar foi criada.</span><span class="sxs-lookup"><span data-stu-id="1e71d-234">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1e71d-235">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1e71d-235">Parent elements</span></span>

|<span data-ttu-id="1e71d-236">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1e71d-236">**Element**</span></span>|<span data-ttu-id="1e71d-237">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1e71d-237">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e71d-238">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="1e71d-238">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="1e71d-239">Identifica todos os itens de calendário adjacentes a um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="1e71d-239">Identifies all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-240">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="1e71d-240">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="1e71d-241">Identifica os dados a serem acrescentados a uma única propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="1e71d-241">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="1e71d-242">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="1e71d-242">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="1e71d-243">Identifica todos os itens que entram em conflito com um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="1e71d-243">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-244">Create (issync)</span><span class="sxs-lookup"><span data-stu-id="1e71d-244">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="1e71d-245">Identifica um único item a ser criado no armazenamento do cliente local.</span><span class="sxs-lookup"><span data-stu-id="1e71d-245">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-246">Itens</span><span class="sxs-lookup"><span data-stu-id="1e71d-246">Items</span></span>](items.md) <br/> |<span data-ttu-id="1e71d-247">Contém uma matriz de itens.</span><span class="sxs-lookup"><span data-stu-id="1e71d-247">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-248">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="1e71d-248">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="1e71d-249">Contém uma matriz de itens a serem criados.</span><span class="sxs-lookup"><span data-stu-id="1e71d-249">Contains an array of items to create.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-250">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="1e71d-250">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="1e71d-251">Representa um item do Exchange anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e71d-251">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="1e71d-252">Setitemfield</span><span class="sxs-lookup"><span data-stu-id="1e71d-252">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="1e71d-253">Representa uma atualização de uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="1e71d-253">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="1e71d-254">Atualização (issync)</span><span class="sxs-lookup"><span data-stu-id="1e71d-254">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="1e71d-255">Identifica um único item a ser atualizado no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="1e71d-255">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1e71d-256">Comentários</span><span class="sxs-lookup"><span data-stu-id="1e71d-256">Remarks</span></span>

<span data-ttu-id="1e71d-257">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="1e71d-257">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1e71d-258">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1e71d-258">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1e71d-259">Namespace</span><span class="sxs-lookup"><span data-stu-id="1e71d-259">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1e71d-260">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1e71d-260">Schema Name</span></span>  <br/> |<span data-ttu-id="1e71d-261">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1e71d-261">Types schema</span></span>  <br/> |
|<span data-ttu-id="1e71d-262">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1e71d-262">Validation File</span></span>  <br/> |<span data-ttu-id="1e71d-263">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1e71d-263">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1e71d-264">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1e71d-264">Can be Empty</span></span>  <br/> |<span data-ttu-id="1e71d-265">False</span><span class="sxs-lookup"><span data-stu-id="1e71d-265">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1e71d-266">Confira também</span><span class="sxs-lookup"><span data-stu-id="1e71d-266">See also</span></span>



- [<span data-ttu-id="1e71d-267">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1e71d-267">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

