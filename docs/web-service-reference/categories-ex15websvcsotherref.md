---
title: Categorias
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Categories
api_type:
- schema
ms.assetid: d84d4927-b524-4e62-bf3d-1f12fec8c21a
description: O elemento Categories contém uma coleção de cadeias de caracteres que identificam as categorias às quais um item na caixa de correio pertence.
ms.openlocfilehash: 0d9f7068aa81306a10436ed0ca0d45f6d3b2c3a3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462210"
---
# <a name="categories"></a><span data-ttu-id="11d1a-103">Categorias</span><span class="sxs-lookup"><span data-stu-id="11d1a-103">Categories</span></span>

<span data-ttu-id="11d1a-104">O elemento **Categories** contém uma coleção de cadeias de caracteres que identificam as categorias às quais um item na caixa de correio pertence.</span><span class="sxs-lookup"><span data-stu-id="11d1a-104">The **Categories** element contains a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span> 
  
```XML
<Categories>
   <String/>
</Categories>
```

 <span data-ttu-id="11d1a-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="11d1a-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11d1a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="11d1a-106">Attributes and elements</span></span>

<span data-ttu-id="11d1a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="11d1a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11d1a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="11d1a-108">Attributes</span></span>

<span data-ttu-id="11d1a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11d1a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="11d1a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="11d1a-110">Child elements</span></span>

|<span data-ttu-id="11d1a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="11d1a-111">**Element**</span></span>|<span data-ttu-id="11d1a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="11d1a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11d1a-113">String</span><span class="sxs-lookup"><span data-stu-id="11d1a-113">String</span></span>](string.md) <br/> |<span data-ttu-id="11d1a-114">Contém uma cadeia de caracteres que identifica uma única categoria.</span><span class="sxs-lookup"><span data-stu-id="11d1a-114">Contains a string that identifies a single category.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="11d1a-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="11d1a-115">Parent elements</span></span>

|<span data-ttu-id="11d1a-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="11d1a-116">**Element**</span></span>|<span data-ttu-id="11d1a-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="11d1a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11d1a-118">Item</span><span class="sxs-lookup"><span data-stu-id="11d1a-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="11d1a-119">Representa um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11d1a-119">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="11d1a-120">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="11d1a-120">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="11d1a-121">Remove um item do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11d1a-121">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="11d1a-122">Message</span><span class="sxs-lookup"><span data-stu-id="11d1a-122">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="11d1a-123">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11d1a-123">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="11d1a-124">Tarefa</span><span class="sxs-lookup"><span data-stu-id="11d1a-124">Task</span></span>](task.md) <br/> |<span data-ttu-id="11d1a-125">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11d1a-125">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="11d1a-126">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="11d1a-126">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="11d1a-127">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11d1a-127">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="11d1a-128">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="11d1a-128">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="11d1a-129">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="11d1a-129">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="11d1a-130">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="11d1a-130">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="11d1a-131">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11d1a-131">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="11d1a-132">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="11d1a-132">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="11d1a-133">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11d1a-133">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="11d1a-134">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="11d1a-134">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="11d1a-135">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11d1a-135">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="11d1a-136">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="11d1a-136">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="11d1a-137">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11d1a-137">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="11d1a-138">Contato</span><span class="sxs-lookup"><span data-stu-id="11d1a-138">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="11d1a-139">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11d1a-139">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="11d1a-140">DistributionList</span><span class="sxs-lookup"><span data-stu-id="11d1a-140">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="11d1a-141">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="11d1a-141">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="11d1a-142">Condições</span><span class="sxs-lookup"><span data-stu-id="11d1a-142">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="11d1a-143">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="11d1a-143">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="11d1a-144">Exceções</span><span class="sxs-lookup"><span data-stu-id="11d1a-144">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="11d1a-145">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="11d1a-145">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="11d1a-146">Conversation</span><span class="sxs-lookup"><span data-stu-id="11d1a-146">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="11d1a-147">Contém uma única ação a ser aplicada a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="11d1a-147">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="11d1a-148">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="11d1a-148">Text value</span></span>

<span data-ttu-id="11d1a-149">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="11d1a-149">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="11d1a-150">Comentários</span><span class="sxs-lookup"><span data-stu-id="11d1a-150">Remarks</span></span>

<span data-ttu-id="11d1a-151">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11d1a-151">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11d1a-152">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="11d1a-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11d1a-153">Namespace</span><span class="sxs-lookup"><span data-stu-id="11d1a-153">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="11d1a-154">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="11d1a-154">Schema Name</span></span>  <br/> |<span data-ttu-id="11d1a-155">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="11d1a-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="11d1a-156">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="11d1a-156">Validation File</span></span>  <br/> |<span data-ttu-id="11d1a-157">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="11d1a-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="11d1a-158">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="11d1a-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="11d1a-159">False</span><span class="sxs-lookup"><span data-stu-id="11d1a-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="11d1a-160">Confira também</span><span class="sxs-lookup"><span data-stu-id="11d1a-160">See also</span></span>



- [<span data-ttu-id="11d1a-161">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="11d1a-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

