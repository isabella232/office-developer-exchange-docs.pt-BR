---
title: BlockStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 08556ee9-0923-437c-99a4-bb630f04e973
description: O elemento BlockStatus especifica o status de bloqueio de um item.
ms.openlocfilehash: e88236274bfa70216e872025c2a94231f837df1f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462273"
---
# <a name="blockstatus"></a><span data-ttu-id="c9f81-103">BlockStatus</span><span class="sxs-lookup"><span data-stu-id="c9f81-103">BlockStatus</span></span>

<span data-ttu-id="c9f81-104">O elemento **BlockStatus** especifica o status de bloqueio de um item.</span><span class="sxs-lookup"><span data-stu-id="c9f81-104">The **BlockStatus** element specifies the block status of an item.</span></span> 
  
```XML
<BlockStatus> true | false </BlockStatus
```

 <span data-ttu-id="c9f81-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c9f81-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9f81-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c9f81-106">Attributes and elements</span></span>

<span data-ttu-id="c9f81-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c9f81-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9f81-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c9f81-108">Attributes</span></span>

<span data-ttu-id="c9f81-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9f81-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9f81-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c9f81-110">Child elements</span></span>

<span data-ttu-id="c9f81-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c9f81-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c9f81-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c9f81-112">Parent elements</span></span>

|<span data-ttu-id="c9f81-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c9f81-113">**Element**</span></span>|<span data-ttu-id="c9f81-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c9f81-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9f81-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="c9f81-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c9f81-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9f81-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c9f81-117">Contato</span><span class="sxs-lookup"><span data-stu-id="c9f81-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="c9f81-118">Representa um item de contato no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9f81-118">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9f81-119">DistributionList</span><span class="sxs-lookup"><span data-stu-id="c9f81-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="c9f81-120">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="c9f81-120">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="c9f81-121">Item</span><span class="sxs-lookup"><span data-stu-id="c9f81-121">Item</span></span>](item.md) <br/> |<span data-ttu-id="c9f81-122">Representa um item genérico no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9f81-122">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c9f81-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c9f81-123">Text value</span></span>

<span data-ttu-id="c9f81-124">Um valor de texto **true** para o elemento **BlockStatus** indica que um item está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="c9f81-124">A text value of **true** for the **BlockStatus** element indicates that an item is blocked.</span></span> <span data-ttu-id="c9f81-125">Um valor **false** indica que um item não está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="c9f81-125">A value of **false** indicates that an item is not blocked.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c9f81-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="c9f81-126">Remarks</span></span>

<span data-ttu-id="c9f81-127">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c9f81-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c9f81-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9f81-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9f81-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c9f81-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9f81-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="c9f81-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c9f81-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c9f81-131">Schema Name</span></span>  <br/> |<span data-ttu-id="c9f81-132">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="c9f81-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="c9f81-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c9f81-133">Validation File</span></span>  <br/> |<span data-ttu-id="c9f81-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c9f81-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c9f81-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c9f81-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c9f81-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="c9f81-136">See also</span></span>



- [<span data-ttu-id="c9f81-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c9f81-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

