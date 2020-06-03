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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461916"
---
# <a name="uniquebody"></a><span data-ttu-id="be663-103">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="be663-103">UniqueBody</span></span>

<span data-ttu-id="be663-104">O elemento **UniqueBody** representa um fragmento HTML ou texto sem formatação que representa o corpo exclusivo desta conversa.</span><span class="sxs-lookup"><span data-stu-id="be663-104">The **UniqueBody** element represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span> 
  
```XML
<UniqueBody BodyType=""/>
```

 <span data-ttu-id="be663-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="be663-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be663-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="be663-106">Attributes and elements</span></span>

<span data-ttu-id="be663-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="be663-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be663-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="be663-108">Attributes</span></span>

|<span data-ttu-id="be663-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="be663-109">**Attribute**</span></span>|<span data-ttu-id="be663-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="be663-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="be663-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="be663-111">**BodyType**</span></span> <br/> |<span data-ttu-id="be663-112">Descreve como o corpo do item é armazenado no item.</span><span class="sxs-lookup"><span data-stu-id="be663-112">Describes how the item body is stored in the item.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="be663-113">Atributo BodyType</span><span class="sxs-lookup"><span data-stu-id="be663-113">BodyType Attribute</span></span>

|<span data-ttu-id="be663-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="be663-114">**Value**</span></span>|<span data-ttu-id="be663-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="be663-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="be663-116">**HTML**</span><span class="sxs-lookup"><span data-stu-id="be663-116">**HTML**</span></span> <br/> |<span data-ttu-id="be663-117">Converte todos os corpos em HTML.</span><span class="sxs-lookup"><span data-stu-id="be663-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="be663-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="be663-118">**Text**</span></span> <br/> |<span data-ttu-id="be663-119">Converte todos os corpos em texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="be663-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="be663-120">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="be663-120">Child elements</span></span>

<span data-ttu-id="be663-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="be663-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="be663-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="be663-122">Parent elements</span></span>

|<span data-ttu-id="be663-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="be663-123">**Element**</span></span>|<span data-ttu-id="be663-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="be663-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be663-125">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="be663-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="be663-126">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be663-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="be663-127">Contato</span><span class="sxs-lookup"><span data-stu-id="be663-127">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="be663-128">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be663-128">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="be663-129">DistributionList</span><span class="sxs-lookup"><span data-stu-id="be663-129">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="be663-130">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="be663-130">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="be663-131">Item</span><span class="sxs-lookup"><span data-stu-id="be663-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="be663-132">Representa um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be663-132">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be663-133">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="be663-133">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="be663-134">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be663-134">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be663-135">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="be663-135">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="be663-136">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be663-136">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be663-137">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="be663-137">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="be663-138">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be663-138">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be663-139">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="be663-139">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="be663-140">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be663-140">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be663-141">Mensagem</span><span class="sxs-lookup"><span data-stu-id="be663-141">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="be663-142">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be663-142">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="be663-143">Item de postagem</span><span class="sxs-lookup"><span data-stu-id="be663-143">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="be663-144">Representa um item de postagem no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be663-144">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be663-145">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="be663-145">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="be663-146">Remove um item do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be663-146">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be663-147">Tarefa</span><span class="sxs-lookup"><span data-stu-id="be663-147">Task</span></span>](task.md) <br/> |<span data-ttu-id="be663-148">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be663-148">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="be663-149">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="be663-149">Text value</span></span>

<span data-ttu-id="be663-150">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="be663-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="be663-151">Comentários</span><span class="sxs-lookup"><span data-stu-id="be663-151">Remarks</span></span>

<span data-ttu-id="be663-152">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be663-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be663-153">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="be663-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be663-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="be663-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="be663-155">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="be663-155">Schema Name</span></span>  <br/> |<span data-ttu-id="be663-156">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="be663-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="be663-157">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="be663-157">Validation File</span></span>  <br/> |<span data-ttu-id="be663-158">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="be663-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="be663-159">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="be663-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="be663-160">False</span><span class="sxs-lookup"><span data-stu-id="be663-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="be663-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="be663-161">See also</span></span>



- [<span data-ttu-id="be663-162">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="be663-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

