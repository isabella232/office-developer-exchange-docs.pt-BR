---
title: ConversationLastSyncTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationLastSyncTime
api_type:
- schema
ms.assetid: 90f8f9e3-5fc6-4a6a-bdfb-fc91fa51f8a2
description: O elemento ConversationLastSyncTime contém a data e hora da última sincronização uma conversa. Este elemento deve estar presente durante a tentativa de excluir todos os itens em uma conversa que foram recebidos do período especificado.
ms.openlocfilehash: 3b086d69ac0ef307059df4902e65f796c63733d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751529"
---
# <a name="conversationlastsynctime"></a><span data-ttu-id="47f00-104">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="47f00-104">ConversationLastSyncTime</span></span>

<span data-ttu-id="47f00-105">O elemento **ConversationLastSyncTime** contém a data e hora da última sincronização uma conversa.</span><span class="sxs-lookup"><span data-stu-id="47f00-105">The **ConversationLastSyncTime** element contains the date and time that a conversation was last synchronized.</span></span> <span data-ttu-id="47f00-106">Este elemento deve estar presente durante a tentativa de excluir todos os itens em uma conversa que foram recebidos do período especificado.</span><span class="sxs-lookup"><span data-stu-id="47f00-106">This element must be present when trying to delete all items in a conversation that were received up to the specified time.</span></span> 
  
[<span data-ttu-id="47f00-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="47f00-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="47f00-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="47f00-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="47f00-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="47f00-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="47f00-110">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="47f00-110">ConversationLastSyncTime</span></span>](conversationlastsynctime.md)
  
```XML
<ConversationLastSyncTime/>
```

 <span data-ttu-id="47f00-111">**xs**</span><span class="sxs-lookup"><span data-stu-id="47f00-111">**xs:dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47f00-112">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="47f00-112">Attributes and elements</span></span>

<span data-ttu-id="47f00-113">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="47f00-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47f00-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="47f00-114">Attributes</span></span>

<span data-ttu-id="47f00-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="47f00-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47f00-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="47f00-116">Child elements</span></span>

<span data-ttu-id="47f00-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="47f00-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="47f00-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="47f00-118">Parent elements</span></span>

|<span data-ttu-id="47f00-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="47f00-119">**Element**</span></span>|<span data-ttu-id="47f00-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47f00-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47f00-121">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="47f00-121">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="47f00-122">Contém uma única ação a ser aplicado a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="47f00-122">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="47f00-123">Text value</span><span class="sxs-lookup"><span data-stu-id="47f00-123">Text value</span></span>

<span data-ttu-id="47f00-124">O valor de texto do **ConversationLastSyncTime** indica a última vez em que a conversa foi sincronizada.</span><span class="sxs-lookup"><span data-stu-id="47f00-124">The text value of the **ConversationLastSyncTime** indicates the last time the conversation was synchronized.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="47f00-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="47f00-125">Remarks</span></span>

<span data-ttu-id="47f00-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="47f00-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="47f00-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="47f00-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47f00-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="47f00-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="47f00-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="47f00-129">Schema Name</span></span>  <br/> |<span data-ttu-id="47f00-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="47f00-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="47f00-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="47f00-131">Validation File</span></span>  <br/> |<span data-ttu-id="47f00-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="47f00-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="47f00-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="47f00-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="47f00-134">False</span><span class="sxs-lookup"><span data-stu-id="47f00-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47f00-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="47f00-135">See also</span></span>



[<span data-ttu-id="47f00-136">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="47f00-136">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="47f00-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="47f00-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

