---
title: Atualizações (Item)
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
description: O elemento Updates contém um conjunto de elementos que definem append, definir e excluir as alterações nas propriedades do item.
ms.openlocfilehash: 13df458c783b942e1c868853c41b6247119cf123
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837938"
---
# <a name="updates-item"></a><span data-ttu-id="790df-103">Atualizações (Item)</span><span class="sxs-lookup"><span data-stu-id="790df-103">Updates (Item)</span></span>

<span data-ttu-id="790df-104">O elemento **Updates** contém um conjunto de elementos que definem append, definir e excluir as alterações nas propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="790df-104">The **Updates** element contains a set of elements that define append, set, and delete changes to item properties.</span></span> 
  
- [<span data-ttu-id="790df-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="790df-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="790df-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="790df-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="790df-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="790df-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="790df-108">Atualizações (Item)</span><span class="sxs-lookup"><span data-stu-id="790df-108">Updates (Item)</span></span>](updates-item.md)
  
```xml
<Updates>
   <AppendToItemField/>
   <SetItemField/>
   <DeleteItemField/>
</Updates>
```

<span data-ttu-id="790df-109">**NonEmptyArrayOfItemChangeDescriptionsType**</span><span class="sxs-lookup"><span data-stu-id="790df-109">**NonEmptyArrayOfItemChangeDescriptionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="790df-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="790df-110">Attributes and elements</span></span>

<span data-ttu-id="790df-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="790df-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="790df-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="790df-112">Attributes</span></span>

<span data-ttu-id="790df-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="790df-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="790df-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="790df-114">Child elements</span></span>

|<span data-ttu-id="790df-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="790df-115">**Element**</span></span>|<span data-ttu-id="790df-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="790df-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="790df-117">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="790df-117">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="790df-118">Representa os dados a serem acrescentados a uma única propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="790df-118">Represents data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="790df-119">SetItemField</span><span class="sxs-lookup"><span data-stu-id="790df-119">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="790df-120">Representa uma atualização para uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="790df-120">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="790df-121">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="790df-121">DeleteItemField</span></span>](deleteitemfield.md) <br/> |<span data-ttu-id="790df-122">Representa uma operação para excluir uma determinada propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="790df-122">Represents an operation to delete a given property from an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="790df-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="790df-123">Parent elements</span></span>

|<span data-ttu-id="790df-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="790df-124">**Element**</span></span>|<span data-ttu-id="790df-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="790df-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="790df-126">ItemChange</span><span class="sxs-lookup"><span data-stu-id="790df-126">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="790df-127">Contém um identificador de item e as atualizações para aplicar ao item.</span><span class="sxs-lookup"><span data-stu-id="790df-127">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> <span data-ttu-id="790df-128">Este é a expressão XPath para esse elemento:`/UpdateItem/ItemChanges/ItemChange[i]`</span><span class="sxs-lookup"><span data-stu-id="790df-128">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="790df-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="790df-129">Remarks</span></span>

<span data-ttu-id="790df-130">As atualizações que são definidas por esse elemento são executadas no item que é identificado pelos elementos [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md)ou [RecurringMasterItemId](recurringmasteritemid.md) .</span><span class="sxs-lookup"><span data-stu-id="790df-130">The updates that are defined by this element are performed on the item that is identified by the [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md), or [RecurringMasterItemId](recurringmasteritemid.md) elements.</span></span> 
  
<span data-ttu-id="790df-131">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="790df-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="790df-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="790df-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="790df-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="790df-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="790df-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="790df-134">Schema Name</span></span>  <br/> |<span data-ttu-id="790df-135">esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="790df-135">types schema</span></span>  <br/> |
|<span data-ttu-id="790df-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="790df-136">Validation File</span></span>  <br/> |<span data-ttu-id="790df-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="790df-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="790df-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="790df-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="790df-139">False</span><span class="sxs-lookup"><span data-stu-id="790df-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="790df-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="790df-140">See also</span></span>

- [<span data-ttu-id="790df-141">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="790df-141">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="790df-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="790df-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

