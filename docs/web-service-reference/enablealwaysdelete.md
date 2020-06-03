---
title: EnableAlwaysDelete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EnableAlwaysDelete
api_type:
- schema
ms.assetid: 7753aec5-3f93-4aeb-a28e-8b9b42ca7f9b
description: O elemento EnableAlwaysDelete especifica um sinalizador que permite a exclusão de todos os novos itens em uma conversa.
ms.openlocfilehash: 14784d3a6ba52c76b64b81e15c0522d66d125cbf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526204"
---
# <a name="enablealwaysdelete"></a><span data-ttu-id="e0762-103">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="e0762-103">EnableAlwaysDelete</span></span>

<span data-ttu-id="e0762-104">O elemento **EnableAlwaysDelete** especifica um sinalizador que permite a exclusão de todos os novos itens em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="e0762-104">The **EnableAlwaysDelete** element specifies a flag that enables deletion for all new items in a conversation.</span></span> 
  
[<span data-ttu-id="e0762-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="e0762-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="e0762-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="e0762-106">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="e0762-107">Conversation</span><span class="sxs-lookup"><span data-stu-id="e0762-107">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="e0762-108">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="e0762-108">EnableAlwaysDelete</span></span>](enablealwaysdelete.md)
  
```XML
<EnableAlwaysDelete/>
```

 <span data-ttu-id="e0762-109">**xs: Boolean**</span><span class="sxs-lookup"><span data-stu-id="e0762-109">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e0762-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e0762-110">Attributes and elements</span></span>

<span data-ttu-id="e0762-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e0762-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e0762-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="e0762-112">Attributes</span></span>

<span data-ttu-id="e0762-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e0762-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e0762-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e0762-114">Child elements</span></span>

<span data-ttu-id="e0762-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e0762-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e0762-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e0762-116">Parent elements</span></span>

|<span data-ttu-id="e0762-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e0762-117">**Element**</span></span>|<span data-ttu-id="e0762-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e0762-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e0762-119">Conversation</span><span class="sxs-lookup"><span data-stu-id="e0762-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="e0762-120">Contém uma única ação a ser aplicada a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="e0762-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e0762-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e0762-121">Text value</span></span>

<span data-ttu-id="e0762-122">O valor de texto do elemento **EnableAlwaysDelete** é **true** para habilitar a exclusão de todos os itens em conversa; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="e0762-122">The text value of the **EnableAlwaysDelete** element is **true** to enable the deletion of all items in conversation; otherwise, **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e0762-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="e0762-123">Remarks</span></span>

<span data-ttu-id="e0762-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e0762-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e0762-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e0762-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e0762-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="e0762-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e0762-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e0762-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e0762-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e0762-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="e0762-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e0762-129">Validation File</span></span>  <br/> |<span data-ttu-id="e0762-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e0762-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e0762-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e0762-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="e0762-132">False</span><span class="sxs-lookup"><span data-stu-id="e0762-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e0762-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="e0762-133">See also</span></span>



[<span data-ttu-id="e0762-134">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="e0762-134">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

