---
title: UniqueBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueBody
api_type:
- schema
ms.assetid: 06bc95d7-121c-433b-bd27-c2b0eb8c011f
description: O elemento UniqueBody representa um fragmento HTML ou texto sem formatação que representa o corpo exclusivo desta conversa.
ms.openlocfilehash: 0a8d52c7d4eb8bda9fd41c4c25e448523185df93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461916"
---
# <a name="uniquebody"></a><span data-ttu-id="e826f-103">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="e826f-103">UniqueBody</span></span>

<span data-ttu-id="e826f-104">O elemento **UniqueBody** representa um fragmento HTML ou texto sem formatação que representa o corpo exclusivo desta conversa.</span><span class="sxs-lookup"><span data-stu-id="e826f-104">The **UniqueBody** element represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span> 
  
```XML
<UniqueBody BodyType=""/>
```

 <span data-ttu-id="e826f-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="e826f-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e826f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e826f-106">Attributes and elements</span></span>

<span data-ttu-id="e826f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e826f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e826f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e826f-108">Attributes</span></span>

|<span data-ttu-id="e826f-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="e826f-109">**Attribute**</span></span>|<span data-ttu-id="e826f-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e826f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e826f-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="e826f-111">**BodyType**</span></span> <br/> |<span data-ttu-id="e826f-112">Descreve como o corpo do item é armazenado no item.</span><span class="sxs-lookup"><span data-stu-id="e826f-112">Describes how the item body is stored in the item.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="e826f-113">Atributo BodyType</span><span class="sxs-lookup"><span data-stu-id="e826f-113">BodyType Attribute</span></span>

|<span data-ttu-id="e826f-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e826f-114">**Value**</span></span>|<span data-ttu-id="e826f-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e826f-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e826f-116">**HTML**</span><span class="sxs-lookup"><span data-stu-id="e826f-116">**HTML**</span></span> <br/> |<span data-ttu-id="e826f-117">Converte todos os corpos em HTML.</span><span class="sxs-lookup"><span data-stu-id="e826f-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="e826f-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="e826f-118">**Text**</span></span> <br/> |<span data-ttu-id="e826f-119">Converte todos os corpos em texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="e826f-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e826f-120">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e826f-120">Child elements</span></span>

<span data-ttu-id="e826f-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e826f-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e826f-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e826f-122">Parent elements</span></span>

|<span data-ttu-id="e826f-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e826f-123">**Element**</span></span>|<span data-ttu-id="e826f-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e826f-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e826f-125">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="e826f-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e826f-126">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e826f-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="e826f-127">Contato</span><span class="sxs-lookup"><span data-stu-id="e826f-127">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="e826f-128">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e826f-128">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="e826f-129">DistributionList</span><span class="sxs-lookup"><span data-stu-id="e826f-129">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="e826f-130">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e826f-130">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="e826f-131">Item</span><span class="sxs-lookup"><span data-stu-id="e826f-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="e826f-132">Representa um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e826f-132">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e826f-133">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="e826f-133">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="e826f-134">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e826f-134">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e826f-135">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="e826f-135">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="e826f-136">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e826f-136">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e826f-137">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="e826f-137">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e826f-138">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e826f-138">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e826f-139">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="e826f-139">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="e826f-140">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e826f-140">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e826f-141">Message</span><span class="sxs-lookup"><span data-stu-id="e826f-141">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e826f-142">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e826f-142">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="e826f-143">Item de postagem</span><span class="sxs-lookup"><span data-stu-id="e826f-143">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="e826f-144">Representa um item de postagem no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e826f-144">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e826f-145">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="e826f-145">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="e826f-146">Remove um item do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e826f-146">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e826f-147">Tarefa</span><span class="sxs-lookup"><span data-stu-id="e826f-147">Task</span></span>](task.md) <br/> |<span data-ttu-id="e826f-148">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e826f-148">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e826f-149">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e826f-149">Text value</span></span>

<span data-ttu-id="e826f-150">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e826f-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e826f-151">Comentários</span><span class="sxs-lookup"><span data-stu-id="e826f-151">Remarks</span></span>

<span data-ttu-id="e826f-152">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e826f-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e826f-153">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e826f-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e826f-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="e826f-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e826f-155">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e826f-155">Schema Name</span></span>  <br/> |<span data-ttu-id="e826f-156">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e826f-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="e826f-157">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e826f-157">Validation File</span></span>  <br/> |<span data-ttu-id="e826f-158">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e826f-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e826f-159">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e826f-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="e826f-160">False</span><span class="sxs-lookup"><span data-stu-id="e826f-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e826f-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="e826f-161">See also</span></span>



- [<span data-ttu-id="e826f-162">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e826f-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

