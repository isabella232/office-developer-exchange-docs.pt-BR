---
title: GlobalFlagStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalFlagStatus
api_type:
- schema
ms.assetid: 3ba300f3-3355-4cab-9e77-0dcc2902e712
description: O elemento GlobalFlagStatus contém o status do sinalizador agregados de todos os itens de conversa em uma caixa de correio.
ms.openlocfilehash: 0c560c065463b8b619f96ecef73d1120b216ca35
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2018
ms.locfileid: "19823713"
---
# <a name="globalflagstatus"></a><span data-ttu-id="a779a-103">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="a779a-103">GlobalFlagStatus</span></span>

<span data-ttu-id="a779a-104">O elemento **GlobalFlagStatus** contém o status do sinalizador agregados de todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a779a-104">The **GlobalFlagStatus** element contains the aggregated flag status for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="a779a-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="a779a-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="a779a-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="a779a-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="a779a-107">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="a779a-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="a779a-108">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="a779a-108">GlobalFlagStatus</span></span>](globalflagstatus.md)
  
```XML
<GlobalFlagStatus> NotFlagged | Flagged | Complete </GlobalFlagStatus>
```

 <span data-ttu-id="a779a-109">**FlagStatusType**</span><span class="sxs-lookup"><span data-stu-id="a779a-109">**FlagStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a779a-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a779a-110">Attributes and elements</span></span>

<span data-ttu-id="a779a-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a779a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a779a-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="a779a-112">Attributes</span></span>

<span data-ttu-id="a779a-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a779a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a779a-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a779a-114">Child elements</span></span>

<span data-ttu-id="a779a-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a779a-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a779a-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a779a-116">Parent elements</span></span>

|<span data-ttu-id="a779a-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a779a-117">**Element**</span></span>|<span data-ttu-id="a779a-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a779a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a779a-119">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="a779a-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="a779a-120">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="a779a-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a779a-121">Text value</span><span class="sxs-lookup"><span data-stu-id="a779a-121">Text value</span></span>

<span data-ttu-id="a779a-122">O valor de texto do elemento **GlobalFlagStatus** é o status do sinalizador agregados para itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="a779a-122">The text value of the **GlobalFlagStatus** element is the aggregated flag status for conversation items in the current folder.</span></span> <span data-ttu-id="a779a-123">Estes são os valores de texto possíveis:</span><span class="sxs-lookup"><span data-stu-id="a779a-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="a779a-124">**NotFlagged** - indica o status de não-sinalizado.</span><span class="sxs-lookup"><span data-stu-id="a779a-124">**NotFlagged** - Indicates the not-flagged status.</span></span> 
    
- <span data-ttu-id="a779a-125">**Sinalizado** - indica o status sinalizado.</span><span class="sxs-lookup"><span data-stu-id="a779a-125">**Flagged** - Indicates the flagged status.</span></span> 
    
- <span data-ttu-id="a779a-126">**Complete** - indica o status do sinalizador completa.</span><span class="sxs-lookup"><span data-stu-id="a779a-126">**Complete** - Indicates the complete flag status.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="a779a-127">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="a779a-127">Remarks</span></span>

<span data-ttu-id="a779a-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a779a-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a779a-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a779a-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a779a-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="a779a-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a779a-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a779a-131">Schema name</span></span>  <br/> |<span data-ttu-id="a779a-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a779a-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="a779a-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a779a-133">Validation file</span></span>  <br/> |<span data-ttu-id="a779a-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a779a-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a779a-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a779a-135">Can be empty</span></span>  <br/> |<span data-ttu-id="a779a-136">False</span><span class="sxs-lookup"><span data-stu-id="a779a-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a779a-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="a779a-137">See also</span></span>



[<span data-ttu-id="a779a-138">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="a779a-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="a779a-139">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="a779a-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="a779a-140">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="a779a-140">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

