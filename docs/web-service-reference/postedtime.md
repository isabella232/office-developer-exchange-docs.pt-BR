---
title: Postadotime
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
description: O elemento Postadotime representa a hora em que um PostItem foi lançado. Este elemento é somente leitura. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 5fc670bfee97a46700bc4442d489696a4489f88a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459192"
---
# <a name="postedtime"></a><span data-ttu-id="e7373-105">Postadotime</span><span class="sxs-lookup"><span data-stu-id="e7373-105">PostedTime</span></span>

<span data-ttu-id="e7373-106">O elemento **postadotime** representa a hora em que um [PostItem](postitem.md) foi lançado.</span><span class="sxs-lookup"><span data-stu-id="e7373-106">The **PostedTime** element represents the time at which a [PostItem](postitem.md) was posted.</span></span> <span data-ttu-id="e7373-107">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7373-107">This element is read-only.</span></span> <span data-ttu-id="e7373-108">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e7373-108">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PostedTime/>
```

 <span data-ttu-id="e7373-109">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="e7373-109">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7373-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e7373-110">Attributes and elements</span></span>

<span data-ttu-id="e7373-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e7373-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7373-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="e7373-112">Attributes</span></span>

<span data-ttu-id="e7373-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e7373-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7373-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e7373-114">Child elements</span></span>

<span data-ttu-id="e7373-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e7373-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e7373-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e7373-116">Parent elements</span></span>

|<span data-ttu-id="e7373-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e7373-117">**Element**</span></span>|<span data-ttu-id="e7373-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e7373-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7373-119">Item de postagem</span><span class="sxs-lookup"><span data-stu-id="e7373-119">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="e7373-120">Representa um PostItem no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7373-120">Represents a PostItem in the Exchange store.</span></span> <span data-ttu-id="e7373-121">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="e7373-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e7373-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e7373-122">Text value</span></span>

<span data-ttu-id="e7373-123">O valor de texto é um dateTime que representa quando um **PostItem** foi lançado.</span><span class="sxs-lookup"><span data-stu-id="e7373-123">The text value is a dateTime that represents when a **PostItem** was posted.</span></span> <span data-ttu-id="e7373-124">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7373-124">This property is read-only.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e7373-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="e7373-125">Remarks</span></span>

<span data-ttu-id="e7373-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="e7373-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7373-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e7373-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7373-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="e7373-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e7373-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e7373-129">Schema Name</span></span>  <br/> |<span data-ttu-id="e7373-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e7373-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="e7373-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e7373-131">Validation File</span></span>  <br/> |<span data-ttu-id="e7373-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e7373-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e7373-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e7373-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="e7373-134">False</span><span class="sxs-lookup"><span data-stu-id="e7373-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e7373-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="e7373-135">See also</span></span>



- [<span data-ttu-id="e7373-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e7373-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

