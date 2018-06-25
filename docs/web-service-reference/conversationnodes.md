---
title: ConversationNodes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c8a35b8-a940-4b3e-8768-9ba95766fd79
description: O elemento ConversationNodes Especifica uma coleção de nós de conversa.
ms.openlocfilehash: 62ec061f6d03abb9db7e511722e5570e70d65772
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751540"
---
# <a name="conversationnodes"></a><span data-ttu-id="8d0bb-103">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="8d0bb-103">ConversationNodes</span></span>

<span data-ttu-id="8d0bb-104">O elemento **ConversationNodes** Especifica uma coleção de nós de conversa.</span><span class="sxs-lookup"><span data-stu-id="8d0bb-104">The **ConversationNodes** element specifies a collection of conversation nodes.</span></span> 
  
```XML
<ConversationNodes>
    <ConversationNode></ConversationNode>
</ConversationNodes>
```

 <span data-ttu-id="8d0bb-105">**ArrayOfConversationNodesType**</span><span class="sxs-lookup"><span data-stu-id="8d0bb-105">**ArrayOfConversationNodesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8d0bb-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8d0bb-106">Attributes and elements</span></span>

<span data-ttu-id="8d0bb-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8d0bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d0bb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8d0bb-108">Attributes</span></span>

<span data-ttu-id="8d0bb-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8d0bb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d0bb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8d0bb-110">Child elements</span></span>

|<span data-ttu-id="8d0bb-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8d0bb-111">**Element**</span></span>|<span data-ttu-id="8d0bb-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8d0bb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d0bb-113">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="8d0bb-113">ConversationNode</span></span>](conversationnode.md) <br/> |<span data-ttu-id="8d0bb-114">Especifica um nó em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="8d0bb-114">Specifies a node in a conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8d0bb-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8d0bb-115">Parent elements</span></span>

|<span data-ttu-id="8d0bb-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8d0bb-116">**Element**</span></span>|<span data-ttu-id="8d0bb-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8d0bb-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d0bb-118">Conversa (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="8d0bb-118">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md) <br/> |<span data-ttu-id="8d0bb-119">Representa uma única conversa retornada em uma resposta **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="8d0bb-119">Represents a single conversation returned in a **GetConversationItems** response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8d0bb-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="8d0bb-120">Remarks</span></span>

<span data-ttu-id="8d0bb-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8d0bb-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8d0bb-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8d0bb-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d0bb-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8d0bb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d0bb-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="8d0bb-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8d0bb-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8d0bb-125">Schema Name</span></span>  <br/> |<span data-ttu-id="8d0bb-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="8d0bb-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="8d0bb-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8d0bb-127">Validation File</span></span>  <br/> |<span data-ttu-id="8d0bb-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8d0bb-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8d0bb-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="8d0bb-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8d0bb-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="8d0bb-130">See also</span></span>



- [<span data-ttu-id="8d0bb-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8d0bb-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

