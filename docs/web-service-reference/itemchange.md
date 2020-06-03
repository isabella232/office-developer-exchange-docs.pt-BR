---
title: ItemChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemChange
api_type:
- schema
ms.assetid: 5cb43b02-d444-4d9c-9075-cdc5a4427daf
description: O elemento ItemChange contém um identificador de item e as atualizações a serem aplicadas ao item.
ms.openlocfilehash: 916ef1ba2c7a709ec1fd80ababd72999506773c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459914"
---
# <a name="itemchange"></a><span data-ttu-id="446b4-103">ItemChange</span><span class="sxs-lookup"><span data-stu-id="446b4-103">ItemChange</span></span>

<span data-ttu-id="446b4-104">O elemento **ItemChange** contém um identificador de item e as atualizações a serem aplicadas ao item.</span><span class="sxs-lookup"><span data-stu-id="446b4-104">The **ItemChange** element contains an item identifier and the updates to apply to the item.</span></span> 
  
- [<span data-ttu-id="446b4-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="446b4-105">UpdateItem</span></span>](updateitem.md) 
- [<span data-ttu-id="446b4-106">Alterações</span><span class="sxs-lookup"><span data-stu-id="446b4-106">ItemChanges</span></span>](itemchanges.md)
- [<span data-ttu-id="446b4-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="446b4-107">ItemChange</span></span>](itemchange.md)
  
```xml
<ItemChange>
   <ItemId/>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <OccurrenceItemId>...</OccurrenceItemId>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <RecurringMasterItemId>...</RecurringMasterItemId>
   <Updates>...</Updates>
</ItemChange>
```

<span data-ttu-id="446b4-108">**Mychangtype**</span><span class="sxs-lookup"><span data-stu-id="446b4-108">**ItemChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="446b4-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="446b4-109">Attributes and elements</span></span>

<span data-ttu-id="446b4-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="446b4-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="446b4-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="446b4-111">Attributes</span></span>

<span data-ttu-id="446b4-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="446b4-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="446b4-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="446b4-113">Child elements</span></span>

|<span data-ttu-id="446b4-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="446b4-114">**Element**</span></span>|<span data-ttu-id="446b4-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="446b4-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="446b4-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="446b4-116">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="446b4-117">Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="446b4-117">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="446b4-118">Esse elemento é necessário se o elemento [OccurrenceItemId](occurrenceitemid.md) ou [RecurringMasterItemId](recurringmasteritemid.md) não é usado.</span><span class="sxs-lookup"><span data-stu-id="446b4-118">This element is required if the [OccurrenceItemId](occurrenceitemid.md) or [RecurringMasterItemId](recurringmasteritemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="446b4-119">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="446b4-119">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="446b4-120">Identifica uma única ocorrência de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="446b4-120">Identifies a single occurrence of a recurring item.</span></span> <span data-ttu-id="446b4-121">Este elemento será necessário se for usado.</span><span class="sxs-lookup"><span data-stu-id="446b4-121">This element is required if used.</span></span> <span data-ttu-id="446b4-122">Este elemento é necessário se o elemento [RecurringMasterItemId](recurringmasteritemid.md) ou [ItemId](itemid.md) não é usado.</span><span class="sxs-lookup"><span data-stu-id="446b4-122">This element is required if the [RecurringMasterItemId](recurringmasteritemid.md) or [ItemId](itemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="446b4-123">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="446b4-123">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="446b4-124">Identifica um item mestre de recorrência identificando um de seus identificadores de itens de ocorrência relacionados.</span><span class="sxs-lookup"><span data-stu-id="446b4-124">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span> <span data-ttu-id="446b4-125">Este elemento será necessário se for usado.</span><span class="sxs-lookup"><span data-stu-id="446b4-125">This element is required if used.</span></span> <span data-ttu-id="446b4-126">Este elemento é necessário se o elemento [OccurrenceItemId](occurrenceitemid.md) ou [ItemId](itemid.md) não é usado.</span><span class="sxs-lookup"><span data-stu-id="446b4-126">This element is required if the [OccurrenceItemId](occurrenceitemid.md) or [ItemId](itemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="446b4-127">Atualizações (item)</span><span class="sxs-lookup"><span data-stu-id="446b4-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="446b4-128">Contém uma matriz que define Append, set e Delete alterações nas propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="446b4-128">Contains an array that defines append, set, and delete changes to item properties.</span></span> <span data-ttu-id="446b4-129">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="446b4-129">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="446b4-130">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="446b4-130">Parent elements</span></span>

|<span data-ttu-id="446b4-131">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="446b4-131">**Element**</span></span>|<span data-ttu-id="446b4-132">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="446b4-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="446b4-133">Alterações</span><span class="sxs-lookup"><span data-stu-id="446b4-133">ItemChanges</span></span>](itemchanges.md) <br/> |<span data-ttu-id="446b4-134">Contém uma matriz de elementos [ItemChange](itemchange.md) que identificam itens e as atualizações a serem aplicadas aos itens.</span><span class="sxs-lookup"><span data-stu-id="446b4-134">Contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span>  <br/> <span data-ttu-id="446b4-135">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="446b4-135">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="446b4-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="446b4-136">Remarks</span></span>

<span data-ttu-id="446b4-137">Somente um único elemento [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md)ou [RecurringMasterItemId](recurringmasteritemid.md) pode ser usado em um elemento **ItemChange** .</span><span class="sxs-lookup"><span data-stu-id="446b4-137">Only a single [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md), or [RecurringMasterItemId](recurringmasteritemid.md) element can be used in an **ItemChange** element.</span></span> 
  
<span data-ttu-id="446b4-138">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="446b4-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="446b4-139">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="446b4-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="446b4-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="446b4-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="446b4-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="446b4-141">Schema Name</span></span>  <br/> |<span data-ttu-id="446b4-142">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="446b4-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="446b4-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="446b4-143">Validation File</span></span>  <br/> |<span data-ttu-id="446b4-144">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="446b4-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="446b4-145">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="446b4-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="446b4-146">False</span><span class="sxs-lookup"><span data-stu-id="446b4-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="446b4-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="446b4-147">See also</span></span>

- [<span data-ttu-id="446b4-148">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="446b4-148">UpdateItem operation</span></span>](updateitem-operation.md)

