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
description: O elemento ConversationActions contém uma coleção de conversas e as ações a serem aplicadas a elas.
ms.openlocfilehash: 2db84f78b4b8c92e0a6ef7d69fba7c778fb5f96d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527100"
---
# <a name="conversationactions"></a><span data-ttu-id="f6200-103">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="f6200-103">ConversationActions</span></span>

<span data-ttu-id="f6200-104">O elemento **ConversationActions** contém uma coleção de conversas e as ações a serem aplicadas a elas.</span><span class="sxs-lookup"><span data-stu-id="f6200-104">The **ConversationActions** element contains a collection of conversations and the actions to apply to them.</span></span> 
  
[<span data-ttu-id="f6200-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f6200-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="f6200-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="f6200-106">ConversationActions</span></span>](conversationactions.md)
  
```XML
<ConversationActions>
   <ConversationAction/>
</ConversationActions>
```

 <span data-ttu-id="f6200-107">**NonEmptyArrayOfApplyConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="f6200-107">**NonEmptyArrayOfApplyConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6200-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f6200-108">Attributes and elements</span></span>

<span data-ttu-id="f6200-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f6200-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6200-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="f6200-110">Attributes</span></span>

<span data-ttu-id="f6200-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f6200-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6200-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f6200-112">Child elements</span></span>

|<span data-ttu-id="f6200-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f6200-113">**Element**</span></span>|<span data-ttu-id="f6200-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f6200-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6200-115">Conversation</span><span class="sxs-lookup"><span data-stu-id="f6200-115">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="f6200-116">Contém uma única ação a ser aplicada a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="f6200-116">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f6200-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f6200-117">Parent elements</span></span>

|<span data-ttu-id="f6200-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f6200-118">**Element**</span></span>|<span data-ttu-id="f6200-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f6200-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6200-120">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f6200-120">ApplyConversationAction</span></span>](applyconversationaction.md) <br/> |<span data-ttu-id="f6200-121">Define uma solicitação para aplicar ações a itens em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="f6200-121">Defines a request to apply actions to items in a conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f6200-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f6200-122">Text value</span></span>

<span data-ttu-id="f6200-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f6200-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f6200-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="f6200-124">Remarks</span></span>

<span data-ttu-id="f6200-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f6200-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6200-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f6200-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6200-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="f6200-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f6200-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f6200-128">Schema Name</span></span>  <br/> |<span data-ttu-id="f6200-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f6200-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f6200-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f6200-130">Validation File</span></span>  <br/> |<span data-ttu-id="f6200-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f6200-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f6200-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f6200-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6200-133">False</span><span class="sxs-lookup"><span data-stu-id="f6200-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6200-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="f6200-134">See also</span></span>



[<span data-ttu-id="f6200-135">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f6200-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

