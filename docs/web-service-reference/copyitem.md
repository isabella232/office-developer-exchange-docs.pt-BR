---
title: CopyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItem
api_type:
- schema
ms.assetid: ffb4c13e-e7ea-4e6b-87a0-509ce5371100
description: O elemento de CopyItem define uma solicitação para copiar um item em uma caixa de correio no armazenamento do Exchange.
ms.openlocfilehash: 08cc1b67f7c7d369263acfc4b3d13e8aa70d2d5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751552"
---
# <a name="copyitem"></a><span data-ttu-id="e2ed9-103">CopyItem</span><span class="sxs-lookup"><span data-stu-id="e2ed9-103">CopyItem</span></span>

<span data-ttu-id="e2ed9-104">O elemento de **CopyItem** define uma solicitação para copiar um item em uma caixa de correio no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2ed9-104">The **CopyItem** element defines a request to copy an item in a mailbox in the Exchange store.</span></span> 
  
```XML
<CopyItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</CopyItem>
```

 <span data-ttu-id="e2ed9-105">**CopyItemType**</span><span class="sxs-lookup"><span data-stu-id="e2ed9-105">**CopyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2ed9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e2ed9-106">Attributes and elements</span></span>

<span data-ttu-id="e2ed9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e2ed9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2ed9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e2ed9-108">Attributes</span></span>

<span data-ttu-id="e2ed9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e2ed9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2ed9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e2ed9-110">Child elements</span></span>

|<span data-ttu-id="e2ed9-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e2ed9-111">**Element**</span></span>|<span data-ttu-id="e2ed9-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e2ed9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2ed9-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="e2ed9-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="e2ed9-114">Representa a pasta de destino para um item copiado.</span><span class="sxs-lookup"><span data-stu-id="e2ed9-114">Represents the destination folder for a copied item.</span></span>  <br/> |
|[<span data-ttu-id="e2ed9-115">ItemIds</span><span class="sxs-lookup"><span data-stu-id="e2ed9-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="e2ed9-116">Contém uma matriz de itens identificados para copiar para a pasta representada por um elemento [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="e2ed9-116">Contains an array of identified items to copy to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="e2ed9-117">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="e2ed9-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="e2ed9-118">Indica se os identificadores de item de novos itens são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="e2ed9-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e2ed9-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e2ed9-119">Parent elements</span></span>

<span data-ttu-id="e2ed9-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e2ed9-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e2ed9-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="e2ed9-121">Remarks</span></span>

<span data-ttu-id="e2ed9-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2ed9-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2ed9-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e2ed9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2ed9-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="e2ed9-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e2ed9-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e2ed9-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e2ed9-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e2ed9-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e2ed9-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e2ed9-127">Validation File</span></span>  <br/> |<span data-ttu-id="e2ed9-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e2ed9-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e2ed9-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e2ed9-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="e2ed9-130">False</span><span class="sxs-lookup"><span data-stu-id="e2ed9-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2ed9-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="e2ed9-131">See also</span></span>



[<span data-ttu-id="e2ed9-132">Operação CopyItem</span><span class="sxs-lookup"><span data-stu-id="e2ed9-132">CopyItem operation</span></span>](copyitem-operation.md)


- [<span data-ttu-id="e2ed9-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e2ed9-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

