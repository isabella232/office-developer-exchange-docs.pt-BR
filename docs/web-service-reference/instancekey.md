---
title: InstanceKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb4dbe9b-aea0-4527-b7d6-e928066caf38
description: O elemento InstanceKey especifica uma chave de instância para um item ou uma conversa.
ms.openlocfilehash: a6b55b9021fe63be7f678f0a1bcb24e88aeba005
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459970"
---
# <a name="instancekey"></a><span data-ttu-id="454c9-103">InstanceKey</span><span class="sxs-lookup"><span data-stu-id="454c9-103">InstanceKey</span></span>

<span data-ttu-id="454c9-104">O elemento **InstanceKey** especifica uma chave de instância para um item ou uma conversa.</span><span class="sxs-lookup"><span data-stu-id="454c9-104">The **InstanceKey** element specifies an instance key for an item or conversation.</span></span> 
  
```XML
<InstanceKey></InstanceKey>
```

 <span data-ttu-id="454c9-105">**base64Binary**</span><span class="sxs-lookup"><span data-stu-id="454c9-105">**base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="454c9-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="454c9-106">Attributes and elements</span></span>

<span data-ttu-id="454c9-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="454c9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="454c9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="454c9-108">Attributes</span></span>

<span data-ttu-id="454c9-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="454c9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="454c9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="454c9-110">Child elements</span></span>

<span data-ttu-id="454c9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="454c9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="454c9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="454c9-112">Parent elements</span></span>

|<span data-ttu-id="454c9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="454c9-113">**Element**</span></span>|<span data-ttu-id="454c9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="454c9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="454c9-115">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="454c9-115">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="454c9-116">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="454c9-116">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="454c9-117">Item</span><span class="sxs-lookup"><span data-stu-id="454c9-117">Item</span></span>](item.md) <br/> |<span data-ttu-id="454c9-118">Representa um item genérico no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="454c9-118">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="454c9-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="454c9-119">Text value</span></span>

<span data-ttu-id="454c9-120">O valor de texto do elemento **InstanceKey** é a chave de instância de um item ou uma conversa.</span><span class="sxs-lookup"><span data-stu-id="454c9-120">The text value of the **InstanceKey** element is the instance key for an item or conversation.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="454c9-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="454c9-121">Remarks</span></span>

<span data-ttu-id="454c9-122">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="454c9-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="454c9-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="454c9-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="454c9-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="454c9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="454c9-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="454c9-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="454c9-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="454c9-126">Schema Name</span></span>  <br/> |<span data-ttu-id="454c9-127">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="454c9-127">Type schema</span></span>  <br/> |
|<span data-ttu-id="454c9-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="454c9-128">Validation File</span></span>  <br/> |<span data-ttu-id="454c9-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="454c9-129">types.xsd</span></span>  <br/> |
|<span data-ttu-id="454c9-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="454c9-130">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="454c9-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="454c9-131">See also</span></span>



- [<span data-ttu-id="454c9-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="454c9-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

