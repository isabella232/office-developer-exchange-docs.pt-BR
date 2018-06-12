---
title: FlagStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FlagStatus
api_type:
- schema
ms.assetid: d5907ec5-3a60-4d83-bf85-406c54f95eb7
description: O elemento de FlagStatus contém o status do sinalizador agregados para itens de conversa na pasta atual.
ms.openlocfilehash: 59e071cbd402c49f4dcc4370059883f3f45409ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752322"
---
# <a name="flagstatus"></a><span data-ttu-id="22e4f-103">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="22e4f-103">FlagStatus</span></span>

<span data-ttu-id="22e4f-104">O elemento de **FlagStatus** contém o status do sinalizador agregados para itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="22e4f-104">The **FlagStatus** element contains the aggregated flag status for conversation items in the current folder.</span></span> 
  
[<span data-ttu-id="22e4f-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="22e4f-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="22e4f-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="22e4f-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="22e4f-107">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="22e4f-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="22e4f-108">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="22e4f-108">FlagStatus</span></span>](flagstatus.md)
  
```XML
<FlagStatus> NotFlagged | Flagged | Complete </FlagStatus>
```

 <span data-ttu-id="22e4f-109">**FlagStatusType**</span><span class="sxs-lookup"><span data-stu-id="22e4f-109">**FlagStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22e4f-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="22e4f-110">Attributes and elements</span></span>

<span data-ttu-id="22e4f-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="22e4f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22e4f-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="22e4f-112">Attributes</span></span>

<span data-ttu-id="22e4f-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="22e4f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22e4f-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="22e4f-114">Child elements</span></span>

<span data-ttu-id="22e4f-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="22e4f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="22e4f-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="22e4f-116">Parent elements</span></span>

|<span data-ttu-id="22e4f-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="22e4f-117">**Element**</span></span>|<span data-ttu-id="22e4f-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="22e4f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22e4f-119">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="22e4f-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="22e4f-120">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="22e4f-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="22e4f-121">Text value</span><span class="sxs-lookup"><span data-stu-id="22e4f-121">Text value</span></span>

<span data-ttu-id="22e4f-122">O valor de texto do elemento **FlagStatus** é o status do sinalizador agregados para itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="22e4f-122">The text value of the **FlagStatus** element is the aggregated flag status for conversation items in the current folder.</span></span> <span data-ttu-id="22e4f-123">Estes são os valores de texto possíveis:</span><span class="sxs-lookup"><span data-stu-id="22e4f-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="22e4f-124">**NotFlagged** - indica o status de não-sinalizado.</span><span class="sxs-lookup"><span data-stu-id="22e4f-124">**NotFlagged** - Indicates the not-flagged status.</span></span> 
    
- <span data-ttu-id="22e4f-125">**Sinalizado** - indica o status sinalizado.</span><span class="sxs-lookup"><span data-stu-id="22e4f-125">**Flagged** - Indicates the flagged status.</span></span> 
    
- <span data-ttu-id="22e4f-126">**Complete** - indica o status do sinalizador completa.</span><span class="sxs-lookup"><span data-stu-id="22e4f-126">**Complete** - Indicates the complete flag status.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="22e4f-127">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="22e4f-127">Remarks</span></span>

<span data-ttu-id="22e4f-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="22e4f-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22e4f-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="22e4f-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22e4f-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="22e4f-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="22e4f-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="22e4f-131">Schema name</span></span>  <br/> |<span data-ttu-id="22e4f-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="22e4f-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="22e4f-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="22e4f-133">Validation file</span></span>  <br/> |<span data-ttu-id="22e4f-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="22e4f-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="22e4f-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="22e4f-135">Can be empty</span></span>  <br/> |<span data-ttu-id="22e4f-136">False</span><span class="sxs-lookup"><span data-stu-id="22e4f-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22e4f-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="22e4f-137">See also</span></span>



[<span data-ttu-id="22e4f-138">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="22e4f-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="22e4f-139">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="22e4f-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="22e4f-140">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="22e4f-140">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

