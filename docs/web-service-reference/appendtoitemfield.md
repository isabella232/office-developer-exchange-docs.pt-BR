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
ms.openlocfilehash: b432399e84ee4a3fd7edc5d3f803079435c79143
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751106"
---
# <a name="appendtoitemfield"></a><span data-ttu-id="93594-103">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="93594-103">AppendToItemField</span></span>

<span data-ttu-id="93594-104">O elemento **AppendToItemField** identifica os dados a serem acrescentados a uma única propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="93594-104">The **AppendToItemField** element identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>
  
- [<span data-ttu-id="93594-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="93594-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="93594-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="93594-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="93594-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="93594-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="93594-108">Atualizações (Item)</span><span class="sxs-lookup"><span data-stu-id="93594-108">Updates (Item)</span></span>](updates-item.md)
  
- [<span data-ttu-id="93594-109">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="93594-109">AppendToItemField</span></span>](appendtoitemfield.md)
  
```xml
<AppendToItemField>
   <FieldURI/>
   <Item/>
</AppendToItemField>
```

 <span data-ttu-id="93594-110">**AppendToItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="93594-110">**AppendToItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93594-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="93594-111">Attributes and elements</span></span>

<span data-ttu-id="93594-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="93594-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93594-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="93594-113">Attributes</span></span>

<span data-ttu-id="93594-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="93594-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93594-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="93594-115">Child elements</span></span>

|<span data-ttu-id="93594-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="93594-116">**Element**</span></span>|<span data-ttu-id="93594-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="93594-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93594-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="93594-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="93594-119">Identifica as propriedades frequentemente referenciadas pelo URI.</span><span class="sxs-lookup"><span data-stu-id="93594-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="93594-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="93594-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="93594-121">Identifica a membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="93594-121">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="93594-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="93594-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="93594-123">Identifica as propriedades estendidas de MAPI para acrescentar.</span><span class="sxs-lookup"><span data-stu-id="93594-123">Identifies extended MAPI properties to append.</span></span>  <br/> |
|[<span data-ttu-id="93594-124">1.1</span><span class="sxs-lookup"><span data-stu-id="93594-124">Item</span></span>](item.md) <br/> |<span data-ttu-id="93594-125">Representa um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="93594-125">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="93594-126">Mensagem</span><span class="sxs-lookup"><span data-stu-id="93594-126">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="93594-127">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="93594-127">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="93594-128">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="93594-128">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="93594-129">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="93594-129">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="93594-130">Contato</span><span class="sxs-lookup"><span data-stu-id="93594-130">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="93594-131">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="93594-131">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="93594-132">DistributionList</span><span class="sxs-lookup"><span data-stu-id="93594-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="93594-133">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="93594-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="93594-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="93594-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="93594-135">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="93594-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="93594-136">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="93594-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="93594-137">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="93594-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="93594-138">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="93594-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="93594-139">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="93594-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="93594-140">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="93594-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="93594-141">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="93594-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="93594-142">Task</span><span class="sxs-lookup"><span data-stu-id="93594-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="93594-143">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="93594-143">Represents a task in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93594-144">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="93594-144">Parent elements</span></span>

|<span data-ttu-id="93594-145">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="93594-145">**Element**</span></span>|<span data-ttu-id="93594-146">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="93594-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93594-147">Atualizações (Item)</span><span class="sxs-lookup"><span data-stu-id="93594-147">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="93594-148">Contém uma matriz que define append, definir e excluir as alterações nas propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="93594-148">Contains an array that defines append, set, and delete changes to item properties.</span></span>  <br/> <span data-ttu-id="93594-149">Este é a expressão XPath para esse elemento:`/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="93594-149">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="93594-150">Comentários</span><span class="sxs-lookup"><span data-stu-id="93594-150">Remarks</span></span>

<span data-ttu-id="93594-151">Somente determinado propriedades de suporte acrescentar operações.</span><span class="sxs-lookup"><span data-stu-id="93594-151">Only certain properties support append operations.</span></span> <span data-ttu-id="93594-152">Uma tentativa de acrescente uma propriedade que não oferece suporte a acrescentando resultará em erro.</span><span class="sxs-lookup"><span data-stu-id="93594-152">An attempt to append to a property that does not support appending will result in an error.</span></span>
  
<span data-ttu-id="93594-153">Para operações de atualização, apenas uma propriedade pode ser modificada dentro de uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="93594-153">For update operations, only one property can be modified within a single request.</span></span> <span data-ttu-id="93594-154">Que a única propriedade deve ser referenciada no elemento de [caminho](path.md) .</span><span class="sxs-lookup"><span data-stu-id="93594-154">That single property must be referenced in the [Path](path.md) element.</span></span> <span data-ttu-id="93594-155">O elemento do **Item** nas classes derivadas pode conter apenas uma única propriedade que é a conformidade com o único elemento de **caminho** .</span><span class="sxs-lookup"><span data-stu-id="93594-155">The **Item** element in the derived classes can then only hold a single property that is in agreement with the single **Path** element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="93594-156">O elemento de [caminho](path.md) é abstrato.</span><span class="sxs-lookup"><span data-stu-id="93594-156">The [Path](path.md) element is abstract.</span></span> <span data-ttu-id="93594-157">Deve ser substituída pelo elemento [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md)ou [ExtendedFieldURI](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="93594-157">It must be substituted by the [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md), or [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
  
<span data-ttu-id="93594-158">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="93594-158">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93594-159">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="93594-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93594-160">Namespace</span><span class="sxs-lookup"><span data-stu-id="93594-160">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="93594-161">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="93594-161">Schema Name</span></span>  <br/> |<span data-ttu-id="93594-162">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="93594-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="93594-163">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="93594-163">Validation File</span></span>  <br/> |<span data-ttu-id="93594-164">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="93594-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="93594-165">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="93594-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="93594-166">False</span><span class="sxs-lookup"><span data-stu-id="93594-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93594-167">Ver também</span><span class="sxs-lookup"><span data-stu-id="93594-167">See also</span></span>

- [<span data-ttu-id="93594-168">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="93594-168">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="93594-169">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="93594-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

