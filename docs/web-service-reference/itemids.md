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
description: O elemento ItemIds contém as identidades exclusivas dos itens, itens de ocorrência e itens recorrentes de mestres que são usados para excluir, enviar, obter, mover ou copiar itens no armazenamento do Exchange.
ms.openlocfilehash: 1bd4d6f4593a7c3b418561269d8b29707cc6030c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824155"
---
# <a name="itemids"></a><span data-ttu-id="ec900-103">ItemIds</span><span class="sxs-lookup"><span data-stu-id="ec900-103">ItemIds</span></span>
  
<span data-ttu-id="ec900-104">O elemento **ItemIds** contém as identidades exclusivas dos itens, itens de ocorrência e itens recorrentes de mestres que são usados para excluir, enviar, obter, mover ou copiar itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec900-104">The **ItemIds** element contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span>
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

<span data-ttu-id="ec900-105">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="ec900-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ec900-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ec900-106">Attributes and elements</span></span>

<span data-ttu-id="ec900-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ec900-107">The following sections describe attributes, child elements, and parent elements.</span></span> 
  
### <a name="attributes"></a><span data-ttu-id="ec900-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ec900-108">Attributes</span></span>

<span data-ttu-id="ec900-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ec900-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec900-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ec900-110">Child elements</span></span>

|<span data-ttu-id="ec900-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ec900-111">**Element**</span></span>|<span data-ttu-id="ec900-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ec900-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec900-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="ec900-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ec900-114">Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec900-114">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ec900-115">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="ec900-115">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="ec900-116">Identifica uma única ocorrência de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="ec900-116">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="ec900-117">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="ec900-117">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="ec900-118">Identifica um item-mestre recorrência identificando um dos identificadores dos seus itens relacionados ocorrência.</span><span class="sxs-lookup"><span data-stu-id="ec900-118">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ec900-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ec900-119">Parent elements</span></span>

|<span data-ttu-id="ec900-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ec900-120">**Element**</span></span>|<span data-ttu-id="ec900-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ec900-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec900-122">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="ec900-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="ec900-123">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="ec900-123">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="ec900-124">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="ec900-124">DeleteItem</span></span>](deleteitem.md) <br/> |<span data-ttu-id="ec900-125">Define uma solicitação para excluir itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec900-125">Defines a request to delete items in the Exchange store.</span></span>  <br/> <span data-ttu-id="ec900-126">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="ec900-126">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteItem` <br/> |
|[<span data-ttu-id="ec900-127">SendItem</span><span class="sxs-lookup"><span data-stu-id="ec900-127">SendItem</span></span>](senditem.md) <br/> |<span data-ttu-id="ec900-128">O elemento raiz que define uma solicitação para enviar itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec900-128">The root element that defines a request to send items in the Exchange store.</span></span>  <br/> <span data-ttu-id="ec900-129">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="ec900-129">The following is the XPath expression to this element:</span></span>  <br/>  `/SendItem` <br/> |
|[<span data-ttu-id="ec900-130">GetItem</span><span class="sxs-lookup"><span data-stu-id="ec900-130">GetItem</span></span>](getitem.md) <br/> |<span data-ttu-id="ec900-131">Define uma solicitação para obter itens do armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec900-131">Defines a request to get items from the Exchange store.</span></span>  <br/> <span data-ttu-id="ec900-132">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="ec900-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetItem` <br/> |
|[<span data-ttu-id="ec900-133">MoveItem</span><span class="sxs-lookup"><span data-stu-id="ec900-133">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="ec900-134">Define uma solicitação para mover itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec900-134">Defines a request to move items in the Exchange store.</span></span>  <br/> <span data-ttu-id="ec900-135">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="ec900-135">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="ec900-136">CopyItem</span><span class="sxs-lookup"><span data-stu-id="ec900-136">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="ec900-137">Define uma solicitação para copiar os itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec900-137">Defines a request to copy items in the Exchange store.</span></span>  <br/> <span data-ttu-id="ec900-138">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="ec900-138">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ec900-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="ec900-139">Remarks</span></span>

<span data-ttu-id="ec900-140">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec900-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec900-141">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ec900-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec900-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="ec900-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ec900-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ec900-143">Schema Name</span></span>  <br/> |<span data-ttu-id="ec900-144">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ec900-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ec900-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ec900-145">Validation File</span></span>  <br/> |<span data-ttu-id="ec900-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ec900-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ec900-147">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ec900-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="ec900-148">False</span><span class="sxs-lookup"><span data-stu-id="ec900-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec900-149">Ver também</span><span class="sxs-lookup"><span data-stu-id="ec900-149">See also</span></span>

- [<span data-ttu-id="ec900-150">Operação DeleteItem</span><span class="sxs-lookup"><span data-stu-id="ec900-150">DeleteItem operation</span></span>](deleteitem-operation.md)
- [<span data-ttu-id="ec900-151">Operação SendItem</span><span class="sxs-lookup"><span data-stu-id="ec900-151">SendItem operation</span></span>](senditem-operation.md) 
- [<span data-ttu-id="ec900-152">Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="ec900-152">GetItem operation</span></span>](getitem-operation.md)
- [<span data-ttu-id="ec900-153">Operação MoveItem</span><span class="sxs-lookup"><span data-stu-id="ec900-153">MoveItem operation</span></span>](moveitem-operation.md)
- [<span data-ttu-id="ec900-154">Operação CopyItem</span><span class="sxs-lookup"><span data-stu-id="ec900-154">CopyItem operation</span></span>](copyitem-operation.md)
- [<span data-ttu-id="ec900-155">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="ec900-155">FindConversation operation</span></span>](findconversation-operation.md)

