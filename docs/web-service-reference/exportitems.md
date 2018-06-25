---
title: ExportItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExportItems
api_type:
- schema
ms.assetid: bbbc56e4-8cc1-43ae-b70a-9a8d6bb0f399
description: O elemento ExportItems representa uma solicitação para exportar itens de uma caixa de correio.
ms.openlocfilehash: 055012166bb125dfcf86070f2e23496bf0209b51
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752145"
---
# <a name="exportitems"></a><span data-ttu-id="f2620-103">ExportItems</span><span class="sxs-lookup"><span data-stu-id="f2620-103">ExportItems</span></span>

<span data-ttu-id="f2620-104">O elemento **ExportItems** representa uma solicitação para exportar itens de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f2620-104">The **ExportItems** element represents a request to export items from a mailbox.</span></span> 
  
[<span data-ttu-id="f2620-105">ExportItems</span><span class="sxs-lookup"><span data-stu-id="f2620-105">ExportItems</span></span>](exportitems.md)
  
```XML
<ExportItems>
   <ItemIds/>
</ExportItems>
```

 <span data-ttu-id="f2620-106">**ExportItemsType**</span><span class="sxs-lookup"><span data-stu-id="f2620-106">**ExportItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2620-107">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f2620-107">Attributes and elements</span></span>

<span data-ttu-id="f2620-108">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f2620-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2620-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="f2620-109">Attributes</span></span>

<span data-ttu-id="f2620-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f2620-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2620-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f2620-111">Child elements</span></span>

|<span data-ttu-id="f2620-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f2620-112">**Element**</span></span>|<span data-ttu-id="f2620-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f2620-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2620-114">ItemIds (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="f2620-114">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="f2620-115">Contém uma matriz de identificadores de item que identificam os itens para exportar de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f2620-115">Contains an array of item identifiers that identify the items to export from a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f2620-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f2620-116">Parent elements</span></span>

<span data-ttu-id="f2620-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f2620-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f2620-118">Text value</span><span class="sxs-lookup"><span data-stu-id="f2620-118">Text value</span></span>

<span data-ttu-id="f2620-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f2620-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f2620-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="f2620-120">Remarks</span></span>

<span data-ttu-id="f2620-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f2620-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2620-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f2620-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2620-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="f2620-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f2620-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f2620-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f2620-125">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="f2620-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="f2620-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f2620-126">Validation File</span></span>  <br/> |<span data-ttu-id="f2620-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f2620-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f2620-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f2620-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2620-129">False</span><span class="sxs-lookup"><span data-stu-id="f2620-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2620-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="f2620-130">See also</span></span>



[<span data-ttu-id="f2620-131">Operação ExportItems</span><span class="sxs-lookup"><span data-stu-id="f2620-131">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="f2620-132">Operação UploadItems</span><span class="sxs-lookup"><span data-stu-id="f2620-132">UploadItems operation</span></span>](uploaditems-operation.md)

