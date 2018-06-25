---
title: ConversationNode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b7f7acd3-ed65-441e-9976-8b4ed5f12c0b
description: O elemento ConversationNode Especifica um nó em uma conversa.
ms.openlocfilehash: c8289e5f30bfd25eb12d54e3be0c561786308dc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751531"
---
# <a name="conversationnode"></a><span data-ttu-id="f701f-103">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="f701f-103">ConversationNode</span></span>

<span data-ttu-id="f701f-104">O elemento **ConversationNode** Especifica um nó em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="f701f-104">The **ConversationNode** element specifies a node in a conversation.</span></span> 
  
```XML
<ConversationNode>
    <InternetMessageId></InternetMessageId>
    <ParentInternetMessageId></ParentInternetMessageId>
    <Items></Items>
</ConversationNode>
```

 <span data-ttu-id="f701f-105">**ConversationNodeType**</span><span class="sxs-lookup"><span data-stu-id="f701f-105">**ConversationNodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f701f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f701f-106">Attributes and elements</span></span>

<span data-ttu-id="f701f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f701f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f701f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f701f-108">Attributes</span></span>

<span data-ttu-id="f701f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f701f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f701f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f701f-110">Child elements</span></span>

|<span data-ttu-id="f701f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f701f-111">**Element**</span></span>|<span data-ttu-id="f701f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f701f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f701f-113">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="f701f-113">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="f701f-114">Representa o identificador de mensagem da Internet de um item.</span><span class="sxs-lookup"><span data-stu-id="f701f-114">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="f701f-115">ParentInternetMessageId</span><span class="sxs-lookup"><span data-stu-id="f701f-115">ParentInternetMessageId</span></span>](parentinternetmessageid.md) <br/> |<span data-ttu-id="f701f-116">Especifica o identificador da mensagem pai da Internet.</span><span class="sxs-lookup"><span data-stu-id="f701f-116">Specifies the identifier of the parent Internet message.</span></span>  <br/> |
|[<span data-ttu-id="f701f-117">ItemIds (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="f701f-117">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="f701f-118">Especifica todos os itens no nó da conversa.</span><span class="sxs-lookup"><span data-stu-id="f701f-118">Specifies all the items in the conversation node.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f701f-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f701f-119">Parent elements</span></span>

|<span data-ttu-id="f701f-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f701f-120">**Element**</span></span>|<span data-ttu-id="f701f-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f701f-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f701f-122">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="f701f-122">ConversationNodes</span></span>](conversationnodes.md) <br/> |<span data-ttu-id="f701f-123">Especifica uma coleção de nós de conversa.</span><span class="sxs-lookup"><span data-stu-id="f701f-123">Specifies a collection of conversation nodes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f701f-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="f701f-124">Remarks</span></span>

<span data-ttu-id="f701f-125">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f701f-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f701f-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f701f-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f701f-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f701f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f701f-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="f701f-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f701f-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f701f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="f701f-130">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="f701f-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="f701f-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f701f-131">Validation File</span></span>  <br/> |<span data-ttu-id="f701f-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f701f-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f701f-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f701f-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f701f-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="f701f-134">See also</span></span>



- [<span data-ttu-id="f701f-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f701f-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

