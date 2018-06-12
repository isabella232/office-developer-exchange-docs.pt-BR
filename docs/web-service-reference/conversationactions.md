---
title: ConversationActions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationActions
api_type:
- schema
ms.assetid: 3d6c663d-4bd9-4eec-b95a-cd683f592672
description: O elemento ConversationActions contém uma coleção de conversas e as ações a serem aplicadas a eles.
ms.openlocfilehash: 3dff7ff66f758f1cd2eb3cd7b8126294d2799fc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751525"
---
# <a name="conversationactions"></a><span data-ttu-id="7291b-103">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="7291b-103">ConversationActions</span></span>

<span data-ttu-id="7291b-104">O elemento **ConversationActions** contém uma coleção de conversas e as ações a serem aplicadas a eles.</span><span class="sxs-lookup"><span data-stu-id="7291b-104">The **ConversationActions** element contains a collection of conversations and the actions to apply to them.</span></span> 
  
[<span data-ttu-id="7291b-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="7291b-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="7291b-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="7291b-106">ConversationActions</span></span>](conversationactions.md)
  
```XML
<ConversationActions>
   <ConversationAction/>
</ConversationActions>
```

 <span data-ttu-id="7291b-107">**NonEmptyArrayOfApplyConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="7291b-107">**NonEmptyArrayOfApplyConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7291b-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7291b-108">Attributes and elements</span></span>

<span data-ttu-id="7291b-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7291b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7291b-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="7291b-110">Attributes</span></span>

<span data-ttu-id="7291b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7291b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7291b-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7291b-112">Child elements</span></span>

|<span data-ttu-id="7291b-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7291b-113">**Element**</span></span>|<span data-ttu-id="7291b-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7291b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7291b-115">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="7291b-115">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="7291b-116">Contém uma única ação a ser aplicado a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="7291b-116">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7291b-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7291b-117">Parent elements</span></span>

|<span data-ttu-id="7291b-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7291b-118">**Element**</span></span>|<span data-ttu-id="7291b-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7291b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7291b-120">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="7291b-120">ApplyConversationAction</span></span>](applyconversationaction.md) <br/> |<span data-ttu-id="7291b-121">Define uma solicitação para aplicar ações a itens em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="7291b-121">Defines a request to apply actions to items in a conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7291b-122">Text value</span><span class="sxs-lookup"><span data-stu-id="7291b-122">Text value</span></span>

<span data-ttu-id="7291b-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7291b-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7291b-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="7291b-124">Remarks</span></span>

<span data-ttu-id="7291b-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7291b-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7291b-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7291b-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7291b-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="7291b-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7291b-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7291b-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7291b-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="7291b-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7291b-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7291b-130">Validation File</span></span>  <br/> |<span data-ttu-id="7291b-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7291b-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7291b-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7291b-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7291b-133">False</span><span class="sxs-lookup"><span data-stu-id="7291b-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7291b-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="7291b-134">See also</span></span>



[<span data-ttu-id="7291b-135">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="7291b-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

