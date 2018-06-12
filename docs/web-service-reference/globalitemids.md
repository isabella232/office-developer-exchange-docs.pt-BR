---
title: GlobalItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalItemIds
api_type:
- schema
ms.assetid: b0f03ce0-a4c3-47de-9360-a880a3606e42
description: O elemento GlobalItemIds contém a coleção de identificadores de item para todos os itens de conversa em uma caixa de correio.
ms.openlocfilehash: 064ebc4c612aaf569eafa56e57a27cf7153f2130
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823737"
---
# <a name="globalitemids"></a><span data-ttu-id="6e9e0-103">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="6e9e0-103">GlobalItemIds</span></span>

<span data-ttu-id="6e9e0-104">O elemento **GlobalItemIds** contém a coleção de identificadores de item para todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6e9e0-104">The **GlobalItemIds** element contains the collection of item identifiers for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="6e9e0-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="6e9e0-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="6e9e0-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="6e9e0-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="6e9e0-107">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="6e9e0-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="6e9e0-108">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="6e9e0-108">GlobalItemIds</span></span>](globalitemids.md)
  
```XML
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

 <span data-ttu-id="6e9e0-109">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="6e9e0-109">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e9e0-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6e9e0-110">Attributes and elements</span></span>

<span data-ttu-id="6e9e0-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6e9e0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e9e0-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="6e9e0-112">Attributes</span></span>

<span data-ttu-id="6e9e0-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6e9e0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e9e0-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6e9e0-114">Child elements</span></span>

|<span data-ttu-id="6e9e0-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6e9e0-115">**Element**</span></span>|<span data-ttu-id="6e9e0-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6e9e0-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e9e0-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="6e9e0-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="6e9e0-118">Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e9e0-118">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6e9e0-119">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="6e9e0-119">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="6e9e0-120">Identifica uma única ocorrência de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="6e9e0-120">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="6e9e0-121">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="6e9e0-121">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="6e9e0-122">Identifica um item-mestre recorrência identificando um dos identificadores dos seus itens relacionados ocorrência.</span><span class="sxs-lookup"><span data-stu-id="6e9e0-122">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e9e0-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6e9e0-123">Parent elements</span></span>

|<span data-ttu-id="6e9e0-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6e9e0-124">**Element**</span></span>|<span data-ttu-id="6e9e0-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6e9e0-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e9e0-126">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="6e9e0-126">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="6e9e0-127">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="6e9e0-127">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6e9e0-128">Text value</span><span class="sxs-lookup"><span data-stu-id="6e9e0-128">Text value</span></span>

<span data-ttu-id="6e9e0-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6e9e0-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6e9e0-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="6e9e0-130">Remarks</span></span>

<span data-ttu-id="6e9e0-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6e9e0-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e9e0-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6e9e0-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e9e0-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="6e9e0-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6e9e0-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6e9e0-134">Schema name</span></span>  <br/> |<span data-ttu-id="6e9e0-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6e9e0-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="6e9e0-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6e9e0-136">Validation file</span></span>  <br/> |<span data-ttu-id="6e9e0-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6e9e0-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6e9e0-138">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="6e9e0-138">Can be empty</span></span>  <br/> |<span data-ttu-id="6e9e0-139">False</span><span class="sxs-lookup"><span data-stu-id="6e9e0-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e9e0-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="6e9e0-140">See also</span></span>



[<span data-ttu-id="6e9e0-141">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="6e9e0-141">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="6e9e0-142">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="6e9e0-142">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="6e9e0-143">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="6e9e0-143">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

