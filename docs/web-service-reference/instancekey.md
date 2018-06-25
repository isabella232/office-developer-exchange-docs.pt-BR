---
title: InstanceKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb4dbe9b-aea0-4527-b7d6-e928066caf38
description: O elemento InstanceKey Especifica uma chave de instância para um item ou conversa.
ms.openlocfilehash: a0e4f9390d5dc368388b5a20e38796c6c0157a40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823943"
---
# <a name="instancekey"></a><span data-ttu-id="3b13a-103">InstanceKey</span><span class="sxs-lookup"><span data-stu-id="3b13a-103">InstanceKey</span></span>

<span data-ttu-id="3b13a-104">O elemento **InstanceKey** Especifica uma chave de instância para um item ou conversa.</span><span class="sxs-lookup"><span data-stu-id="3b13a-104">The **InstanceKey** element specifies an instance key for an item or conversation.</span></span> 
  
```XML
<InstanceKey></InstanceKey>
```

 <span data-ttu-id="3b13a-105">**base64Binary**</span><span class="sxs-lookup"><span data-stu-id="3b13a-105">**base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b13a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3b13a-106">Attributes and elements</span></span>

<span data-ttu-id="3b13a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3b13a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b13a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3b13a-108">Attributes</span></span>

<span data-ttu-id="3b13a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3b13a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b13a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3b13a-110">Child elements</span></span>

<span data-ttu-id="3b13a-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3b13a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3b13a-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3b13a-112">Parent elements</span></span>

|<span data-ttu-id="3b13a-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3b13a-113">**Element**</span></span>|<span data-ttu-id="3b13a-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3b13a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b13a-115">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="3b13a-115">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="3b13a-116">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="3b13a-116">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="3b13a-117">1.1</span><span class="sxs-lookup"><span data-stu-id="3b13a-117">Item</span></span>](item.md) <br/> |<span data-ttu-id="3b13a-118">Representa um item genérico no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b13a-118">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3b13a-119">Text value</span><span class="sxs-lookup"><span data-stu-id="3b13a-119">Text value</span></span>

<span data-ttu-id="3b13a-120">O valor de texto do elemento **InstanceKey** é a chave de instância de um item ou conversa.</span><span class="sxs-lookup"><span data-stu-id="3b13a-120">The text value of the **InstanceKey** element is the instance key for an item or conversation.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3b13a-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="3b13a-121">Remarks</span></span>

<span data-ttu-id="3b13a-122">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3b13a-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3b13a-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b13a-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b13a-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3b13a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b13a-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="3b13a-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3b13a-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3b13a-126">Schema Name</span></span>  <br/> |<span data-ttu-id="3b13a-127">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="3b13a-127">Type schema</span></span>  <br/> |
|<span data-ttu-id="3b13a-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3b13a-128">Validation File</span></span>  <br/> |<span data-ttu-id="3b13a-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3b13a-129">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3b13a-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3b13a-130">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3b13a-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="3b13a-131">See also</span></span>



- [<span data-ttu-id="3b13a-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3b13a-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

