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
description: O elemento MeetingResponse representa uma resposta de reunião no armazenamento do Exchange.
ms.openlocfilehash: c5f9f3ac2fcd12e9c95f663311c33cdd36783251
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824446"
---
# <a name="meetingresponse"></a><span data-ttu-id="2dea1-103">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="2dea1-103">MeetingResponse</span></span>

<span data-ttu-id="2dea1-104">O elemento **MeetingResponse** representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2dea1-104">The **MeetingResponse** element represents a meeting response in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="2dea1-105">**MeetingResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="2dea1-105">**MeetingResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2dea1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2dea1-106">Attributes and elements</span></span>

<span data-ttu-id="2dea1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2dea1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2dea1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2dea1-108">Attributes</span></span>

<span data-ttu-id="2dea1-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2dea1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2dea1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2dea1-110">Child elements</span></span>

|<span data-ttu-id="2dea1-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2dea1-111">**Element**</span></span>|<span data-ttu-id="2dea1-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2dea1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2dea1-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="2dea1-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="2dea1-114">Contém o fluxo MIME nativo de um objeto que é representado no formato base64Binary.</span><span class="sxs-lookup"><span data-stu-id="2dea1-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="2dea1-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="2dea1-116">Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2dea1-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="2dea1-117">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2dea1-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="2dea1-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="2dea1-119">Representa o identificador da pasta pai que contém o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="2dea1-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="2dea1-120">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2dea1-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="2dea1-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="2dea1-122">Representa a classe de mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="2dea1-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-123">Assunto</span><span class="sxs-lookup"><span data-stu-id="2dea1-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="2dea1-124">Representa o assunto para armazenar itens do Exchange e objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="2dea1-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="2dea1-125">O assunto é limitado a 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="2dea1-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="2dea1-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="2dea1-127">Indica o nível de sensibilidade de um item.</span><span class="sxs-lookup"><span data-stu-id="2dea1-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-128">Corpo</span><span class="sxs-lookup"><span data-stu-id="2dea1-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="2dea1-129">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="2dea1-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-130">Anexos</span><span class="sxs-lookup"><span data-stu-id="2dea1-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2dea1-131">Contém os itens ou arquivos que estejam anexados a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2dea1-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="2dea1-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="2dea1-133">Representa a data e hora em que um item em uma caixa de correio foi recebido.</span><span class="sxs-lookup"><span data-stu-id="2dea1-133">Represents the data and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-134">Size</span><span class="sxs-lookup"><span data-stu-id="2dea1-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="2dea1-135">Representa o tamanho em bytes de um item.</span><span class="sxs-lookup"><span data-stu-id="2dea1-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="2dea1-136">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2dea1-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-137">Categorias</span><span class="sxs-lookup"><span data-stu-id="2dea1-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2dea1-138">Representa uma coleção de cadeias de caracteres que identificam a quais categorias de um item na caixa de correio pertence.</span><span class="sxs-lookup"><span data-stu-id="2dea1-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-139">Importância</span><span class="sxs-lookup"><span data-stu-id="2dea1-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="2dea1-140">Descreve a importância de um item.</span><span class="sxs-lookup"><span data-stu-id="2dea1-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="2dea1-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="2dea1-142">Representa o identificador do item ao qual este item é uma resposta.</span><span class="sxs-lookup"><span data-stu-id="2dea1-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="2dea1-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="2dea1-144">Indica se um item foi enviado à pasta padrão caixa de saída.</span><span class="sxs-lookup"><span data-stu-id="2dea1-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="2dea1-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="2dea1-146">Indica se um item ainda não foi enviado.</span><span class="sxs-lookup"><span data-stu-id="2dea1-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="2dea1-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="2dea1-148">Indica se um usuário enviada a um item para si mesmo.</span><span class="sxs-lookup"><span data-stu-id="2dea1-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="2dea1-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="2dea1-150">Indica se o item anteriormente foi enviado.</span><span class="sxs-lookup"><span data-stu-id="2dea1-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="2dea1-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="2dea1-152">Indica se o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="2dea1-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="2dea1-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="2dea1-154">Representa a coleção de todos os cabeçalhos de mensagem da Internet que está contido dentro de um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2dea1-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="2dea1-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="2dea1-156">Representa a data e hora em que um item em uma caixa de correio foi enviado.</span><span class="sxs-lookup"><span data-stu-id="2dea1-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="2dea1-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="2dea1-158">Representa a data e hora em que um determinado item na caixa de correio foi criado.</span><span class="sxs-lookup"><span data-stu-id="2dea1-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="2dea1-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="2dea1-160">Contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2dea1-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="2dea1-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="2dea1-162">Representa a data e hora quando o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="2dea1-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="2dea1-163">Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="2dea1-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="2dea1-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="2dea1-165">Indica se um lembrete tiver sido definido para um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2dea1-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="2dea1-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="2dea1-167">Representa o número de minutos antes de um evento, quando um lembrete é exibido.</span><span class="sxs-lookup"><span data-stu-id="2dea1-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="2dea1-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="2dea1-169">Representa a cadeia de caracteres de exibição que é usada para o conteúdo da caixa Cc.</span><span class="sxs-lookup"><span data-stu-id="2dea1-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="2dea1-170">Esta é a cadeia de caracteres concatenada de todos os nomes de exibição destinatários Cc.</span><span class="sxs-lookup"><span data-stu-id="2dea1-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="2dea1-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="2dea1-172">Representa a cadeia de caracteres de exibição que é usada para o conteúdo da caixa para.</span><span class="sxs-lookup"><span data-stu-id="2dea1-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="2dea1-173">Esta é a cadeia de caracteres concatenada de todos os aos nomes de exibição do destinatário.</span><span class="sxs-lookup"><span data-stu-id="2dea1-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="2dea1-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="2dea1-175">Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo visível.</span><span class="sxs-lookup"><span data-stu-id="2dea1-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="2dea1-176">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2dea1-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="2dea1-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="2dea1-178">Identifica as propriedades estendidas em pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="2dea1-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-179">Cultura</span><span class="sxs-lookup"><span data-stu-id="2dea1-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="2dea1-180">Representa a cultura de um determinado item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2dea1-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-181">Sender</span><span class="sxs-lookup"><span data-stu-id="2dea1-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="2dea1-182">Identifica o remetente de um item.</span><span class="sxs-lookup"><span data-stu-id="2dea1-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="2dea1-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="2dea1-184">Contém um conjunto de destinatários de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="2dea1-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="2dea1-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="2dea1-186">Representa uma coleção dos destinatários que receberão uma cópia da mensagem.</span><span class="sxs-lookup"><span data-stu-id="2dea1-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="2dea1-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="2dea1-188">Representa uma coleção de destinatários para receber uma cópia oculta (Cco) de um email.</span><span class="sxs-lookup"><span data-stu-id="2dea1-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-189">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2dea1-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="2dea1-190">Indica se o remetente de um item solicita uma confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="2dea1-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-191">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2dea1-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="2dea1-192">Indica se o remetente de um item solicita uma confirmação de entrega.</span><span class="sxs-lookup"><span data-stu-id="2dea1-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="2dea1-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="2dea1-194">Contém uma ID binária que representa o segmento ao qual esta mensagem pertence.</span><span class="sxs-lookup"><span data-stu-id="2dea1-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="2dea1-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="2dea1-196">Representa o identificador de conversa.</span><span class="sxs-lookup"><span data-stu-id="2dea1-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-197">From</span><span class="sxs-lookup"><span data-stu-id="2dea1-197">From</span></span>](from.md) <br/> |<span data-ttu-id="2dea1-198">Representa o destinatário de quem a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="2dea1-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="2dea1-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="2dea1-200">Representa o identificador de mensagem da Internet de um item.</span><span class="sxs-lookup"><span data-stu-id="2dea1-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-201">Foi lido</span><span class="sxs-lookup"><span data-stu-id="2dea1-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="2dea1-202">Indica se uma mensagem foi lido.</span><span class="sxs-lookup"><span data-stu-id="2dea1-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-203">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="2dea1-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="2dea1-204">Indica se uma resposta a uma mensagem de email é solicitada.</span><span class="sxs-lookup"><span data-stu-id="2dea1-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-205">Referências</span><span class="sxs-lookup"><span data-stu-id="2dea1-205">References</span></span>](references.md) <br/> |<span data-ttu-id="2dea1-206">Representa o cabeçalho de Usenet é usado para correlacionar respostas com suas mensagens originais.</span><span class="sxs-lookup"><span data-stu-id="2dea1-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="2dea1-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="2dea1-208">Identifica um conjunto de endereços para o qual as respostas devem ser enviadas.</span><span class="sxs-lookup"><span data-stu-id="2dea1-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-209">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="2dea1-209">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="2dea1-210">Representa o item de calendário que está associado um [MeetingMessage](meetingmessage.md).</span><span class="sxs-lookup"><span data-stu-id="2dea1-210">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="2dea1-211">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="2dea1-211">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="2dea1-212">Indica se uma reunião foi tratada por uma conta com acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="2dea1-212">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-213">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="2dea1-213">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="2dea1-214">Indica se uma mensagem de reunião desatualizada.</span><span class="sxs-lookup"><span data-stu-id="2dea1-214">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-215">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="2dea1-215">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="2dea1-216">Indica se uma mensagem de reunião item foi processada.</span><span class="sxs-lookup"><span data-stu-id="2dea1-216">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-217">ResponseType</span><span class="sxs-lookup"><span data-stu-id="2dea1-217">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="2dea1-218">Representa o tipo de destinatário resposta recebida para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="2dea1-218">Represents the type of recipient response that is received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-219">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="2dea1-219">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="2dea1-220">Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="2dea1-220">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="2dea1-221">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2dea1-221">This element is read-only.</span></span> <span data-ttu-id="2dea1-222">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2dea1-222">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="2dea1-223">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="2dea1-223">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="2dea1-224">Identifica o delegado em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="2dea1-224">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="2dea1-225">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="2dea1-225">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-226">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="2dea1-226">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="2dea1-227">Identifica a entidade em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="2dea1-227">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="2dea1-228">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="2dea1-228">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-229">UID</span><span class="sxs-lookup"><span data-stu-id="2dea1-229">UID</span></span>](uid.md) <br/> |<span data-ttu-id="2dea1-230">Identifica um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="2dea1-230">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-231">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="2dea1-231">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="2dea1-232">Usado para identificar uma instância específica de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="2dea1-232">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-233">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="2dea1-233">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="2dea1-234">Indica a data e hora em que uma instância de um objeto iCalendar foi criada.</span><span class="sxs-lookup"><span data-stu-id="2dea1-234">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2dea1-235">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2dea1-235">Parent elements</span></span>

