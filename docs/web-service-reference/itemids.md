---
title: ItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemIds
api_type:
- schema
ms.assetid: 6b82122b-5544-4adf-91b7-ef2db7d5046f
description: O elemento ItemIds contém as identidades exclusivas de itens, itens de ocorrência e itens mestres recorrentes que são usados para excluir, enviar, obter, mover ou copiar itens no repositório do Exchange.
ms.openlocfilehash: bbd594ce2610bd625b0e16a0383fda552ee9eb19
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460600"
---
# <a name="itemids"></a><span data-ttu-id="ac5ad-103">ItemIds</span><span class="sxs-lookup"><span data-stu-id="ac5ad-103">ItemIds</span></span>
  
<span data-ttu-id="ac5ad-104">O elemento **ItemIds** contém as identidades exclusivas de itens, itens de ocorrência e itens mestres recorrentes que são usados para excluir, enviar, obter, mover ou copiar itens no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac5ad-104">The **ItemIds** element contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span>
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

<span data-ttu-id="ac5ad-105">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="ac5ad-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ac5ad-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ac5ad-106">Attributes and elements</span></span>

<span data-ttu-id="ac5ad-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ac5ad-107">The following sections describe attributes, child elements, and parent elements.</span></span> 
  
### <a name="attributes"></a><span data-ttu-id="ac5ad-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ac5ad-108">Attributes</span></span>

<span data-ttu-id="ac5ad-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac5ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac5ad-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ac5ad-110">Child elements</span></span>

|<span data-ttu-id="ac5ad-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ac5ad-111">**Element**</span></span>|<span data-ttu-id="ac5ad-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ac5ad-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac5ad-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="ac5ad-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ac5ad-114">Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac5ad-114">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ac5ad-115">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="ac5ad-115">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="ac5ad-116">Identifica uma única ocorrência de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="ac5ad-116">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="ac5ad-117">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="ac5ad-117">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="ac5ad-118">Identifica um item mestre de recorrência identificando um de seus identificadores de itens de ocorrência relacionados.</span><span class="sxs-lookup"><span data-stu-id="ac5ad-118">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ac5ad-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ac5ad-119">Parent elements</span></span>

|<span data-ttu-id="ac5ad-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ac5ad-120">**Element**</span></span>|<span data-ttu-id="ac5ad-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ac5ad-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac5ad-122">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="ac5ad-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="ac5ad-123">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="ac5ad-123">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="ac5ad-124">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="ac5ad-124">DeleteItem</span></span>](deleteitem.md) <br/> |<span data-ttu-id="ac5ad-125">Define uma solicitação para excluir itens no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac5ad-125">Defines a request to delete items in the Exchange store.</span></span>  <br/> <span data-ttu-id="ac5ad-126">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="ac5ad-126">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteItem` <br/> |
|[<span data-ttu-id="ac5ad-127">SendItem</span><span class="sxs-lookup"><span data-stu-id="ac5ad-127">SendItem</span></span>](senditem.md) <br/> |<span data-ttu-id="ac5ad-128">O elemento raiz que define uma solicitação para enviar itens no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac5ad-128">The root element that defines a request to send items in the Exchange store.</span></span>  <br/> <span data-ttu-id="ac5ad-129">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="ac5ad-129">The following is the XPath expression to this element:</span></span>  <br/>  `/SendItem` <br/> |
|[<span data-ttu-id="ac5ad-130">GetItem</span><span class="sxs-lookup"><span data-stu-id="ac5ad-130">GetItem</span></span>](getitem.md) <br/> |<span data-ttu-id="ac5ad-131">Define uma solicitação para obter itens do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac5ad-131">Defines a request to get items from the Exchange store.</span></span>  <br/> <span data-ttu-id="ac5ad-132">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="ac5ad-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetItem` <br/> |
|[<span data-ttu-id="ac5ad-133">MoveItem</span><span class="sxs-lookup"><span data-stu-id="ac5ad-133">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="ac5ad-134">Define uma solicitação para mover itens no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac5ad-134">Defines a request to move items in the Exchange store.</span></span>  <br/> <span data-ttu-id="ac5ad-135">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="ac5ad-135">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="ac5ad-136">CopyItem</span><span class="sxs-lookup"><span data-stu-id="ac5ad-136">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="ac5ad-137">Define uma solicitação para copiar itens no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac5ad-137">Defines a request to copy items in the Exchange store.</span></span>  <br/> <span data-ttu-id="ac5ad-138">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="ac5ad-138">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ac5ad-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="ac5ad-139">Remarks</span></span>

<span data-ttu-id="ac5ad-140">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac5ad-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac5ad-141">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ac5ad-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac5ad-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="ac5ad-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ac5ad-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ac5ad-143">Schema Name</span></span>  <br/> |<span data-ttu-id="ac5ad-144">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ac5ad-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ac5ad-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ac5ad-145">Validation File</span></span>  <br/> |<span data-ttu-id="ac5ad-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ac5ad-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ac5ad-147">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ac5ad-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="ac5ad-148">False</span><span class="sxs-lookup"><span data-stu-id="ac5ad-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac5ad-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="ac5ad-149">See also</span></span>

- [<span data-ttu-id="ac5ad-150">Operação DeleteItem</span><span class="sxs-lookup"><span data-stu-id="ac5ad-150">DeleteItem operation</span></span>](deleteitem-operation.md)
- [<span data-ttu-id="ac5ad-151">Operação SendItem</span><span class="sxs-lookup"><span data-stu-id="ac5ad-151">SendItem operation</span></span>](senditem-operation.md) 
- [<span data-ttu-id="ac5ad-152">Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="ac5ad-152">GetItem operation</span></span>](getitem-operation.md)
- [<span data-ttu-id="ac5ad-153">Operação MoveItem</span><span class="sxs-lookup"><span data-stu-id="ac5ad-153">MoveItem operation</span></span>](moveitem-operation.md)
- [<span data-ttu-id="ac5ad-154">Operação CopyItem</span><span class="sxs-lookup"><span data-stu-id="ac5ad-154">CopyItem operation</span></span>](copyitem-operation.md)
- [<span data-ttu-id="ac5ad-155">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="ac5ad-155">FindConversation operation</span></span>](findconversation-operation.md)

