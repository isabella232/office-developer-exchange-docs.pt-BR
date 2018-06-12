---
title: ItemClasses (ArrayOfItemClassType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 971784d1-6860-4833-bb26-0e930fa11c21
description: O elemento ItemClasses contém uma lista das classes de item que representa todas as classes de item, os itens de conversa na pasta atual.
ms.openlocfilehash: 62ea5b624025b3f012249afd1763e2b393ef5caa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824150"
---
# <a name="itemclasses-arrayofitemclasstype"></a><span data-ttu-id="d3239-103">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="d3239-103">ItemClasses (ArrayOfItemClassType)</span></span>

<span data-ttu-id="d3239-104">O elemento **ItemClasses** contém uma lista das classes de item que representa todas as classes de item, os itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="d3239-104">The **ItemClasses** element contains a list of item classes that represents all the item classes of the conversation items in the current folder.</span></span> 
  
[<span data-ttu-id="d3239-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="d3239-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="d3239-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="d3239-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="d3239-107">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="d3239-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="d3239-108">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="d3239-108">ItemClasses (ArrayOfItemClassType)</span></span>](itemclasses-arrayofitemclasstype.md)
  
```XML
<ItemClasses>
    <String/>
</ItemClasses>
```

 <span data-ttu-id="d3239-109">**ArrayOfItemClassType**</span><span class="sxs-lookup"><span data-stu-id="d3239-109">**ArrayOfItemClassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3239-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d3239-110">Attributes and elements</span></span>

<span data-ttu-id="d3239-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d3239-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3239-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="d3239-112">Attributes</span></span>

<span data-ttu-id="d3239-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d3239-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3239-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d3239-114">Child elements</span></span>

|<span data-ttu-id="d3239-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d3239-115">**Element**</span></span>|<span data-ttu-id="d3239-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d3239-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3239-117">ItemClass</span><span class="sxs-lookup"><span data-stu-id="d3239-117">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="d3239-118">Representa a classe de mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="d3239-118">Represents the message class of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3239-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d3239-119">Parent elements</span></span>

|<span data-ttu-id="d3239-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d3239-120">**Element**</span></span>|<span data-ttu-id="d3239-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d3239-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3239-122">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="d3239-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="d3239-123">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="d3239-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d3239-124">Text value</span><span class="sxs-lookup"><span data-stu-id="d3239-124">Text value</span></span>

<span data-ttu-id="d3239-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d3239-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d3239-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="d3239-126">Remarks</span></span>

<span data-ttu-id="d3239-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d3239-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3239-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d3239-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3239-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="d3239-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3239-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d3239-130">Schema name</span></span>  <br/> |<span data-ttu-id="d3239-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d3239-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3239-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d3239-132">Validation file</span></span>  <br/> |<span data-ttu-id="d3239-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d3239-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3239-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d3239-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3239-135">False</span><span class="sxs-lookup"><span data-stu-id="d3239-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3239-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="d3239-136">See also</span></span>



[<span data-ttu-id="d3239-137">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="d3239-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="d3239-138">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="d3239-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="d3239-139">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="d3239-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

