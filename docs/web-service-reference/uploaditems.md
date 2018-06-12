---
title: UploadItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItems
api_type:
- schema
ms.assetid: fd2b9545-7213-4427-95ae-71a155b75971
description: O elemento UploadItems representa uma solicitação para carregar os itens em uma caixa de correio.
ms.openlocfilehash: d3cd69cdb744431daeede736c2e156c8ab92a79b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837948"
---
# <a name="uploaditems"></a><span data-ttu-id="6fa15-103">UploadItems</span><span class="sxs-lookup"><span data-stu-id="6fa15-103">UploadItems</span></span>

<span data-ttu-id="6fa15-104">O elemento **UploadItems** representa uma solicitação para carregar os itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6fa15-104">The **UploadItems** element represents a request to upload items into a mailbox.</span></span> 
  
[<span data-ttu-id="6fa15-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="6fa15-105">UploadItems</span></span>](uploaditems.md)
  
```XML
<UploadItems>
   <Items/>
</UploadItems>
```

 <span data-ttu-id="6fa15-106">**UploadItemsType**</span><span class="sxs-lookup"><span data-stu-id="6fa15-106">**UploadItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6fa15-107">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6fa15-107">Attributes and elements</span></span>

<span data-ttu-id="6fa15-108">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6fa15-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6fa15-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="6fa15-109">Attributes</span></span>

<span data-ttu-id="6fa15-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6fa15-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6fa15-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6fa15-111">Child elements</span></span>

|<span data-ttu-id="6fa15-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6fa15-112">**Element**</span></span>|<span data-ttu-id="6fa15-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6fa15-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6fa15-114">Itens (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="6fa15-114">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md) <br/> |<span data-ttu-id="6fa15-115">Contém uma matriz de itens para carregar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6fa15-115">Contains an array of items to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6fa15-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6fa15-116">Parent elements</span></span>

<span data-ttu-id="6fa15-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6fa15-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="6fa15-118">Text value</span><span class="sxs-lookup"><span data-stu-id="6fa15-118">Text value</span></span>

<span data-ttu-id="6fa15-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6fa15-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6fa15-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="6fa15-120">Remarks</span></span>

<span data-ttu-id="6fa15-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6fa15-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6fa15-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6fa15-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6fa15-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="6fa15-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6fa15-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6fa15-124">Schema Name</span></span>  <br/> |<span data-ttu-id="6fa15-125">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="6fa15-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="6fa15-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6fa15-126">Validation File</span></span>  <br/> |<span data-ttu-id="6fa15-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6fa15-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6fa15-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6fa15-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="6fa15-129">False</span><span class="sxs-lookup"><span data-stu-id="6fa15-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6fa15-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="6fa15-130">See also</span></span>



[<span data-ttu-id="6fa15-131">Operação ExportItems</span><span class="sxs-lookup"><span data-stu-id="6fa15-131">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="6fa15-132">Operação UploadItems</span><span class="sxs-lookup"><span data-stu-id="6fa15-132">UploadItems operation</span></span>](uploaditems-operation.md)

