---
title: Atualizações (item)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Updates
api_type:
- schema
ms.assetid: 5c1a855e-390d-4713-9d10-6e86ca392814
description: O elemento updates contém um conjunto de elementos que definem Append, set e Delete alterações nas propriedades do item.
ms.openlocfilehash: 6902ea4d3d3d9adc074745d5642cdfa6d91a9163
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456350"
---
# <a name="updates-item"></a><span data-ttu-id="ff1b2-103">Atualizações (item)</span><span class="sxs-lookup"><span data-stu-id="ff1b2-103">Updates (Item)</span></span>

<span data-ttu-id="ff1b2-104">O elemento **updates** contém um conjunto de elementos que definem Append, set e Delete alterações nas propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="ff1b2-104">The **Updates** element contains a set of elements that define append, set, and delete changes to item properties.</span></span> 
  
- [<span data-ttu-id="ff1b2-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ff1b2-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="ff1b2-106">Alterações</span><span class="sxs-lookup"><span data-stu-id="ff1b2-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="ff1b2-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="ff1b2-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="ff1b2-108">Atualizações (item)</span><span class="sxs-lookup"><span data-stu-id="ff1b2-108">Updates (Item)</span></span>](updates-item.md)
  
```xml
<Updates>
   <AppendToItemField/>
   <SetItemField/>
   <DeleteItemField/>
</Updates>
```

<span data-ttu-id="ff1b2-109">**NonEmptyArrayOfItemChangeDescriptionsType**</span><span class="sxs-lookup"><span data-stu-id="ff1b2-109">**NonEmptyArrayOfItemChangeDescriptionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ff1b2-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ff1b2-110">Attributes and elements</span></span>

<span data-ttu-id="ff1b2-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ff1b2-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff1b2-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="ff1b2-112">Attributes</span></span>

<span data-ttu-id="ff1b2-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff1b2-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff1b2-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ff1b2-114">Child elements</span></span>

|<span data-ttu-id="ff1b2-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ff1b2-115">**Element**</span></span>|<span data-ttu-id="ff1b2-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ff1b2-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff1b2-117">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="ff1b2-117">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="ff1b2-118">Representa os dados a serem acrescentados a uma única propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ff1b2-118">Represents data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ff1b2-119">Setitemfield</span><span class="sxs-lookup"><span data-stu-id="ff1b2-119">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="ff1b2-120">Representa uma atualização de uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ff1b2-120">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ff1b2-121">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="ff1b2-121">DeleteItemField</span></span>](deleteitemfield.md) <br/> |<span data-ttu-id="ff1b2-122">Representa uma operação para excluir uma determinada propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ff1b2-122">Represents an operation to delete a given property from an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ff1b2-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ff1b2-123">Parent elements</span></span>

|<span data-ttu-id="ff1b2-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ff1b2-124">**Element**</span></span>|<span data-ttu-id="ff1b2-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ff1b2-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff1b2-126">ItemChange</span><span class="sxs-lookup"><span data-stu-id="ff1b2-126">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="ff1b2-127">Contém um identificador de item e as atualizações a serem aplicadas ao item.</span><span class="sxs-lookup"><span data-stu-id="ff1b2-127">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> <span data-ttu-id="ff1b2-128">A seguir está a expressão XPath para este elemento:`/UpdateItem/ItemChanges/ItemChange[i]`</span><span class="sxs-lookup"><span data-stu-id="ff1b2-128">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ff1b2-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="ff1b2-129">Remarks</span></span>

<span data-ttu-id="ff1b2-130">As atualizações definidas por esse elemento são executadas no item que é identificado pelos elementos [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md)ou [RecurringMasterItemId](recurringmasteritemid.md) .</span><span class="sxs-lookup"><span data-stu-id="ff1b2-130">The updates that are defined by this element are performed on the item that is identified by the [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md), or [RecurringMasterItemId](recurringmasteritemid.md) elements.</span></span> 
  
<span data-ttu-id="ff1b2-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ff1b2-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff1b2-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ff1b2-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff1b2-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="ff1b2-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ff1b2-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ff1b2-134">Schema Name</span></span>  <br/> |<span data-ttu-id="ff1b2-135">esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ff1b2-135">types schema</span></span>  <br/> |
|<span data-ttu-id="ff1b2-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ff1b2-136">Validation File</span></span>  <br/> |<span data-ttu-id="ff1b2-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ff1b2-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ff1b2-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ff1b2-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff1b2-139">False</span><span class="sxs-lookup"><span data-stu-id="ff1b2-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff1b2-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="ff1b2-140">See also</span></span>

- [<span data-ttu-id="ff1b2-141">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ff1b2-141">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="ff1b2-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ff1b2-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

