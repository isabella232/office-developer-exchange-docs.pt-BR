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
description: O elemento ItemChange contém um identificador de item e as atualizações para aplicar ao item.
ms.openlocfilehash: d10ce96cacb0be7411c4e8230ebc9b2803b7a5b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824145"
---
# <a name="itemchange"></a><span data-ttu-id="dcfae-103">ItemChange</span><span class="sxs-lookup"><span data-stu-id="dcfae-103">ItemChange</span></span>

<span data-ttu-id="dcfae-104">O elemento **ItemChange** contém um identificador de item e as atualizações para aplicar ao item.</span><span class="sxs-lookup"><span data-stu-id="dcfae-104">The **ItemChange** element contains an item identifier and the updates to apply to the item.</span></span> 
  
[<span data-ttu-id="dcfae-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="dcfae-105">UpdateItem</span></span>](updateitem.md)
  
[<span data-ttu-id="dcfae-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="dcfae-106">ItemChanges</span></span>](itemchanges.md)
  
[<span data-ttu-id="dcfae-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="dcfae-107">ItemChange</span></span>](itemchange.md)
  
```xml
<ItemChange>
   <ItemId/>
   <Updates>...</Updates>
</ItemChange>
```

 <span data-ttu-id="dcfae-108">**ItemChangeType**</span><span class="sxs-lookup"><span data-stu-id="dcfae-108">**ItemChangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dcfae-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="dcfae-109">Attributes and elements</span></span>

<span data-ttu-id="dcfae-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dcfae-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dcfae-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="dcfae-111">Attributes</span></span>

<span data-ttu-id="dcfae-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="dcfae-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dcfae-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dcfae-113">Child elements</span></span>

|<span data-ttu-id="dcfae-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dcfae-114">**Element**</span></span>|<span data-ttu-id="dcfae-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dcfae-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcfae-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="dcfae-116">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="dcfae-117">Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="dcfae-117">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="dcfae-118">Esse elemento é necessário se o elemento [OccurrenceItemId](occurrenceitemid.md) ou [RecurringMasterItemId](recurringmasteritemid.md) não for usado.</span><span class="sxs-lookup"><span data-stu-id="dcfae-118">This element is required if the [OccurrenceItemId](occurrenceitemid.md) or [RecurringMasterItemId](recurringmasteritemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="dcfae-119">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="dcfae-119">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="dcfae-120">Identifica uma única ocorrência de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="dcfae-120">Identifies a single occurrence of a recurring item.</span></span> <span data-ttu-id="dcfae-121">Esse elemento é obrigatório se usada.</span><span class="sxs-lookup"><span data-stu-id="dcfae-121">This element is required if used.</span></span> <span data-ttu-id="dcfae-122">Esse elemento é necessário se o elemento [RecurringMasterItemId](recurringmasteritemid.md) ou [ItemId](itemid.md) não for usado.</span><span class="sxs-lookup"><span data-stu-id="dcfae-122">This element is required if the [RecurringMasterItemId](recurringmasteritemid.md) or [ItemId](itemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="dcfae-123">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="dcfae-123">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="dcfae-124">Identifica um item-mestre recorrência identificando um dos identificadores dos seus itens relacionados ocorrência.</span><span class="sxs-lookup"><span data-stu-id="dcfae-124">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span> <span data-ttu-id="dcfae-125">Esse elemento é obrigatório se usada.</span><span class="sxs-lookup"><span data-stu-id="dcfae-125">This element is required if used.</span></span> <span data-ttu-id="dcfae-126">Esse elemento é necessário se o elemento [OccurrenceItemId](occurrenceitemid.md) ou [ItemId](itemid.md) não for usado.</span><span class="sxs-lookup"><span data-stu-id="dcfae-126">This element is required if the [OccurrenceItemId](occurrenceitemid.md) or [ItemId](itemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="dcfae-127">Atualizações (Item)</span><span class="sxs-lookup"><span data-stu-id="dcfae-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="dcfae-128">Contém uma matriz que define append, definir e excluir as alterações nas propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="dcfae-128">Contains an array that defines append, set, and delete changes to item properties.</span></span> <span data-ttu-id="dcfae-129">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcfae-129">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dcfae-130">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dcfae-130">Parent elements</span></span>

|<span data-ttu-id="dcfae-131">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dcfae-131">**Element**</span></span>|<span data-ttu-id="dcfae-132">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dcfae-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcfae-133">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="dcfae-133">ItemChanges</span></span>](itemchanges.md) <br/> |<span data-ttu-id="dcfae-134">Contém uma matriz de elementos [ItemChange](itemchange.md) que identificam os itens e as atualizações para aplicar aos itens.</span><span class="sxs-lookup"><span data-stu-id="dcfae-134">Contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span>  <br/> <span data-ttu-id="dcfae-135">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="dcfae-135">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dcfae-136">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="dcfae-136">Remarks</span></span>

<span data-ttu-id="dcfae-137">Somente um único elemento de [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md)ou [RecurringMasterItemId](recurringmasteritemid.md) pode ser usado em um elemento **ItemChange** .</span><span class="sxs-lookup"><span data-stu-id="dcfae-137">Only a single [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md), or [RecurringMasterItemId](recurringmasteritemid.md) element can be used in an **ItemChange** element.</span></span> 
  
<span data-ttu-id="dcfae-138">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="dcfae-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dcfae-139">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="dcfae-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dcfae-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="dcfae-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dcfae-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dcfae-141">Schema Name</span></span>  <br/> |<span data-ttu-id="dcfae-142">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="dcfae-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="dcfae-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dcfae-143">Validation File</span></span>  <br/> |<span data-ttu-id="dcfae-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dcfae-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dcfae-145">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="dcfae-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="dcfae-146">False</span><span class="sxs-lookup"><span data-stu-id="dcfae-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dcfae-147">Ver também</span><span class="sxs-lookup"><span data-stu-id="dcfae-147">See also</span></span>



[<span data-ttu-id="dcfae-148">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="dcfae-148">UpdateItem operation</span></span>](updateitem-operation.md)

