---
title: GroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupBy
api_type:
- schema
ms.assetid: 9728619b-4674-4b9d-9f6c-e75c6165966c
description: O elemento GroupBy especifica um agrupamento arbitrário para consultas do FindItem.
ms.openlocfilehash: 0d681e5376e4dd71921cc97f270211e49179db85
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530096"
---
# <a name="groupby"></a><span data-ttu-id="2980d-103">GroupBy</span><span class="sxs-lookup"><span data-stu-id="2980d-103">GroupBy</span></span>

<span data-ttu-id="2980d-104">O elemento **GroupBy** especifica um agrupamento arbitrário para consultas do FindItem.</span><span class="sxs-lookup"><span data-stu-id="2980d-104">The **GroupBy** element specifies an arbitrary grouping for FindItem queries.</span></span> 
  
- [<span data-ttu-id="2980d-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="2980d-105">FindItem</span></span>](finditem.md)
- [<span data-ttu-id="2980d-106">GroupBy</span><span class="sxs-lookup"><span data-stu-id="2980d-106">GroupBy</span></span>](groupby.md)
  
```xml
<GroupBy Order="">
   <FieldURI/>
   <AggregateOn/>
</GroupBy>
```

```xml
<GroupBy Order="">
   <ExtendededFieldURI/>
   <AggregateOn/>
</GroupBy>
```

```xml
<GroupBy Order="">
   <IndexedFieldURI/>
   <AggregateOn/>
</GroupBy>
```

<span data-ttu-id="2980d-107">**GroupBytype**</span><span class="sxs-lookup"><span data-stu-id="2980d-107">**GroupByType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2980d-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2980d-108">Attributes and elements</span></span>

<span data-ttu-id="2980d-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2980d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2980d-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="2980d-110">Attributes</span></span>

|<span data-ttu-id="2980d-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="2980d-111">**Attribute**</span></span>|<span data-ttu-id="2980d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2980d-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2980d-113">**Order**</span><span class="sxs-lookup"><span data-stu-id="2980d-113">**Order**</span></span> <br/> | <span data-ttu-id="2980d-114">Determina a ordem dos grupos na matriz de itens agrupadas que é retornada na resposta.</span><span class="sxs-lookup"><span data-stu-id="2980d-114">Determines the order of the groups in the grouped item array that is returned in the response.</span></span> <span data-ttu-id="2980d-115">Este atributo é do tipo SortDirectionType.</span><span class="sxs-lookup"><span data-stu-id="2980d-115">This attribute is of type SortDirectionType.</span></span>  <br/> |
   
#### <a name="order-attribute-values"></a><span data-ttu-id="2980d-116">Valores de atributo de ordem</span><span class="sxs-lookup"><span data-stu-id="2980d-116">Order attribute values</span></span>

|<span data-ttu-id="2980d-117">**Valor**</span><span class="sxs-lookup"><span data-stu-id="2980d-117">**Value**</span></span>|<span data-ttu-id="2980d-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2980d-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2980d-119">Crescente</span><span class="sxs-lookup"><span data-stu-id="2980d-119">Ascending</span></span>  <br/> |<span data-ttu-id="2980d-120">Os grupos são ordenados em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="2980d-120">The groups are ordered in ascending order.</span></span>  <br/> |
|<span data-ttu-id="2980d-121">Decrescente</span><span class="sxs-lookup"><span data-stu-id="2980d-121">Descending</span></span>  <br/> |<span data-ttu-id="2980d-122">Os grupos são ordenados em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="2980d-122">The groups are ordered in descending order.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2980d-123">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2980d-123">Child elements</span></span>

|<span data-ttu-id="2980d-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2980d-124">**Element**</span></span>|<span data-ttu-id="2980d-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2980d-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2980d-126">FieldURI</span><span class="sxs-lookup"><span data-stu-id="2980d-126">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="2980d-127">Identifica as propriedades com frequência referenciadas por URI.</span><span class="sxs-lookup"><span data-stu-id="2980d-127">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="2980d-128">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="2980d-128">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="2980d-129">Identifica membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="2980d-129">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="2980d-130">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="2980d-130">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="2980d-131">Identifica as propriedades de MAPI estendidas a serem obtidas, definidas ou criadas.</span><span class="sxs-lookup"><span data-stu-id="2980d-131">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="2980d-132">Agregar</span><span class="sxs-lookup"><span data-stu-id="2980d-132">AggregateOn</span></span>](aggregateon.md) <br/> |<span data-ttu-id="2980d-133">Representa o campo que é usado para determinar a ordem dos grupos em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="2980d-133">Represents the field that is used to determine the order of groups in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2980d-134">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2980d-134">Parent elements</span></span>

|<span data-ttu-id="2980d-135">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2980d-135">**Element**</span></span>|<span data-ttu-id="2980d-136">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2980d-136">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2980d-137">FindItem</span><span class="sxs-lookup"><span data-stu-id="2980d-137">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="2980d-138">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2980d-138">Defines a request to find items in a mailbox.</span></span>  <br/><br/> <span data-ttu-id="2980d-139">A seguir está a expressão XPath para este elemento:`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="2980d-139">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2980d-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="2980d-140">Remarks</span></span>

<span data-ttu-id="2980d-141">A resposta FindItem conterá uma coleção de grupos.</span><span class="sxs-lookup"><span data-stu-id="2980d-141">The FindItem response will contain a collection of groups.</span></span> <span data-ttu-id="2980d-142">Cada grupo conterá todos os itens que tiveram valores correspondentes para a propriedade **GroupBy** .</span><span class="sxs-lookup"><span data-stu-id="2980d-142">Each group will contain all items that had matching values for the **GroupBy** property.</span></span> <span data-ttu-id="2980d-143">A propriedade que determina o agrupamento é identificada no elemento [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md)ou [ExtendedFieldURI](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="2980d-143">The property that determines the grouping is identified in the [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md), or [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
  
<span data-ttu-id="2980d-144">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="2980d-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2980d-145">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2980d-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2980d-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="2980d-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2980d-147">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2980d-147">Schema Name</span></span>  <br/> |<span data-ttu-id="2980d-148">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="2980d-148">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2980d-149">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2980d-149">Validation File</span></span>  <br/> |<span data-ttu-id="2980d-150">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2980d-150">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2980d-151">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2980d-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="2980d-152">False</span><span class="sxs-lookup"><span data-stu-id="2980d-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2980d-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="2980d-153">See also</span></span>

- [<span data-ttu-id="2980d-154">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="2980d-154">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="2980d-155">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2980d-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="2980d-156">Localizar itens</span><span class="sxs-lookup"><span data-stu-id="2980d-156">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

