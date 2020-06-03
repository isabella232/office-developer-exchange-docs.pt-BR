---
title: RecurringMasterItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringMasterItemId
api_type:
- schema
ms.assetid: 5800b58c-f3d7-4d8f-acc0-d13e02f4e258
description: O elemento RecurringMasterItemId identifica um item mestre de recorrência identificando os identificadores de um de seus itens de ocorrência relacionados.
ms.openlocfilehash: 896a9ce95d619e7bb44c8158288bc4f62ce417d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529879"
---
# <a name="recurringmasteritemid"></a><span data-ttu-id="36e49-103">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="36e49-103">RecurringMasterItemId</span></span>

<span data-ttu-id="36e49-104">O elemento **RecurringMasterItemId** identifica um item mestre de recorrência identificando os identificadores de um de seus itens de ocorrência relacionados.</span><span class="sxs-lookup"><span data-stu-id="36e49-104">The **RecurringMasterItemId** element identifies a recurrence master item by identifying the identifiers of one of its related occurrence items.</span></span> 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 <span data-ttu-id="36e49-105">**RecurringMasterItemIdType**</span><span class="sxs-lookup"><span data-stu-id="36e49-105">**RecurringMasterItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36e49-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="36e49-106">Attributes and elements</span></span>

<span data-ttu-id="36e49-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="36e49-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36e49-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="36e49-108">Attributes</span></span>

|<span data-ttu-id="36e49-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="36e49-109">**Attribute**</span></span>|<span data-ttu-id="36e49-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="36e49-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="36e49-111">**Occurrences**</span><span class="sxs-lookup"><span data-stu-id="36e49-111">**OccurrenceId**</span></span> <br/> |<span data-ttu-id="36e49-112">Identifica uma única ocorrência de um item mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="36e49-112">Identifies a single occurrence of a recurring master item.</span></span> <span data-ttu-id="36e49-113">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="36e49-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="36e49-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="36e49-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="36e49-115">Identifica uma versão específica de uma única ocorrência de um item mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="36e49-115">Identifies a specific version of a single occurrence of a recurring master item.</span></span> <span data-ttu-id="36e49-116">Além disso, o item mestre recorrente também é identificado porque ele e a ocorrência única conterá a mesma chave de alteração.</span><span class="sxs-lookup"><span data-stu-id="36e49-116">Additionally, the recurring master item is also identified because it and the single occurrence will contain the same change key.</span></span> <span data-ttu-id="36e49-117">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="36e49-117">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="36e49-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="36e49-118">Child elements</span></span>

<span data-ttu-id="36e49-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="36e49-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="36e49-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="36e49-120">Parent elements</span></span>

|<span data-ttu-id="36e49-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="36e49-121">**Element**</span></span>|<span data-ttu-id="36e49-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="36e49-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36e49-123">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="36e49-123">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="36e49-124">Contém a coleção de identificadores de item para todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="36e49-124">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="36e49-125">ItemChange</span><span class="sxs-lookup"><span data-stu-id="36e49-125">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="36e49-126">Contém um identificador de item e as atualizações a serem aplicadas ao item.</span><span class="sxs-lookup"><span data-stu-id="36e49-126">Contains an item identifier and the updates to apply to the item.</span></span> <br/> <br/> <span data-ttu-id="36e49-127">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="36e49-127">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[<span data-ttu-id="36e49-128">ItemIds</span><span class="sxs-lookup"><span data-stu-id="36e49-128">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="36e49-129">Contém as identidades exclusivas de itens, itens de ocorrência e itens mestre recorrentes que são usados para excluir, enviar, obter, mover ou copiar itens no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="36e49-129">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/> <br/>  <span data-ttu-id="36e49-130">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="36e49-130">The following are the XPath expressions to this element:</span></span>  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="36e49-131">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="36e49-131">Text value</span></span>

<span data-ttu-id="36e49-132">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="36e49-132">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="36e49-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="36e49-133">Remarks</span></span>

<span data-ttu-id="36e49-134">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="36e49-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="36e49-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36e49-135">Example</span></span>

<span data-ttu-id="36e49-136">O exemplo a seguir identifica o item mestre recorrente identificando uma de suas ocorrências com o identificador 56lkjh6.</span><span class="sxs-lookup"><span data-stu-id="36e49-136">The following example identifies the recurring master item by identifying one of its occurrences with the identifier 56lkjh6.</span></span>
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a><span data-ttu-id="36e49-137">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="36e49-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36e49-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="36e49-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36e49-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="36e49-139">Schema Name</span></span>  <br/> |<span data-ttu-id="36e49-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="36e49-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="36e49-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="36e49-141">Validation File</span></span>  <br/> |<span data-ttu-id="36e49-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="36e49-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36e49-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="36e49-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="36e49-144">False</span><span class="sxs-lookup"><span data-stu-id="36e49-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36e49-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="36e49-145">See also</span></span>

- [<span data-ttu-id="36e49-146">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="36e49-146">OccurrenceItemId</span></span>](occurrenceitemid.md)
- [<span data-ttu-id="36e49-147">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="36e49-147">FindConversation operation</span></span>](findconversation-operation.md)

