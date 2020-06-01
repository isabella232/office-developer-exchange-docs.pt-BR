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
description: O elemento UploadItems representa uma solicitação para carregar itens em uma caixa de correio.
ms.openlocfilehash: 8fdb7253926e030085374b650e792349e598ee4a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468821"
---
# <a name="uploaditems"></a><span data-ttu-id="acddd-103">UploadItems</span><span class="sxs-lookup"><span data-stu-id="acddd-103">UploadItems</span></span>

<span data-ttu-id="acddd-104">O elemento **UploadItems** representa uma solicitação para carregar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="acddd-104">The **UploadItems** element represents a request to upload items into a mailbox.</span></span> 
  
[<span data-ttu-id="acddd-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="acddd-105">UploadItems</span></span>](uploaditems.md)
  
```XML
<UploadItems>
   <Items/>
</UploadItems>
```

 <span data-ttu-id="acddd-106">**UploadItemsType**</span><span class="sxs-lookup"><span data-stu-id="acddd-106">**UploadItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="acddd-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="acddd-107">Attributes and elements</span></span>

<span data-ttu-id="acddd-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="acddd-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="acddd-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="acddd-109">Attributes</span></span>

<span data-ttu-id="acddd-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="acddd-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="acddd-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="acddd-111">Child elements</span></span>

|<span data-ttu-id="acddd-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="acddd-112">**Element**</span></span>|<span data-ttu-id="acddd-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="acddd-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="acddd-114">Itens (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="acddd-114">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md) <br/> |<span data-ttu-id="acddd-115">Contém uma matriz de itens para carregar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="acddd-115">Contains an array of items to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="acddd-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="acddd-116">Parent elements</span></span>

<span data-ttu-id="acddd-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="acddd-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="acddd-118">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="acddd-118">Text value</span></span>

<span data-ttu-id="acddd-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="acddd-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="acddd-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="acddd-120">Remarks</span></span>

<span data-ttu-id="acddd-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="acddd-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="acddd-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="acddd-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="acddd-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="acddd-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="acddd-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="acddd-124">Schema Name</span></span>  <br/> |<span data-ttu-id="acddd-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="acddd-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="acddd-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="acddd-126">Validation File</span></span>  <br/> |<span data-ttu-id="acddd-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="acddd-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="acddd-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="acddd-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="acddd-129">False</span><span class="sxs-lookup"><span data-stu-id="acddd-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="acddd-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="acddd-130">See also</span></span>



[<span data-ttu-id="acddd-131">Operação ExportItems</span><span class="sxs-lookup"><span data-stu-id="acddd-131">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="acddd-132">Operação UploadItems</span><span class="sxs-lookup"><span data-stu-id="acddd-132">UploadItems operation</span></span>](uploaditems-operation.md)

