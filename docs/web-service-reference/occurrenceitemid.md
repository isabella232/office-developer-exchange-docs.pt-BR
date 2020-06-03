---
title: OccurrenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OccurrenceItemId
api_type:
- schema
ms.assetid: 4a15bbc3-5b93-4193-b9ec-da32f0a9a552
description: O elemento OccurrenceItemId identifica uma única ocorrência de um item recorrente.
ms.openlocfilehash: 37c3a2442afb3302bca88ef0301e98013ff0319b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468373"
---
# <a name="occurrenceitemid"></a><span data-ttu-id="93771-103">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="93771-103">OccurrenceItemId</span></span>

<span data-ttu-id="93771-104">O elemento **OccurrenceItemId** identifica uma única ocorrência de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="93771-104">The **OccurrenceItemId** element identifies a single occurrence of a recurring item.</span></span> 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

<span data-ttu-id="93771-105">**OccurrenceItemIdType**</span><span class="sxs-lookup"><span data-stu-id="93771-105">**OccurrenceItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="93771-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="93771-106">Attributes and elements</span></span>

<span data-ttu-id="93771-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="93771-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93771-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="93771-108">Attributes</span></span>

|<span data-ttu-id="93771-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="93771-109">**Attribute**</span></span>|<span data-ttu-id="93771-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="93771-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="93771-111">**RecurringMasterId**</span><span class="sxs-lookup"><span data-stu-id="93771-111">**RecurringMasterId**</span></span> <br/> |<span data-ttu-id="93771-112">Identifica o mestre recorrente de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="93771-112">Identifies the recurring master of a recurring item.</span></span> <span data-ttu-id="93771-113">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="93771-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="93771-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="93771-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="93771-115">Identifica uma versão específica do mestre recorrente ou de uma ocorrência de item.</span><span class="sxs-lookup"><span data-stu-id="93771-115">Identifies a specific version of the recurring master or an item occurrence.</span></span> <span data-ttu-id="93771-116">Se o mestre recorrente ou qualquer uma das suas ocorrências forem alterados, o **ChangeKey** será alterado.</span><span class="sxs-lookup"><span data-stu-id="93771-116">If either the recurring master or any of its occurrences change, the **ChangeKey** changes.</span></span> <span data-ttu-id="93771-117">O **ChangeKey** é o mesmo para o mestre recorrente e todas as ocorrências.</span><span class="sxs-lookup"><span data-stu-id="93771-117">The **ChangeKey** is the same for the recurring master and all occurrences.</span></span>  <br/> |
|<span data-ttu-id="93771-118">**InstanceIndex**</span><span class="sxs-lookup"><span data-stu-id="93771-118">**InstanceIndex**</span></span> <br/> |<span data-ttu-id="93771-119">Identifica o índice da ocorrência do item.</span><span class="sxs-lookup"><span data-stu-id="93771-119">Identifies the index of the item occurrence.</span></span> <span data-ttu-id="93771-120">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="93771-120">This attribute is required.</span></span> <span data-ttu-id="93771-121">Esse valor representa um inteiro.</span><span class="sxs-lookup"><span data-stu-id="93771-121">This value represents an integer.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="93771-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="93771-122">Child elements</span></span>

<span data-ttu-id="93771-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="93771-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="93771-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="93771-124">Parent elements</span></span>

|<span data-ttu-id="93771-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="93771-125">**Element**</span></span>|<span data-ttu-id="93771-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="93771-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93771-127">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="93771-127">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="93771-128">Contém a coleção de identificadores de item para todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="93771-128">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="93771-129">ItemIds</span><span class="sxs-lookup"><span data-stu-id="93771-129">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="93771-130">Contém as identidades exclusivas de itens, itens de ocorrência e itens mestre recorrentes que são usados para excluir, enviar, obter, mover ou copiar itens no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="93771-130">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/><br/><span data-ttu-id="93771-131">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="93771-131">The following are the XPath expressions to this element:</span></span> <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/><span data-ttu-id="93771-132">**Observação**: a operação [MoveItem](moveitem-operation.md) e a operação [CopyItem](copyitem-operation.md) só funcionam com itens de calendário únicos e itens mestres recorrentes.</span><span class="sxs-lookup"><span data-stu-id="93771-132">**NOTE**: [MoveItem operation](moveitem-operation.md) and [CopyItem operation](copyitem-operation.md) only work with single calendar items and recurring master items.</span></span> <span data-ttu-id="93771-133">As ocorrências de item são inválidas com essas operações.</span><span class="sxs-lookup"><span data-stu-id="93771-133">Item occurrences are invalid with these operations.</span></span>           |
|[<span data-ttu-id="93771-134">ItemChange</span><span class="sxs-lookup"><span data-stu-id="93771-134">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="93771-135">Contém um identificador de item e as atualizações a serem aplicadas ao item.</span><span class="sxs-lookup"><span data-stu-id="93771-135">Contains an item identifier and the updates to apply to the item.</span></span><br/><br/> <span data-ttu-id="93771-136">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="93771-136">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="93771-137">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="93771-137">Text value</span></span>

<span data-ttu-id="93771-138">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="93771-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="93771-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="93771-139">Remarks</span></span>

<span data-ttu-id="93771-140">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="93771-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="93771-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93771-141">Example</span></span>

<span data-ttu-id="93771-142">O exemplo a seguir identifica a quarta ocorrência de um item recorrente que tem a identidade 34vswe4.</span><span class="sxs-lookup"><span data-stu-id="93771-142">The following example identifies the fourth occurrence of a recurring item that has the identity 34vswe4.</span></span>
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a><span data-ttu-id="93771-143">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="93771-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93771-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="93771-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="93771-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="93771-145">Schema Name</span></span>  <br/> |<span data-ttu-id="93771-146">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="93771-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="93771-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="93771-147">Validation File</span></span>  <br/> |<span data-ttu-id="93771-148">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="93771-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="93771-149">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="93771-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="93771-150">False</span><span class="sxs-lookup"><span data-stu-id="93771-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93771-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="93771-151">See also</span></span>

- [<span data-ttu-id="93771-152">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="93771-152">RecurringMasterItemId</span></span>](recurringmasteritemid.md)
- [<span data-ttu-id="93771-153">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="93771-153">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="93771-154">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="93771-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

