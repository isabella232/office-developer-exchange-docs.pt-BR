---
title: PostedTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostedTime
api_type:
- schema
ms.assetid: e8b3813c-fc7e-4674-a4c6-6818c13d2bcf
description: O elemento PostedTime representa a hora em que um PostItem postado. Este elemento é somente leitura. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 8280fc26c534b280d0f30f663b6cc3a3958036c5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824860"
---
# <a name="postedtime"></a><span data-ttu-id="a7a94-105">PostedTime</span><span class="sxs-lookup"><span data-stu-id="a7a94-105">PostedTime</span></span>

<span data-ttu-id="a7a94-106">O elemento **PostedTime** representa a hora em que um [PostItem](postitem.md) postado.</span><span class="sxs-lookup"><span data-stu-id="a7a94-106">The **PostedTime** element represents the time at which a [PostItem](postitem.md) was posted.</span></span> <span data-ttu-id="a7a94-107">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a7a94-107">This element is read-only.</span></span> <span data-ttu-id="a7a94-108">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a7a94-108">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PostedTime/>
```

 <span data-ttu-id="a7a94-109">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="a7a94-109">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7a94-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a7a94-110">Attributes and elements</span></span>

<span data-ttu-id="a7a94-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a7a94-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7a94-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="a7a94-112">Attributes</span></span>

<span data-ttu-id="a7a94-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a7a94-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a7a94-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a7a94-114">Child elements</span></span>

<span data-ttu-id="a7a94-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a7a94-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a7a94-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a7a94-116">Parent elements</span></span>

|<span data-ttu-id="a7a94-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a7a94-117">**Element**</span></span>|<span data-ttu-id="a7a94-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a7a94-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7a94-119">PostItem</span><span class="sxs-lookup"><span data-stu-id="a7a94-119">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="a7a94-120">Representa uma PostItem no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7a94-120">Represents a PostItem in the Exchange store.</span></span> <span data-ttu-id="a7a94-121">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="a7a94-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a7a94-122">Text value</span><span class="sxs-lookup"><span data-stu-id="a7a94-122">Text value</span></span>

<span data-ttu-id="a7a94-123">O valor de texto é uma data e hora que representa quando um **PostItem** foi lançado.</span><span class="sxs-lookup"><span data-stu-id="a7a94-123">The text value is a dateTime that represents when a **PostItem** was posted.</span></span> <span data-ttu-id="a7a94-124">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a7a94-124">This property is read-only.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a7a94-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="a7a94-125">Remarks</span></span>

<span data-ttu-id="a7a94-126">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="a7a94-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7a94-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a7a94-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7a94-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="a7a94-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a7a94-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a7a94-129">Schema Name</span></span>  <br/> |<span data-ttu-id="a7a94-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a7a94-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="a7a94-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a7a94-131">Validation File</span></span>  <br/> |<span data-ttu-id="a7a94-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a7a94-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a7a94-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a7a94-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="a7a94-134">False</span><span class="sxs-lookup"><span data-stu-id="a7a94-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7a94-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="a7a94-135">See also</span></span>



- [<span data-ttu-id="a7a94-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a7a94-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

