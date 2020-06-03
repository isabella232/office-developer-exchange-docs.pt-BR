---
title: AppendToItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppendToItemField
api_type:
- schema
ms.assetid: 66dbcb4a-ae6d-4648-8610-67187bdb105c
description: O elemento AppendToItemField identifica os dados a serem acrescentados a uma única propriedade de um item durante uma operação UpdateItem.
ms.openlocfilehash: 902239155bff45d6f81989de954c9459cf012288
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466042"
---
# <a name="appendtoitemfield"></a><span data-ttu-id="5c082-103">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="5c082-103">AppendToItemField</span></span>

<span data-ttu-id="5c082-104">O elemento **AppendToItemField** identifica os dados a serem acrescentados a uma única propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="5c082-104">The **AppendToItemField** element identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>
  
- [<span data-ttu-id="5c082-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="5c082-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="5c082-106">Alterações</span><span class="sxs-lookup"><span data-stu-id="5c082-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="5c082-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="5c082-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="5c082-108">Atualizações (item)</span><span class="sxs-lookup"><span data-stu-id="5c082-108">Updates (Item)</span></span>](updates-item.md)
  
- [<span data-ttu-id="5c082-109">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="5c082-109">AppendToItemField</span></span>](appendtoitemfield.md)
  
```xml
<AppendToItemField>
   <FieldURI/>
   <Item/>
</AppendToItemField>
```

 <span data-ttu-id="5c082-110">**AppendToItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="5c082-110">**AppendToItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c082-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5c082-111">Attributes and elements</span></span>

<span data-ttu-id="5c082-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5c082-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c082-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="5c082-113">Attributes</span></span>

<span data-ttu-id="5c082-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5c082-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c082-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5c082-115">Child elements</span></span>

|<span data-ttu-id="5c082-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5c082-116">**Element**</span></span>|<span data-ttu-id="5c082-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5c082-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c082-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="5c082-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="5c082-119">Identifica as propriedades com frequência referenciadas por URI.</span><span class="sxs-lookup"><span data-stu-id="5c082-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="5c082-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="5c082-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="5c082-121">Identifica membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="5c082-121">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="5c082-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="5c082-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="5c082-123">Identifica as propriedades de MAPI estendidas a serem acrescentadas.</span><span class="sxs-lookup"><span data-stu-id="5c082-123">Identifies extended MAPI properties to append.</span></span>  <br/> |
|[<span data-ttu-id="5c082-124">Item</span><span class="sxs-lookup"><span data-stu-id="5c082-124">Item</span></span>](item.md) <br/> |<span data-ttu-id="5c082-125">Representa um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c082-125">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c082-126">Mensagem</span><span class="sxs-lookup"><span data-stu-id="5c082-126">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5c082-127">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c082-127">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="5c082-128">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="5c082-128">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="5c082-129">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c082-129">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c082-130">Contato</span><span class="sxs-lookup"><span data-stu-id="5c082-130">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="5c082-131">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c082-131">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="5c082-132">DistributionList</span><span class="sxs-lookup"><span data-stu-id="5c082-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="5c082-133">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="5c082-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="5c082-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="5c082-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="5c082-135">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c082-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c082-136">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="5c082-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="5c082-137">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c082-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c082-138">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5c082-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5c082-139">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c082-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c082-140">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="5c082-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="5c082-141">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c082-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c082-142">Tarefa</span><span class="sxs-lookup"><span data-stu-id="5c082-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="5c082-143">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c082-143">Represents a task in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c082-144">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5c082-144">Parent elements</span></span>

|<span data-ttu-id="5c082-145">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5c082-145">**Element**</span></span>|<span data-ttu-id="5c082-146">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5c082-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c082-147">Atualizações (item)</span><span class="sxs-lookup"><span data-stu-id="5c082-147">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="5c082-148">Contém uma matriz que define Append, set e Delete alterações nas propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="5c082-148">Contains an array that defines append, set, and delete changes to item properties.</span></span>  <br/> <span data-ttu-id="5c082-149">A seguir está a expressão XPath para este elemento:`/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="5c082-149">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5c082-150">Comentários</span><span class="sxs-lookup"><span data-stu-id="5c082-150">Remarks</span></span>

<span data-ttu-id="5c082-151">Apenas algumas propriedades dão suporte a operações de acréscimo.</span><span class="sxs-lookup"><span data-stu-id="5c082-151">Only certain properties support append operations.</span></span> <span data-ttu-id="5c082-152">Uma tentativa de acrescentar a uma propriedade que não oferece suporte à anexação resultará em um erro.</span><span class="sxs-lookup"><span data-stu-id="5c082-152">An attempt to append to a property that does not support appending will result in an error.</span></span>
  
<span data-ttu-id="5c082-153">Para operações de atualização, apenas uma propriedade pode ser modificada em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c082-153">For update operations, only one property can be modified within a single request.</span></span> <span data-ttu-id="5c082-154">Essa propriedade única deve ser referenciada no elemento [path](path.md) .</span><span class="sxs-lookup"><span data-stu-id="5c082-154">That single property must be referenced in the [Path](path.md) element.</span></span> <span data-ttu-id="5c082-155">O elemento **Item** nas classes derivadas pode então armazenar apenas uma única propriedade que está no contrato com o elemento **Path** único.</span><span class="sxs-lookup"><span data-stu-id="5c082-155">The **Item** element in the derived classes can then only hold a single property that is in agreement with the single **Path** element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5c082-156">O elemento [path](path.md) é abstract.</span><span class="sxs-lookup"><span data-stu-id="5c082-156">The [Path](path.md) element is abstract.</span></span> <span data-ttu-id="5c082-157">Ele deve ser substituído pelo elemento [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md)ou [ExtendedFieldURI](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="5c082-157">It must be substituted by the [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md), or [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
  
<span data-ttu-id="5c082-158">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="5c082-158">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c082-159">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5c082-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c082-160">Namespace</span><span class="sxs-lookup"><span data-stu-id="5c082-160">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5c082-161">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5c082-161">Schema Name</span></span>  <br/> |<span data-ttu-id="5c082-162">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5c082-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="5c082-163">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5c082-163">Validation File</span></span>  <br/> |<span data-ttu-id="5c082-164">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5c082-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5c082-165">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5c082-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c082-166">False</span><span class="sxs-lookup"><span data-stu-id="5c082-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c082-167">Confira também</span><span class="sxs-lookup"><span data-stu-id="5c082-167">See also</span></span>

- [<span data-ttu-id="5c082-168">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="5c082-168">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="5c082-169">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5c082-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

