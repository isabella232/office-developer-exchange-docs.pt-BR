---
title: MoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItem
api_type:
- schema
ms.assetid: a4593377-22dd-415f-b01d-387389ef650f
description: O elemento de MoveItem define uma solicitação para mover um item no armazenamento do Exchange.
ms.openlocfilehash: cd7f35bdabe8a596f4c186df1c8cd54e0ea1c540
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824486"
---
# <a name="moveitem"></a><span data-ttu-id="cc0a5-103">MoveItem</span><span class="sxs-lookup"><span data-stu-id="cc0a5-103">MoveItem</span></span>

<span data-ttu-id="cc0a5-104">O elemento de **MoveItem** define uma solicitação para mover um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cc0a5-104">The **MoveItem** element defines a request to move an item in the Exchange store.</span></span> 
  
```XML
<MoveItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</MoveItem>
```

 <span data-ttu-id="cc0a5-105">**MoveItemType**</span><span class="sxs-lookup"><span data-stu-id="cc0a5-105">**MoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc0a5-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="cc0a5-106">Attributes and elements</span></span>

<span data-ttu-id="cc0a5-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cc0a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc0a5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cc0a5-108">Attributes</span></span>

<span data-ttu-id="cc0a5-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cc0a5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc0a5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cc0a5-110">Child elements</span></span>

|<span data-ttu-id="cc0a5-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cc0a5-111">**Element**</span></span>|<span data-ttu-id="cc0a5-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cc0a5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc0a5-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="cc0a5-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="cc0a5-114">Representa a pasta de destino para um item movido.</span><span class="sxs-lookup"><span data-stu-id="cc0a5-114">Represents the destination folder for a moved item.</span></span>  <br/> |
|[<span data-ttu-id="cc0a5-115">ItemIds</span><span class="sxs-lookup"><span data-stu-id="cc0a5-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="cc0a5-116">Contém uma matriz de itens identificados para mover para a pasta representada por um elemento [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="cc0a5-116">Contains an array of identified items to move to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="cc0a5-117">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="cc0a5-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="cc0a5-118">Indica se os identificadores de item de novos itens são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="cc0a5-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cc0a5-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cc0a5-119">Parent elements</span></span>

<span data-ttu-id="cc0a5-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cc0a5-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="cc0a5-121">Text value</span><span class="sxs-lookup"><span data-stu-id="cc0a5-121">Text value</span></span>

<span data-ttu-id="cc0a5-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cc0a5-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cc0a5-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="cc0a5-123">Remarks</span></span>

<span data-ttu-id="cc0a5-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cc0a5-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc0a5-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="cc0a5-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc0a5-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="cc0a5-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cc0a5-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cc0a5-127">Schema Name</span></span>  <br/> |<span data-ttu-id="cc0a5-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="cc0a5-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cc0a5-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cc0a5-129">Validation File</span></span>  <br/> |<span data-ttu-id="cc0a5-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cc0a5-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cc0a5-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cc0a5-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="cc0a5-132">False</span><span class="sxs-lookup"><span data-stu-id="cc0a5-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cc0a5-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="cc0a5-133">See also</span></span>



[<span data-ttu-id="cc0a5-134">Operação MoveItem</span><span class="sxs-lookup"><span data-stu-id="cc0a5-134">MoveItem operation</span></span>](moveitem-operation.md)


- [<span data-ttu-id="cc0a5-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cc0a5-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

