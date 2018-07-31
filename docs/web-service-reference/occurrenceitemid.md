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
ms.openlocfilehash: 073639ecbca6ffda872e9253b7c7e44c3541f13b
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353459"
---
# <a name="occurrenceitemid"></a><span data-ttu-id="47b41-103">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="47b41-103">OccurrenceItemId</span></span>

<span data-ttu-id="47b41-104">O elemento **OccurrenceItemId** identifica uma única ocorrência de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="47b41-104">The **OccurrenceItemId** element identifies a single occurrence of a recurring item.</span></span> 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

<span data-ttu-id="47b41-105">**OccurrenceItemIdType**</span><span class="sxs-lookup"><span data-stu-id="47b41-105">**OccurrenceItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="47b41-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="47b41-106">Attributes and elements</span></span>

<span data-ttu-id="47b41-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="47b41-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47b41-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="47b41-108">Attributes</span></span>

|<span data-ttu-id="47b41-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="47b41-109">**Attribute**</span></span>|<span data-ttu-id="47b41-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47b41-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="47b41-111">**RecurringMasterId**</span><span class="sxs-lookup"><span data-stu-id="47b41-111">**RecurringMasterId**</span></span> <br/> |<span data-ttu-id="47b41-112">Identifica o mestre recorrente de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="47b41-112">Identifies the recurring master of a recurring item.</span></span> <span data-ttu-id="47b41-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="47b41-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="47b41-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="47b41-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="47b41-115">Identifica uma versão específica do mestre recorrente ou uma ocorrência de item.</span><span class="sxs-lookup"><span data-stu-id="47b41-115">Identifies a specific version of the recurring master or an item occurrence.</span></span> <span data-ttu-id="47b41-116">Se o mestre recorrente ou qualquer um dos seus ocorrências alterar, altera a **ChangeKey** .</span><span class="sxs-lookup"><span data-stu-id="47b41-116">If either the recurring master or any of its occurrences change, the **ChangeKey** changes.</span></span> <span data-ttu-id="47b41-117">A **ChangeKey** é a mesma para o mestre recorrente e todas as ocorrências.</span><span class="sxs-lookup"><span data-stu-id="47b41-117">The **ChangeKey** is the same for the recurring master and all occurrences.</span></span>  <br/> |
|<span data-ttu-id="47b41-118">**InstanceIndex**</span><span class="sxs-lookup"><span data-stu-id="47b41-118">**InstanceIndex**</span></span> <br/> |<span data-ttu-id="47b41-119">Identifica o índice da ocorrência item.</span><span class="sxs-lookup"><span data-stu-id="47b41-119">Identifies the index of the item occurrence.</span></span> <span data-ttu-id="47b41-120">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="47b41-120">This attribute is required.</span></span> <span data-ttu-id="47b41-121">Esse valor representa um número inteiro.</span><span class="sxs-lookup"><span data-stu-id="47b41-121">This value represents an integer.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="47b41-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="47b41-122">Child elements</span></span>

<span data-ttu-id="47b41-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="47b41-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="47b41-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="47b41-124">Parent elements</span></span>

|<span data-ttu-id="47b41-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="47b41-125">**Element**</span></span>|<span data-ttu-id="47b41-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47b41-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47b41-127">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="47b41-127">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="47b41-128">Contém o conjunto de identificadores de item para todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="47b41-128">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="47b41-129">ItemIds</span><span class="sxs-lookup"><span data-stu-id="47b41-129">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="47b41-130">Contém as identidades exclusivas dos itens, itens de ocorrência e itens recorrentes de mestres que são usados para excluir, enviar, obter, mover ou copiar itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="47b41-130">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/><br/><span data-ttu-id="47b41-131">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="47b41-131">The following are the XPath expressions to this element:</span></span> <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/><span data-ttu-id="47b41-132">**Observação**: [operação MoveItem](moveitem-operation.md) e [operação CopyItem](copyitem-operation.md) só funcionam com itens de calendário único e itens recorrentes de mestres.</span><span class="sxs-lookup"><span data-stu-id="47b41-132">**NOTE**: [MoveItem operation](moveitem-operation.md) and [CopyItem operation](copyitem-operation.md) only work with single calendar items and recurring master items.</span></span> <span data-ttu-id="47b41-133">Ocorrências de item são inválidas com essas operações.</span><span class="sxs-lookup"><span data-stu-id="47b41-133">Item occurrences are invalid with these operations.</span></span>           |
|[<span data-ttu-id="47b41-134">ItemChange</span><span class="sxs-lookup"><span data-stu-id="47b41-134">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="47b41-135">Contém um identificador de item e as atualizações para aplicar ao item.</span><span class="sxs-lookup"><span data-stu-id="47b41-135">Contains an item identifier and the updates to apply to the item.</span></span><br/><br/> <span data-ttu-id="47b41-136">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="47b41-136">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="47b41-137">Text value</span><span class="sxs-lookup"><span data-stu-id="47b41-137">Text value</span></span>

<span data-ttu-id="47b41-138">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="47b41-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="47b41-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="47b41-139">Remarks</span></span>

<span data-ttu-id="47b41-140">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="47b41-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="47b41-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47b41-141">Example</span></span>

<span data-ttu-id="47b41-142">O exemplo a seguir identifica a quarta ocorrência de um item recorrente que tem o 34vswe4 de identidade.</span><span class="sxs-lookup"><span data-stu-id="47b41-142">The following example identifies the fourth occurrence of a recurring item that has the identity 34vswe4.</span></span>
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a><span data-ttu-id="47b41-143">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="47b41-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47b41-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="47b41-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="47b41-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="47b41-145">Schema Name</span></span>  <br/> |<span data-ttu-id="47b41-146">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="47b41-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="47b41-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="47b41-147">Validation File</span></span>  <br/> |<span data-ttu-id="47b41-148">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="47b41-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="47b41-149">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="47b41-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="47b41-150">False</span><span class="sxs-lookup"><span data-stu-id="47b41-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47b41-151">Ver também</span><span class="sxs-lookup"><span data-stu-id="47b41-151">See also</span></span>

- [<span data-ttu-id="47b41-152">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="47b41-152">RecurringMasterItemId</span></span>](recurringmasteritemid.md)
- [<span data-ttu-id="47b41-153">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="47b41-153">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="47b41-154">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="47b41-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

