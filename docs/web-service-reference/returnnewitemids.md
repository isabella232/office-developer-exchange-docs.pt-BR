---
title: ReturnNewItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: aeef79e4-31e1-4213-b627-9bac676be018
description: O elemento ReturnNewItemIds indica se os identificadores de item de novos itens são retornados na resposta.
ms.openlocfilehash: 6d3bc83c05a82d6e448041167676f41c2620dcd4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825232"
---
# <a name="returnnewitemids"></a><span data-ttu-id="394f3-103">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="394f3-103">ReturnNewItemIds</span></span>

<span data-ttu-id="394f3-104">O elemento **ReturnNewItemIds** indica se os identificadores de item de novos itens são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="394f3-104">The **ReturnNewItemIds** element indicates whether the item identifiers of new items are returned in the response.</span></span> 
  
```XML
<ReturnNewItemIds/>
```

 <span data-ttu-id="394f3-105">**xs:Boolean**</span><span class="sxs-lookup"><span data-stu-id="394f3-105">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="394f3-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="394f3-106">Attributes and elements</span></span>

<span data-ttu-id="394f3-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="394f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="394f3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="394f3-108">Attributes</span></span>

<span data-ttu-id="394f3-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="394f3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="394f3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="394f3-110">Child elements</span></span>

<span data-ttu-id="394f3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="394f3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="394f3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="394f3-112">Parent elements</span></span>

|<span data-ttu-id="394f3-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="394f3-113">**Element**</span></span>|<span data-ttu-id="394f3-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="394f3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="394f3-115">CopyItem</span><span class="sxs-lookup"><span data-stu-id="394f3-115">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="394f3-116">Define uma solicitação para copiar um item em uma caixa de correio no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="394f3-116">Defines a request to copy an item in a mailbox in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="394f3-117">MoveItem</span><span class="sxs-lookup"><span data-stu-id="394f3-117">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="394f3-118">Define uma solicitação para mover um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="394f3-118">Defines a request to move an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="394f3-119">Text value</span><span class="sxs-lookup"><span data-stu-id="394f3-119">Text value</span></span>

<span data-ttu-id="394f3-120">Um valor de texto de **true** para o elemento **ReturnNewItemIds** indica se os identificadores de item novo são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="394f3-120">A text value of **true** for the **ReturnNewItemIds** element indicates that the new item identifiers are returned in the response.</span></span> <span data-ttu-id="394f3-121">Um valor **false** indica se os identificadores de item novo não são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="394f3-121">A value of **false** indicates that the new item identifiers are not returned in the response.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="394f3-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="394f3-122">Remarks</span></span>

<span data-ttu-id="394f3-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="394f3-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="394f3-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="394f3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="394f3-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="394f3-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="394f3-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="394f3-126">Schema Name</span></span>  <br/> |<span data-ttu-id="394f3-127">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="394f3-127">Message schema</span></span>  <br/> |
|<span data-ttu-id="394f3-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="394f3-128">Validation File</span></span>  <br/> |<span data-ttu-id="394f3-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="394f3-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="394f3-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="394f3-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="394f3-131">False</span><span class="sxs-lookup"><span data-stu-id="394f3-131">False</span></span>  <br/> |
   

