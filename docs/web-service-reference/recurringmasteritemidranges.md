---
title: RecurringMasterItemIdRanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c9c89b5-4ce8-437b-a332-fa7ed35c8388
description: O elemento RecurringMasterItemIdRanges especifica uma matriz de intervalos de ocorrência.
ms.openlocfilehash: 784676844c5c58c65b8cc6177843bf26d351b7d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528752"
---
# <a name="recurringmasteritemidranges"></a><span data-ttu-id="b4c44-103">RecurringMasterItemIdRanges</span><span class="sxs-lookup"><span data-stu-id="b4c44-103">RecurringMasterItemIdRanges</span></span>

<span data-ttu-id="b4c44-104">O elemento **RecurringMasterItemIdRanges** especifica uma matriz de intervalos de ocorrência.</span><span class="sxs-lookup"><span data-stu-id="b4c44-104">The **RecurringMasterItemIdRanges** element specifies an array of occurrence ranges.</span></span> 
  
```XML
<RecurringMasterItemIdRanges Id="" ChangeKey="">
   <Ranges/>
</RecurringMasterItemIdRanges>
```

 <span data-ttu-id="b4c44-105">**RecurringMasterItemIdRangesType**</span><span class="sxs-lookup"><span data-stu-id="b4c44-105">**RecurringMasterItemIdRangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b4c44-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b4c44-106">Attributes and elements</span></span>

<span data-ttu-id="b4c44-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b4c44-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b4c44-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b4c44-108">Attributes</span></span>

|<span data-ttu-id="b4c44-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="b4c44-109">**Attribute**</span></span>|<span data-ttu-id="b4c44-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b4c44-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b4c44-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="b4c44-111">**Id**</span></span> <br/> |<span data-ttu-id="b4c44-112">O valor de texto do atributo **ID** é um identificador exclusivo do item mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="b4c44-112">The text value of the **Id** attribute is a recurring master item's unique identifier.</span></span> <span data-ttu-id="b4c44-113">Este é um valor de **cadeia de caracteres** .</span><span class="sxs-lookup"><span data-stu-id="b4c44-113">This is a **string** value.</span></span>  <br/> |
|<span data-ttu-id="b4c44-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="b4c44-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="b4c44-115">O valor de texto do atributo **ChangeKey** é a chave de alteração do item mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="b4c44-115">The text value of the **ChangeKey** attribute is the recurring master item's change key.</span></span> <span data-ttu-id="b4c44-116">Este é um valor de **cadeia de caracteres** .</span><span class="sxs-lookup"><span data-stu-id="b4c44-116">This is a **string** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b4c44-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b4c44-117">Child elements</span></span>

[<span data-ttu-id="b4c44-118">Ranges</span><span class="sxs-lookup"><span data-stu-id="b4c44-118">Ranges</span></span>](ranges.md)
  
### <a name="parent-elements"></a><span data-ttu-id="b4c44-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b4c44-119">Parent elements</span></span>

<span data-ttu-id="b4c44-120">[ItemIds](itemids.md)  |  [GlobalItemIds](globalitemids.md)  |  [DraftItemIds](draftitemids.md)  |  [ContactIds](contactids.md)  |  [GroupIds](groupids.md)</span><span class="sxs-lookup"><span data-stu-id="b4c44-120">[ItemIds](itemids.md) | [GlobalItemIds](globalitemids.md) | [DraftItemIds](draftitemids.md) | [ContactIds](contactids.md) | [GroupIds](groupids.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b4c44-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="b4c44-121">Remarks</span></span>

<span data-ttu-id="b4c44-122">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b4c44-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b4c44-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b4c44-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b4c44-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b4c44-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b4c44-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="b4c44-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b4c44-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b4c44-126">Schema name</span></span>  <br/> |<span data-ttu-id="b4c44-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b4c44-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="b4c44-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b4c44-128">Validation file</span></span>  <br/> |<span data-ttu-id="b4c44-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b4c44-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b4c44-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b4c44-130">Can be empty</span></span>  <br/> ||
   

