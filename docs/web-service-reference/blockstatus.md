---
title: BlockStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 08556ee9-0923-437c-99a4-bb630f04e973
description: O elemento BlockStatus Especifica o status de bloqueio de um item.
ms.openlocfilehash: 5733738d733578c47b849b9d7c62c9b66cd8922e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751283"
---
# <a name="blockstatus"></a><span data-ttu-id="22d4f-103">BlockStatus</span><span class="sxs-lookup"><span data-stu-id="22d4f-103">BlockStatus</span></span>

<span data-ttu-id="22d4f-104">O elemento **BlockStatus** Especifica o status de bloqueio de um item.</span><span class="sxs-lookup"><span data-stu-id="22d4f-104">The **BlockStatus** element specifies the block status of an item.</span></span> 
  
```XML
<BlockStatus> true | false </BlockStatus
```

 <span data-ttu-id="22d4f-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="22d4f-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22d4f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="22d4f-106">Attributes and elements</span></span>

<span data-ttu-id="22d4f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="22d4f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22d4f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="22d4f-108">Attributes</span></span>

<span data-ttu-id="22d4f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="22d4f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22d4f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="22d4f-110">Child elements</span></span>

<span data-ttu-id="22d4f-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="22d4f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="22d4f-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="22d4f-112">Parent elements</span></span>

|<span data-ttu-id="22d4f-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="22d4f-113">**Element**</span></span>|<span data-ttu-id="22d4f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="22d4f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22d4f-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="22d4f-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="22d4f-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="22d4f-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="22d4f-117">Contato</span><span class="sxs-lookup"><span data-stu-id="22d4f-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="22d4f-118">Representa um item de contato no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="22d4f-118">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="22d4f-119">DistributionList</span><span class="sxs-lookup"><span data-stu-id="22d4f-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="22d4f-120">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="22d4f-120">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="22d4f-121">1.1</span><span class="sxs-lookup"><span data-stu-id="22d4f-121">Item</span></span>](item.md) <br/> |<span data-ttu-id="22d4f-122">Representa um item genérico no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="22d4f-122">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="22d4f-123">Text value</span><span class="sxs-lookup"><span data-stu-id="22d4f-123">Text value</span></span>

<span data-ttu-id="22d4f-124">Um valor de texto de **true** para o elemento **BlockStatus** indica que um item está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="22d4f-124">A text value of **true** for the **BlockStatus** element indicates that an item is blocked.</span></span> <span data-ttu-id="22d4f-125">Um valor **false** indica que um item não será bloqueado.</span><span class="sxs-lookup"><span data-stu-id="22d4f-125">A value of **false** indicates that an item is not blocked.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="22d4f-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="22d4f-126">Remarks</span></span>

<span data-ttu-id="22d4f-127">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="22d4f-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="22d4f-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="22d4f-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22d4f-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="22d4f-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22d4f-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="22d4f-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="22d4f-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="22d4f-131">Schema Name</span></span>  <br/> |<span data-ttu-id="22d4f-132">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="22d4f-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="22d4f-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="22d4f-133">Validation File</span></span>  <br/> |<span data-ttu-id="22d4f-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="22d4f-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="22d4f-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="22d4f-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="22d4f-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="22d4f-136">See also</span></span>



- [<span data-ttu-id="22d4f-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="22d4f-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

