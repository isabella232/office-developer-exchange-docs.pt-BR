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
description: O elemento CopyItem define uma solicitação para copiar um item em uma caixa de correio no repositório do Exchange.
ms.openlocfilehash: b9af1670fd580107de08ad3b950191399436388d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458499"
---
# <a name="copyitem"></a><span data-ttu-id="3c5b7-103">CopyItem</span><span class="sxs-lookup"><span data-stu-id="3c5b7-103">CopyItem</span></span>

<span data-ttu-id="3c5b7-104">O elemento **CopyItem** define uma solicitação para copiar um item em uma caixa de correio no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c5b7-104">The **CopyItem** element defines a request to copy an item in a mailbox in the Exchange store.</span></span> 
  
```XML
<CopyItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</CopyItem>
```

 <span data-ttu-id="3c5b7-105">**CopyItemType**</span><span class="sxs-lookup"><span data-stu-id="3c5b7-105">**CopyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c5b7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3c5b7-106">Attributes and elements</span></span>

<span data-ttu-id="3c5b7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3c5b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c5b7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3c5b7-108">Attributes</span></span>

<span data-ttu-id="3c5b7-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c5b7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c5b7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3c5b7-110">Child elements</span></span>

|<span data-ttu-id="3c5b7-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3c5b7-111">**Element**</span></span>|<span data-ttu-id="3c5b7-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3c5b7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c5b7-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="3c5b7-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="3c5b7-114">Representa a pasta de destino de um item copiado.</span><span class="sxs-lookup"><span data-stu-id="3c5b7-114">Represents the destination folder for a copied item.</span></span>  <br/> |
|[<span data-ttu-id="3c5b7-115">ItemIds</span><span class="sxs-lookup"><span data-stu-id="3c5b7-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="3c5b7-116">Contém uma matriz de itens identificados para copiar para a pasta representada pelo elemento [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="3c5b7-116">Contains an array of identified items to copy to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="3c5b7-117">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="3c5b7-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="3c5b7-118">Indica se os identificadores de item de novos itens são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="3c5b7-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3c5b7-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3c5b7-119">Parent elements</span></span>

<span data-ttu-id="3c5b7-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c5b7-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3c5b7-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="3c5b7-121">Remarks</span></span>

<span data-ttu-id="3c5b7-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c5b7-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c5b7-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3c5b7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c5b7-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="3c5b7-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3c5b7-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3c5b7-125">Schema Name</span></span>  <br/> |<span data-ttu-id="3c5b7-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3c5b7-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3c5b7-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3c5b7-127">Validation File</span></span>  <br/> |<span data-ttu-id="3c5b7-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3c5b7-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3c5b7-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3c5b7-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="3c5b7-130">False</span><span class="sxs-lookup"><span data-stu-id="3c5b7-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c5b7-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="3c5b7-131">See also</span></span>



[<span data-ttu-id="3c5b7-132">Operação CopyItem</span><span class="sxs-lookup"><span data-stu-id="3c5b7-132">CopyItem operation</span></span>](copyitem-operation.md)


- [<span data-ttu-id="3c5b7-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3c5b7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

