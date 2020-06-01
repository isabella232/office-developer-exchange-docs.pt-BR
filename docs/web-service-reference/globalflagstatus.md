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
description: O elemento GlobalFlagStatus contém o status de sinalizador agregado para todos os itens de conversa em uma caixa de correio.
ms.openlocfilehash: f9984a1bb7e8205a98dd3ef91f841b48a7ab9389
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459501"
---
# <a name="globalflagstatus"></a><span data-ttu-id="1a3b9-103">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="1a3b9-103">GlobalFlagStatus</span></span>

<span data-ttu-id="1a3b9-104">O elemento **GlobalFlagStatus** contém o status de sinalizador agregado para todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="1a3b9-104">The **GlobalFlagStatus** element contains the aggregated flag status for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="1a3b9-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="1a3b9-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="1a3b9-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="1a3b9-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="1a3b9-107">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="1a3b9-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="1a3b9-108">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="1a3b9-108">GlobalFlagStatus</span></span>](globalflagstatus.md)
  
```XML
<GlobalFlagStatus> NotFlagged | Flagged | Complete </GlobalFlagStatus>
```

 <span data-ttu-id="1a3b9-109">**FlagStatusType**</span><span class="sxs-lookup"><span data-stu-id="1a3b9-109">**FlagStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a3b9-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1a3b9-110">Attributes and elements</span></span>

<span data-ttu-id="1a3b9-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1a3b9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a3b9-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="1a3b9-112">Attributes</span></span>

<span data-ttu-id="1a3b9-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a3b9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a3b9-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1a3b9-114">Child elements</span></span>

<span data-ttu-id="1a3b9-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1a3b9-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1a3b9-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1a3b9-116">Parent elements</span></span>

|<span data-ttu-id="1a3b9-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1a3b9-117">**Element**</span></span>|<span data-ttu-id="1a3b9-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1a3b9-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a3b9-119">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="1a3b9-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="1a3b9-120">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="1a3b9-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1a3b9-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="1a3b9-121">Text value</span></span>

<span data-ttu-id="1a3b9-122">O valor de texto do elemento **GlobalFlagStatus** é o status de sinalizador agregado para itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="1a3b9-122">The text value of the **GlobalFlagStatus** element is the aggregated flag status for conversation items in the current folder.</span></span> <span data-ttu-id="1a3b9-123">Estes são os valores de texto possíveis:</span><span class="sxs-lookup"><span data-stu-id="1a3b9-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="1a3b9-124">Não **sinalizado** : indica o status não sinalizado.</span><span class="sxs-lookup"><span data-stu-id="1a3b9-124">**NotFlagged** - Indicates the not-flagged status.</span></span> 
    
- <span data-ttu-id="1a3b9-125">**Marcado** : indica o status sinalizado.</span><span class="sxs-lookup"><span data-stu-id="1a3b9-125">**Flagged** - Indicates the flagged status.</span></span> 
    
- <span data-ttu-id="1a3b9-126">**Concluído** -indica o status completo do sinalizador.</span><span class="sxs-lookup"><span data-stu-id="1a3b9-126">**Complete** - Indicates the complete flag status.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="1a3b9-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="1a3b9-127">Remarks</span></span>

<span data-ttu-id="1a3b9-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="1a3b9-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a3b9-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1a3b9-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a3b9-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="1a3b9-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1a3b9-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1a3b9-131">Schema name</span></span>  <br/> |<span data-ttu-id="1a3b9-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1a3b9-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="1a3b9-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1a3b9-133">Validation file</span></span>  <br/> |<span data-ttu-id="1a3b9-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1a3b9-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1a3b9-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="1a3b9-135">Can be empty</span></span>  <br/> |<span data-ttu-id="1a3b9-136">False</span><span class="sxs-lookup"><span data-stu-id="1a3b9-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a3b9-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="1a3b9-137">See also</span></span>



[<span data-ttu-id="1a3b9-138">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="1a3b9-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="1a3b9-139">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="1a3b9-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="1a3b9-140">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="1a3b9-140">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

