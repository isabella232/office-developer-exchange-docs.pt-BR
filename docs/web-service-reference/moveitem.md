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
description: O elemento MoveItem define uma solicitação para mover um item no repositório do Exchange.
ms.openlocfilehash: 61dbb91cc20a71f50999241b3daa21bf8ebfbcc8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530398"
---
# <a name="moveitem"></a><span data-ttu-id="e30a8-103">MoveItem</span><span class="sxs-lookup"><span data-stu-id="e30a8-103">MoveItem</span></span>

<span data-ttu-id="e30a8-104">O elemento **MoveItem** define uma solicitação para mover um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e30a8-104">The **MoveItem** element defines a request to move an item in the Exchange store.</span></span> 
  
```XML
<MoveItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</MoveItem>
```

 <span data-ttu-id="e30a8-105">**MoveItemType**</span><span class="sxs-lookup"><span data-stu-id="e30a8-105">**MoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e30a8-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e30a8-106">Attributes and elements</span></span>

<span data-ttu-id="e30a8-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e30a8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e30a8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e30a8-108">Attributes</span></span>

<span data-ttu-id="e30a8-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e30a8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e30a8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e30a8-110">Child elements</span></span>

|<span data-ttu-id="e30a8-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e30a8-111">**Element**</span></span>|<span data-ttu-id="e30a8-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e30a8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e30a8-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="e30a8-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="e30a8-114">Representa a pasta de destino de um item movido.</span><span class="sxs-lookup"><span data-stu-id="e30a8-114">Represents the destination folder for a moved item.</span></span>  <br/> |
|[<span data-ttu-id="e30a8-115">ItemIds</span><span class="sxs-lookup"><span data-stu-id="e30a8-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="e30a8-116">Contém uma matriz de itens identificados para mover para a pasta representada pelo elemento [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="e30a8-116">Contains an array of identified items to move to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="e30a8-117">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="e30a8-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="e30a8-118">Indica se os identificadores de item de novos itens são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="e30a8-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e30a8-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e30a8-119">Parent elements</span></span>

<span data-ttu-id="e30a8-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e30a8-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="e30a8-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e30a8-121">Text value</span></span>

<span data-ttu-id="e30a8-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e30a8-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e30a8-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="e30a8-123">Remarks</span></span>

<span data-ttu-id="e30a8-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e30a8-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e30a8-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e30a8-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e30a8-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="e30a8-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e30a8-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e30a8-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e30a8-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e30a8-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e30a8-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e30a8-129">Validation File</span></span>  <br/> |<span data-ttu-id="e30a8-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e30a8-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e30a8-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e30a8-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="e30a8-132">False</span><span class="sxs-lookup"><span data-stu-id="e30a8-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e30a8-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="e30a8-133">See also</span></span>



[<span data-ttu-id="e30a8-134">Operação MoveItem</span><span class="sxs-lookup"><span data-stu-id="e30a8-134">MoveItem operation</span></span>](moveitem-operation.md)


- [<span data-ttu-id="e30a8-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e30a8-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