|<span data-ttu-id="2dea1-236">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2dea1-236">**Element**</span></span>|<span data-ttu-id="2dea1-237">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2dea1-237">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2dea1-238">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="2dea1-238">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="2dea1-239">Identifica todos os itens de calendário que são adjacentes para um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="2dea1-239">Identifies all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-240">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="2dea1-240">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="2dea1-241">Identifica os dados a serem acrescentados a uma única propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="2dea1-241">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="2dea1-242">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="2dea1-242">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="2dea1-243">Identifica todos os itens que estão em conflito com um tempo de reunião.</span><span class="sxs-lookup"><span data-stu-id="2dea1-243">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-244">Criar (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="2dea1-244">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="2dea1-245">Identifica um único item para criar no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="2dea1-245">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-246">Items</span><span class="sxs-lookup"><span data-stu-id="2dea1-246">Items</span></span>](items.md) <br/> |<span data-ttu-id="2dea1-247">Contém uma matriz de itens.</span><span class="sxs-lookup"><span data-stu-id="2dea1-247">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-248">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="2dea1-248">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="2dea1-249">Contém uma matriz de itens para criar.</span><span class="sxs-lookup"><span data-stu-id="2dea1-249">Contains an array of items to create.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-250">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="2dea1-250">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="2dea1-251">Representa um item do Exchange que está anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2dea1-251">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="2dea1-252">SetItemField</span><span class="sxs-lookup"><span data-stu-id="2dea1-252">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="2dea1-253">Representa uma atualização para uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="2dea1-253">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="2dea1-254">Atualização (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="2dea1-254">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="2dea1-255">Identifica um único item a ser atualizado no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="2dea1-255">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2dea1-256">Comentários</span><span class="sxs-lookup"><span data-stu-id="2dea1-256">Remarks</span></span>

<span data-ttu-id="2dea1-257">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="2dea1-257">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2dea1-258">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2dea1-258">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2dea1-259">Namespace</span><span class="sxs-lookup"><span data-stu-id="2dea1-259">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2dea1-260">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2dea1-260">Schema Name</span></span>  <br/> |<span data-ttu-id="2dea1-261">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2dea1-261">Types schema</span></span>  <br/> |
|<span data-ttu-id="2dea1-262">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2dea1-262">Validation File</span></span>  <br/> |<span data-ttu-id="2dea1-263">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2dea1-263">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2dea1-264">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2dea1-264">Can be Empty</span></span>  <br/> |<span data-ttu-id="2dea1-265">False</span><span class="sxs-lookup"><span data-stu-id="2dea1-265">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2dea1-266">Ver também</span><span class="sxs-lookup"><span data-stu-id="2dea1-266">See also</span></span>



- [<span data-ttu-id="2dea1-267">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2dea1-267">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

