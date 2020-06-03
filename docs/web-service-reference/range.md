---
title: Intervalo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: O elemento Range especifica um intervalo de ocorrências de item de calendário para um item de calendário repetido.
ms.openlocfilehash: b5fb41709905290326b47e2662383031c34fd9c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465307"
---
# <a name="range"></a><span data-ttu-id="36af1-103">Intervalo</span><span class="sxs-lookup"><span data-stu-id="36af1-103">Range</span></span>

<span data-ttu-id="36af1-104">O elemento **Range** especifica um intervalo de ocorrências de item de calendário para um item de calendário repetido.</span><span class="sxs-lookup"><span data-stu-id="36af1-104">The **Range** element specifies a range of calendar item occurrences for a repeating calendar item.</span></span> 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 <span data-ttu-id="36af1-105">**OccurrencesRangeType**</span><span class="sxs-lookup"><span data-stu-id="36af1-105">**OccurrencesRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36af1-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="36af1-106">Attributes and elements</span></span>

<span data-ttu-id="36af1-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="36af1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36af1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="36af1-108">Attributes</span></span>

|<span data-ttu-id="36af1-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="36af1-109">**Attribute**</span></span>|<span data-ttu-id="36af1-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="36af1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="36af1-111">**Start**</span><span class="sxs-lookup"><span data-stu-id="36af1-111">**Start**</span></span> <br/> |<span data-ttu-id="36af1-112">O valor de texto do atributo de **início** é a data de início do intervalo de itens recorrentes.</span><span class="sxs-lookup"><span data-stu-id="36af1-112">The text value of the **Start** attribute is the start date of the recurring item range.</span></span> <span data-ttu-id="36af1-113">Este é um valor de **data/hora** .</span><span class="sxs-lookup"><span data-stu-id="36af1-113">This is a **dateTime** value.</span></span>  <br/> |
|<span data-ttu-id="36af1-114">**End**</span><span class="sxs-lookup"><span data-stu-id="36af1-114">**End**</span></span> <br/> |<span data-ttu-id="36af1-115">O valor de texto do atributo **final** é a data de término do intervalo de itens recorrentes.</span><span class="sxs-lookup"><span data-stu-id="36af1-115">The text value of the **End** attribute is the end date of the recurring item range.</span></span> <span data-ttu-id="36af1-116">Este é um valor de **data/hora** .</span><span class="sxs-lookup"><span data-stu-id="36af1-116">This is a **dateTime** value.</span></span>  <br/> |
|<span data-ttu-id="36af1-117">**Count**</span><span class="sxs-lookup"><span data-stu-id="36af1-117">**Count**</span></span> <br/> |<span data-ttu-id="36af1-118">O valor de texto do atributo **Count** é o número de ocorrências do item recorrente.</span><span class="sxs-lookup"><span data-stu-id="36af1-118">The text value of the **Count** attribute is the number of occurrences of the recurring item.</span></span> <span data-ttu-id="36af1-119">Este é um valor **inteiro** .</span><span class="sxs-lookup"><span data-stu-id="36af1-119">This is an **integer** value.</span></span>  <br/> |
|<span data-ttu-id="36af1-120">**CompareOriginalStartTime**</span><span class="sxs-lookup"><span data-stu-id="36af1-120">**CompareOriginalStartTime**</span></span> <br/> |<span data-ttu-id="36af1-121">O valor de texto **true** para o atributo **CompareOriginalStartTime** indica que o cliente deve comparar a hora de início original com a nova hora de início.</span><span class="sxs-lookup"><span data-stu-id="36af1-121">The text value of **true** for the **CompareOriginalStartTime** attribute indicates that the client should compare the original start time with the new start time.</span></span> <span data-ttu-id="36af1-122">Um valor **false** indica que o cliente não precisa comparar a hora de início original com a nova hora de início.</span><span class="sxs-lookup"><span data-stu-id="36af1-122">A value of **false** indicates that the client does not need to compare the original start time with the new start time.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="36af1-123">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="36af1-123">Child elements</span></span>

<span data-ttu-id="36af1-124">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="36af1-124">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="36af1-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="36af1-125">Parent elements</span></span>

[<span data-ttu-id="36af1-126">Ranges</span><span class="sxs-lookup"><span data-stu-id="36af1-126">Ranges</span></span>](ranges.md)
  
## <a name="remarks"></a><span data-ttu-id="36af1-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="36af1-127">Remarks</span></span>

<span data-ttu-id="36af1-128">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="36af1-128">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="36af1-129">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="36af1-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36af1-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="36af1-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36af1-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="36af1-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36af1-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="36af1-132">Schema name</span></span>  <br/> |<span data-ttu-id="36af1-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="36af1-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="36af1-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="36af1-134">Validation file</span></span>  <br/> |<span data-ttu-id="36af1-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="36af1-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36af1-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="36af1-136">Can be empty</span></span>  <br/> ||
   

