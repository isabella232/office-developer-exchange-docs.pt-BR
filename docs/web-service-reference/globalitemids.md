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
ms.openlocfilehash: aa656e7f2fb78dafe5bf6013c1f7ad14e2372ba1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459423"
---
# <a name="globalitemids"></a><span data-ttu-id="b6ae4-103">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="b6ae4-103">GlobalItemIds</span></span>

<span data-ttu-id="b6ae4-104">O elemento **GlobalItemIds** contém a coleção de identificadores de item para todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b6ae4-104">The **GlobalItemIds** element contains the collection of item identifiers for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="b6ae4-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="b6ae4-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="b6ae4-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="b6ae4-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="b6ae4-107">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="b6ae4-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="b6ae4-108">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="b6ae4-108">GlobalItemIds</span></span>](globalitemids.md)
  
```XML
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

 <span data-ttu-id="b6ae4-109">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="b6ae4-109">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6ae4-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b6ae4-110">Attributes and elements</span></span>

<span data-ttu-id="b6ae4-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b6ae4-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6ae4-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="b6ae4-112">Attributes</span></span>

<span data-ttu-id="b6ae4-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6ae4-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6ae4-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b6ae4-114">Child elements</span></span>

|<span data-ttu-id="b6ae4-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b6ae4-115">**Element**</span></span>|<span data-ttu-id="b6ae4-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b6ae4-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6ae4-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="b6ae4-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="b6ae4-118">Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6ae4-118">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b6ae4-119">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="b6ae4-119">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="b6ae4-120">Identifica uma única ocorrência de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="b6ae4-120">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="b6ae4-121">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="b6ae4-121">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="b6ae4-122">Identifica um item mestre de recorrência identificando um de seus identificadores de itens de ocorrência relacionados.</span><span class="sxs-lookup"><span data-stu-id="b6ae4-122">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b6ae4-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b6ae4-123">Parent elements</span></span>

|<span data-ttu-id="b6ae4-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b6ae4-124">**Element**</span></span>|<span data-ttu-id="b6ae4-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b6ae4-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6ae4-126">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="b6ae4-126">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="b6ae4-127">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="b6ae4-127">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b6ae4-128">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b6ae4-128">Text value</span></span>

<span data-ttu-id="b6ae4-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b6ae4-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b6ae4-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="b6ae4-130">Remarks</span></span>

<span data-ttu-id="b6ae4-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="b6ae4-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6ae4-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b6ae4-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6ae4-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="b6ae4-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b6ae4-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b6ae4-134">Schema name</span></span>  <br/> |<span data-ttu-id="b6ae4-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b6ae4-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="b6ae4-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b6ae4-136">Validation file</span></span>  <br/> |<span data-ttu-id="b6ae4-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b6ae4-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b6ae4-138">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b6ae4-138">Can be empty</span></span>  <br/> |<span data-ttu-id="b6ae4-139">False</span><span class="sxs-lookup"><span data-stu-id="b6ae4-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b6ae4-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="b6ae4-140">See also</span></span>



[<span data-ttu-id="b6ae4-141">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="b6ae4-141">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="b6ae4-142">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="b6ae4-142">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="b6ae4-143">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="b6ae4-143">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

