---
title: GlobalImportance
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalImportance
api_type:
- schema
ms.assetid: 8bcec699-e771-4f38-b7d9-61f324af1b4e
description: O elemento GlobalImportance contém a importância agregada para todos os itens de conversa em uma caixa de correio.
ms.openlocfilehash: c760168afa3edac20ca0ae7bc677610d8456d178
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459444"
---
# <a name="globalimportance"></a><span data-ttu-id="02b0b-103">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="02b0b-103">GlobalImportance</span></span>

<span data-ttu-id="02b0b-104">O elemento **GlobalImportance** contém a importância agregada para todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="02b0b-104">The **GlobalImportance** element contains the aggregated importance for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="02b0b-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="02b0b-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="02b0b-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="02b0b-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="02b0b-107">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="02b0b-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="02b0b-108">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="02b0b-108">GlobalImportance</span></span>](globalimportance.md)
  
```XML
<GlobalImportance> Low | Normal | High </GlobalImportance>
```

 <span data-ttu-id="02b0b-109">**ImportanceChoicesType**</span><span class="sxs-lookup"><span data-stu-id="02b0b-109">**ImportanceChoicesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02b0b-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="02b0b-110">Attributes and elements</span></span>

<span data-ttu-id="02b0b-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="02b0b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02b0b-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="02b0b-112">Attributes</span></span>

<span data-ttu-id="02b0b-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="02b0b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02b0b-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="02b0b-114">Child elements</span></span>

<span data-ttu-id="02b0b-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="02b0b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="02b0b-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="02b0b-116">Parent elements</span></span>

|<span data-ttu-id="02b0b-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="02b0b-117">**Element**</span></span>|<span data-ttu-id="02b0b-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="02b0b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02b0b-119">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="02b0b-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="02b0b-120">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="02b0b-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="02b0b-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="02b0b-121">Text value</span></span>

<span data-ttu-id="02b0b-122">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02b0b-122">A text value is required.</span></span> <span data-ttu-id="02b0b-123">Estes são os valores possíveis para este elemento:</span><span class="sxs-lookup"><span data-stu-id="02b0b-123">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="02b0b-124">Baixo</span><span class="sxs-lookup"><span data-stu-id="02b0b-124">Low</span></span>
    
- <span data-ttu-id="02b0b-125">Normal</span><span class="sxs-lookup"><span data-stu-id="02b0b-125">Normal</span></span>
    
- <span data-ttu-id="02b0b-126">Alta</span><span class="sxs-lookup"><span data-stu-id="02b0b-126">High</span></span>
    
## <a name="remarks"></a><span data-ttu-id="02b0b-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="02b0b-127">Remarks</span></span>

<span data-ttu-id="02b0b-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="02b0b-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02b0b-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="02b0b-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02b0b-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="02b0b-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="02b0b-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="02b0b-131">Schema name</span></span>  <br/> |<span data-ttu-id="02b0b-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="02b0b-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="02b0b-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="02b0b-133">Validation file</span></span>  <br/> |<span data-ttu-id="02b0b-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="02b0b-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="02b0b-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="02b0b-135">Can be empty</span></span>  <br/> |<span data-ttu-id="02b0b-136">False</span><span class="sxs-lookup"><span data-stu-id="02b0b-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="02b0b-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="02b0b-137">See also</span></span>



[<span data-ttu-id="02b0b-138">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="02b0b-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="02b0b-139">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="02b0b-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="02b0b-140">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="02b0b-140">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

