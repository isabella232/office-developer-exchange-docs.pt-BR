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
description: O elemento EnableAlwaysDelete Especifica um sinalizador que permite a exclusão de todos os novos itens em uma conversa.
ms.openlocfilehash: f86765c641604afbf13ac962f4b34fbd8de56200
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752046"
---
# <a name="enablealwaysdelete"></a><span data-ttu-id="bcc34-103">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="bcc34-103">EnableAlwaysDelete</span></span>

<span data-ttu-id="bcc34-104">O elemento **EnableAlwaysDelete** Especifica um sinalizador que permite a exclusão de todos os novos itens em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="bcc34-104">The **EnableAlwaysDelete** element specifies a flag that enables deletion for all new items in a conversation.</span></span> 
  
[<span data-ttu-id="bcc34-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="bcc34-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="bcc34-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="bcc34-106">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="bcc34-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="bcc34-107">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="bcc34-108">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="bcc34-108">EnableAlwaysDelete</span></span>](enablealwaysdelete.md)
  
```XML
<EnableAlwaysDelete/>
```

 <span data-ttu-id="bcc34-109">**xs:Boolean**</span><span class="sxs-lookup"><span data-stu-id="bcc34-109">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bcc34-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="bcc34-110">Attributes and elements</span></span>

<span data-ttu-id="bcc34-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bcc34-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bcc34-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="bcc34-112">Attributes</span></span>

<span data-ttu-id="bcc34-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bcc34-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bcc34-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bcc34-114">Child elements</span></span>

<span data-ttu-id="bcc34-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bcc34-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bcc34-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bcc34-116">Parent elements</span></span>

|<span data-ttu-id="bcc34-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bcc34-117">**Element**</span></span>|<span data-ttu-id="bcc34-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bcc34-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bcc34-119">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="bcc34-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="bcc34-120">Contém uma única ação a ser aplicado a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="bcc34-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bcc34-121">Text value</span><span class="sxs-lookup"><span data-stu-id="bcc34-121">Text value</span></span>

<span data-ttu-id="bcc34-122">O valor de texto do elemento **EnableAlwaysDelete** é **true** para habilitar a exclusão de todos os itens na conversa; Caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="bcc34-122">The text value of the **EnableAlwaysDelete** element is **true** to enable the deletion of all items in conversation; otherwise, **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bcc34-123">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="bcc34-123">Remarks</span></span>

<span data-ttu-id="bcc34-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="bcc34-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bcc34-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="bcc34-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bcc34-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="bcc34-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bcc34-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bcc34-127">Schema Name</span></span>  <br/> |<span data-ttu-id="bcc34-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="bcc34-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="bcc34-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bcc34-129">Validation File</span></span>  <br/> |<span data-ttu-id="bcc34-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bcc34-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bcc34-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="bcc34-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="bcc34-132">False</span><span class="sxs-lookup"><span data-stu-id="bcc34-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bcc34-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="bcc34-133">See also</span></span>



[<span data-ttu-id="bcc34-134">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="bcc34-134">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

