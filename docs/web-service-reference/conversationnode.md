---
title: ConversationNode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b7f7acd3-ed65-441e-9976-8b4ed5f12c0b
description: O elemento ConversationNode especifica um nó em uma conversa.
ms.openlocfilehash: 074209c1b5669db8dd1ea4ba7f9dea064628afbd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462700"
---
# <a name="conversationnode"></a><span data-ttu-id="bb455-103">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="bb455-103">ConversationNode</span></span>

<span data-ttu-id="bb455-104">O elemento **ConversationNode** especifica um nó em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="bb455-104">The **ConversationNode** element specifies a node in a conversation.</span></span> 
  
```XML
<ConversationNode>
    <InternetMessageId></InternetMessageId>
    <ParentInternetMessageId></ParentInternetMessageId>
    <Items></Items>
</ConversationNode>
```

 <span data-ttu-id="bb455-105">**ConversationNodeType**</span><span class="sxs-lookup"><span data-stu-id="bb455-105">**ConversationNodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb455-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="bb455-106">Attributes and elements</span></span>

<span data-ttu-id="bb455-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bb455-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb455-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="bb455-108">Attributes</span></span>

<span data-ttu-id="bb455-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb455-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb455-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bb455-110">Child elements</span></span>

|<span data-ttu-id="bb455-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bb455-111">**Element**</span></span>|<span data-ttu-id="bb455-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bb455-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb455-113">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="bb455-113">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="bb455-114">Representa o identificador de mensagem da Internet de um item.</span><span class="sxs-lookup"><span data-stu-id="bb455-114">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="bb455-115">ParentInternetMessageId</span><span class="sxs-lookup"><span data-stu-id="bb455-115">ParentInternetMessageId</span></span>](parentinternetmessageid.md) <br/> |<span data-ttu-id="bb455-116">Especifica o identificador da mensagem de Internet pai.</span><span class="sxs-lookup"><span data-stu-id="bb455-116">Specifies the identifier of the parent Internet message.</span></span>  <br/> |
|[<span data-ttu-id="bb455-117">ItemIds (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="bb455-117">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="bb455-118">Especifica todos os itens no nó de conversa.</span><span class="sxs-lookup"><span data-stu-id="bb455-118">Specifies all the items in the conversation node.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bb455-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bb455-119">Parent elements</span></span>

|<span data-ttu-id="bb455-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bb455-120">**Element**</span></span>|<span data-ttu-id="bb455-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bb455-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb455-122">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="bb455-122">ConversationNodes</span></span>](conversationnodes.md) <br/> |<span data-ttu-id="bb455-123">Especifica uma coleção de nós de conversa.</span><span class="sxs-lookup"><span data-stu-id="bb455-123">Specifies a collection of conversation nodes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bb455-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="bb455-124">Remarks</span></span>

<span data-ttu-id="bb455-125">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bb455-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bb455-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb455-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb455-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="bb455-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb455-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="bb455-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bb455-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bb455-129">Schema Name</span></span>  <br/> |<span data-ttu-id="bb455-130">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="bb455-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="bb455-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bb455-131">Validation File</span></span>  <br/> |<span data-ttu-id="bb455-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bb455-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="bb455-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="bb455-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bb455-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="bb455-134">See also</span></span>



- [<span data-ttu-id="bb455-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bb455-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

