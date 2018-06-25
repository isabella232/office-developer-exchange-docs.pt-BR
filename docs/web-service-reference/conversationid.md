---
title: ConversationId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationId
api_type:
- schema
ms.assetid: d5f1ddb3-9af3-4677-a6ba-111b304a951e
description: O elemento ConversationId contém o identificador de um item ou conversa.
ms.openlocfilehash: 1f82e6ade60fb70db4a9f026fd72d9f11cc63821
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751524"
---
# <a name="conversationid"></a><span data-ttu-id="7bec2-103">ConversationId</span><span class="sxs-lookup"><span data-stu-id="7bec2-103">ConversationId</span></span>

<span data-ttu-id="7bec2-104">O elemento **ConversationId** contém o identificador de um item ou conversa.</span><span class="sxs-lookup"><span data-stu-id="7bec2-104">The **ConversationId** element contains the identifier of an item or conversation.</span></span> 
  
```XML
<ConversationId Id="" ChangeKey="" />
```

 <span data-ttu-id="7bec2-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="7bec2-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7bec2-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7bec2-106">Attributes and elements</span></span>

<span data-ttu-id="7bec2-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7bec2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7bec2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7bec2-108">Attributes</span></span>

|<span data-ttu-id="7bec2-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="7bec2-109">**Attribute**</span></span>|<span data-ttu-id="7bec2-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7bec2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7bec2-111">**ID de**</span><span class="sxs-lookup"><span data-stu-id="7bec2-111">**Id**</span></span> <br/> |<span data-ttu-id="7bec2-112">Identifica um item específico no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bec2-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="7bec2-113">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="7bec2-113">**ChangeKey**</span></span> <br/> | <span data-ttu-id="7bec2-114">Identifica uma versão específica de um item.</span><span class="sxs-lookup"><span data-stu-id="7bec2-114">Identifies a specific version of an item.</span></span> <span data-ttu-id="7bec2-115">Um **ChangeKey** é necessária para os seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="7bec2-115">A **ChangeKey** is required for the following scenarios:</span></span>  <br/><br/><span data-ttu-id="7bec2-116">-O elemento [UpdateItem](updateitem.md) requer um **ChangeKey** se o atributo **ConflictResolution** estiver definido como resolver automaticamente.</span><span class="sxs-lookup"><span data-stu-id="7bec2-116">- The [UpdateItem](updateitem.md) element requires a **ChangeKey** if the **ConflictResolution** attribute is set to AutoResolve.</span></span> <span data-ttu-id="7bec2-117">Resolver automaticamente é um valor padrão.</span><span class="sxs-lookup"><span data-stu-id="7bec2-117">AutoResolve is a default value.</span></span> <span data-ttu-id="7bec2-118">Se o atributo **ChangeKey** não for incluído, a resposta retornará um valor [ResponseCode](responsecode.md) igual a **ErrorChangeKeyRequired**.</span><span class="sxs-lookup"><span data-stu-id="7bec2-118">If the **ChangeKey** attribute is not included, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorChangeKeyRequired**.</span></span><br/><br/><span data-ttu-id="7bec2-119">- Elementos [SendItem](senditem.md), [DeleteItem](deleteitem.md)e [DeleteFolder](deletefolder.md) exigem um **ChangeKey** testar se a operação tentada atuará após a versão mais recente de um item.</span><span class="sxs-lookup"><span data-stu-id="7bec2-119">- [SendItem](senditem.md), [DeleteItem](deleteitem.md), and [DeleteFolder](deletefolder.md) elements require a **ChangeKey** to test whether the attempted operation will act upon the most recent version of an item.</span></span> <span data-ttu-id="7bec2-120">Se o atributo **ChangeKey** não está incluído no **ItemId** ou se o **ChangeKey** estiver vazia, a resposta retornará um valor [ResponseCode](responsecode.md) igual a **ErrorStaleObject**.</span><span class="sxs-lookup"><span data-stu-id="7bec2-120">If the **ChangeKey** attribute is not included in the **ItemId** or if the **ChangeKey** is empty, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorStaleObject**.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7bec2-121">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7bec2-121">Child elements</span></span>

<span data-ttu-id="7bec2-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7bec2-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7bec2-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7bec2-123">Parent elements</span></span>

|<span data-ttu-id="7bec2-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7bec2-124">**Element**</span></span>|<span data-ttu-id="7bec2-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7bec2-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7bec2-126">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="7bec2-126">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="7bec2-127">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bec2-127">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7bec2-128">Contato</span><span class="sxs-lookup"><span data-stu-id="7bec2-128">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="7bec2-129">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bec2-129">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="7bec2-130">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="7bec2-130">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="7bec2-131">Representa uma única ação a ser aplicado a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="7bec2-131">Represents a single action to be applied to a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="7bec2-132">DistributionList</span><span class="sxs-lookup"><span data-stu-id="7bec2-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="7bec2-133">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="7bec2-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="7bec2-134">1.1</span><span class="sxs-lookup"><span data-stu-id="7bec2-134">Item</span></span>](item.md) <br/> |<span data-ttu-id="7bec2-135">Representa um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bec2-135">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7bec2-136">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="7bec2-136">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="7bec2-137">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bec2-137">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7bec2-138">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="7bec2-138">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="7bec2-139">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bec2-139">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7bec2-140">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="7bec2-140">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="7bec2-141">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bec2-141">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7bec2-142">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="7bec2-142">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="7bec2-143">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bec2-143">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7bec2-144">Mensagem</span><span class="sxs-lookup"><span data-stu-id="7bec2-144">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7bec2-145">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bec2-145">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="7bec2-146">PostItem</span><span class="sxs-lookup"><span data-stu-id="7bec2-146">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="7bec2-147">Representa um item de postagem no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bec2-147">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7bec2-148">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="7bec2-148">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="7bec2-149">Remove um item de armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bec2-149">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7bec2-150">Task</span><span class="sxs-lookup"><span data-stu-id="7bec2-150">Task</span></span>](task.md) <br/> |<span data-ttu-id="7bec2-151">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bec2-151">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7bec2-152">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="7bec2-152">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="7bec2-153">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="7bec2-153">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7bec2-154">Text value</span><span class="sxs-lookup"><span data-stu-id="7bec2-154">Text value</span></span>

<span data-ttu-id="7bec2-155">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7bec2-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7bec2-156">Comentários</span><span class="sxs-lookup"><span data-stu-id="7bec2-156">Remarks</span></span>

<span data-ttu-id="7bec2-157">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bec2-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7bec2-158">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7bec2-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7bec2-159">Namespace</span><span class="sxs-lookup"><span data-stu-id="7bec2-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7bec2-160">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7bec2-160">Schema Name</span></span>  <br/> |<span data-ttu-id="7bec2-161">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7bec2-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="7bec2-162">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7bec2-162">Validation File</span></span>  <br/> |<span data-ttu-id="7bec2-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7bec2-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7bec2-164">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7bec2-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="7bec2-165">False</span><span class="sxs-lookup"><span data-stu-id="7bec2-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7bec2-166">Ver também</span><span class="sxs-lookup"><span data-stu-id="7bec2-166">See also</span></span>

- [<span data-ttu-id="7bec2-167">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="7bec2-167">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="7bec2-168">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7bec2-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

