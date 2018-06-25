---
title: RecurringMasterItemIdRanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c9c89b5-4ce8-437b-a332-fa7ed35c8388
description: O elemento RecurringMasterItemIdRanges Especifica uma matriz de intervalos de ocorrência.
ms.openlocfilehash: 60d987f475bed5d630a1238550e4d14578ebd0d5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825016"
---
# <a name="recurringmasteritemidranges"></a><span data-ttu-id="7365f-103">RecurringMasterItemIdRanges</span><span class="sxs-lookup"><span data-stu-id="7365f-103">RecurringMasterItemIdRanges</span></span>

<span data-ttu-id="7365f-104">O elemento **RecurringMasterItemIdRanges** Especifica uma matriz de intervalos de ocorrência.</span><span class="sxs-lookup"><span data-stu-id="7365f-104">The **RecurringMasterItemIdRanges** element specifies an array of occurrence ranges.</span></span> 
  
```XML
<RecurringMasterItemIdRanges Id="" ChangeKey="">
   <Ranges/>
</RecurringMasterItemIdRanges>
```

 <span data-ttu-id="7365f-105">**RecurringMasterItemIdRangesType**</span><span class="sxs-lookup"><span data-stu-id="7365f-105">**RecurringMasterItemIdRangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7365f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7365f-106">Attributes and elements</span></span>

<span data-ttu-id="7365f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7365f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7365f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7365f-108">Attributes</span></span>

|<span data-ttu-id="7365f-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="7365f-109">**Attribute**</span></span>|<span data-ttu-id="7365f-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7365f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7365f-111">**ID de**</span><span class="sxs-lookup"><span data-stu-id="7365f-111">**Id**</span></span> <br/> |<span data-ttu-id="7365f-112">O valor de texto do atributo **Id** é o identificador exclusivo de um item mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="7365f-112">The text value of the **Id** attribute is a recurring master item's unique identifier.</span></span> <span data-ttu-id="7365f-113">Este é um valor de **cadeia de caracteres** .</span><span class="sxs-lookup"><span data-stu-id="7365f-113">This is a **string** value.</span></span>  <br/> |
|<span data-ttu-id="7365f-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="7365f-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="7365f-115">O valor de texto do atributo **ChangeKey** é alterar a chave do item mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="7365f-115">The text value of the **ChangeKey** attribute is the recurring master item's change key.</span></span> <span data-ttu-id="7365f-116">Este é um valor de **cadeia de caracteres** .</span><span class="sxs-lookup"><span data-stu-id="7365f-116">This is a **string** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7365f-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7365f-117">Child elements</span></span>

[<span data-ttu-id="7365f-118">Ranges</span><span class="sxs-lookup"><span data-stu-id="7365f-118">Ranges</span></span>](ranges.md)
  
### <a name="parent-elements"></a><span data-ttu-id="7365f-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7365f-119">Parent elements</span></span>

<span data-ttu-id="7365f-120">[ItemIds](itemids.md) | [GlobalItemIds](globalitemids.md) | [DraftItemIds](draftitemids.md) | [ContactIds](contactids.md) | [IDs de grupo](groupids.md)</span><span class="sxs-lookup"><span data-stu-id="7365f-120">[ItemIds](itemids.md) | [GlobalItemIds](globalitemids.md) | [DraftItemIds](draftitemids.md) | [ContactIds](contactids.md) | [GroupIds](groupids.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7365f-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="7365f-121">Remarks</span></span>

<span data-ttu-id="7365f-122">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7365f-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7365f-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7365f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7365f-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7365f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7365f-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="7365f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7365f-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7365f-126">Schema name</span></span>  <br/> |<span data-ttu-id="7365f-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7365f-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="7365f-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7365f-128">Validation file</span></span>  <br/> |<span data-ttu-id="7365f-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7365f-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7365f-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="7365f-130">Can be empty</span></span>  <br/> ||
   

