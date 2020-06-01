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
description: O elemento ConversationLastSyncTime contém a data e hora em que uma conversa foi sincronizada pela última vez. Esse elemento deve estar presente ao tentar excluir todos os itens em uma conversa que foram recebidos até o momento especificado.
ms.openlocfilehash: f7cc6e205ab9936685d7b8c1f34129b799a53021
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461426"
---
# <a name="conversationlastsynctime"></a><span data-ttu-id="3768a-104">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="3768a-104">ConversationLastSyncTime</span></span>

<span data-ttu-id="3768a-105">O elemento **ConversationLastSyncTime** contém a data e hora em que uma conversa foi sincronizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3768a-105">The **ConversationLastSyncTime** element contains the date and time that a conversation was last synchronized.</span></span> <span data-ttu-id="3768a-106">Esse elemento deve estar presente ao tentar excluir todos os itens em uma conversa que foram recebidos até o momento especificado.</span><span class="sxs-lookup"><span data-stu-id="3768a-106">This element must be present when trying to delete all items in a conversation that were received up to the specified time.</span></span> 
  
[<span data-ttu-id="3768a-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="3768a-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="3768a-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="3768a-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="3768a-109">Conversation</span><span class="sxs-lookup"><span data-stu-id="3768a-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="3768a-110">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="3768a-110">ConversationLastSyncTime</span></span>](conversationlastsynctime.md)
  
```XML
<ConversationLastSyncTime/>
```

 <span data-ttu-id="3768a-111">**xs: dateTime**</span><span class="sxs-lookup"><span data-stu-id="3768a-111">**xs:dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3768a-112">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3768a-112">Attributes and elements</span></span>

<span data-ttu-id="3768a-113">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3768a-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3768a-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="3768a-114">Attributes</span></span>

<span data-ttu-id="3768a-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3768a-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3768a-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3768a-116">Child elements</span></span>

<span data-ttu-id="3768a-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3768a-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3768a-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3768a-118">Parent elements</span></span>

|<span data-ttu-id="3768a-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3768a-119">**Element**</span></span>|<span data-ttu-id="3768a-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3768a-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3768a-121">Conversation</span><span class="sxs-lookup"><span data-stu-id="3768a-121">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="3768a-122">Contém uma única ação a ser aplicada a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="3768a-122">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3768a-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3768a-123">Text value</span></span>

<span data-ttu-id="3768a-124">O valor de texto do **ConversationLastSyncTime** indica a última vez em que a conversa foi sincronizada.</span><span class="sxs-lookup"><span data-stu-id="3768a-124">The text value of the **ConversationLastSyncTime** indicates the last time the conversation was synchronized.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3768a-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="3768a-125">Remarks</span></span>

<span data-ttu-id="3768a-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3768a-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3768a-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3768a-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3768a-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="3768a-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3768a-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3768a-129">Schema Name</span></span>  <br/> |<span data-ttu-id="3768a-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3768a-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="3768a-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3768a-131">Validation File</span></span>  <br/> |<span data-ttu-id="3768a-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3768a-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3768a-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3768a-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="3768a-134">False</span><span class="sxs-lookup"><span data-stu-id="3768a-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3768a-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="3768a-135">See also</span></span>



[<span data-ttu-id="3768a-136">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="3768a-136">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="3768a-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3768a-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

