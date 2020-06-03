---
title: StandardGroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StandardGroupBy
api_type:
- schema
ms.assetid: 04a84f71-b7eb-44dc-ac2c-ed504b52c463
description: O elemento StandardGroupBy representa os mecanismos padrão de agrupamento e agregação para uma operação FindItem agrupada.
ms.openlocfilehash: 3e135feba322979de3d66d5a45d423654ccc9100
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467554"
---
# <a name="standardgroupby"></a><span data-ttu-id="eb737-103">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="eb737-103">StandardGroupBy</span></span>

<span data-ttu-id="eb737-104">O elemento **StandardGroupBy** representa os mecanismos padrão de agrupamento e agregação para uma operação FindItem agrupada.</span><span class="sxs-lookup"><span data-stu-id="eb737-104">The **StandardGroupBy** element represents the standard grouping and aggregating mechanisms for a grouped FindItem operation.</span></span> 
  
[<span data-ttu-id="eb737-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="eb737-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="eb737-106">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="eb737-106">DistinguishedGroupBy</span></span>](distinguishedgroupby.md)
  
[<span data-ttu-id="eb737-107">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="eb737-107">StandardGroupBy</span></span>](standardgroupby.md)
  
```xml
<StandardGroupBy/>
```

 <span data-ttu-id="eb737-108">**StandardGroupByType**</span><span class="sxs-lookup"><span data-stu-id="eb737-108">**StandardGroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb737-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="eb737-109">Attributes and elements</span></span>

<span data-ttu-id="eb737-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="eb737-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb737-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="eb737-111">Attributes</span></span>

<span data-ttu-id="eb737-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb737-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb737-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="eb737-113">Child elements</span></span>

<span data-ttu-id="eb737-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="eb737-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eb737-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="eb737-115">Parent elements</span></span>

|<span data-ttu-id="eb737-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eb737-116">**Element**</span></span>|<span data-ttu-id="eb737-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eb737-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb737-118">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="eb737-118">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="eb737-119">Fornece agrupamentos padrão para consultas do FindItem.</span><span class="sxs-lookup"><span data-stu-id="eb737-119">Provides standard groupings for FindItem queries.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eb737-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="eb737-120">Text value</span></span>

<span data-ttu-id="eb737-121">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb737-121">A text value is required.</span></span> <span data-ttu-id="eb737-122">O único valor que pode ser usado para esse elemento é **ConversationTopic**.</span><span class="sxs-lookup"><span data-stu-id="eb737-122">The only value that can be used for this element is **ConversationTopic**.</span></span> <span data-ttu-id="eb737-123">**ConversationTopic** grupos por mensagem: ConversationTopic e agregados no item: DateTimeReceived (máximo).</span><span class="sxs-lookup"><span data-stu-id="eb737-123">**ConversationTopic** groups by message:ConversationTopic and aggregates on item:DateTimeReceived (maximum).</span></span> <span data-ttu-id="eb737-124">Para obter mais informações sobre agregação, confira [Aggregate](aggregateon.md).</span><span class="sxs-lookup"><span data-stu-id="eb737-124">For more information about aggregation, see [AggregateOn](aggregateon.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="eb737-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="eb737-125">Remarks</span></span>

<span data-ttu-id="eb737-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="eb737-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb737-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="eb737-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb737-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="eb737-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eb737-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="eb737-129">Schema Name</span></span>  <br/> |<span data-ttu-id="eb737-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="eb737-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="eb737-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="eb737-131">Validation File</span></span>  <br/> |<span data-ttu-id="eb737-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="eb737-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eb737-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="eb737-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="eb737-134">False</span><span class="sxs-lookup"><span data-stu-id="eb737-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eb737-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="eb737-135">See also</span></span>



[<span data-ttu-id="eb737-136">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="eb737-136">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="eb737-137">FindItem</span><span class="sxs-lookup"><span data-stu-id="eb737-137">FindItem</span></span>](finditem.md)


[<span data-ttu-id="eb737-138">Localizar itens</span><span class="sxs-lookup"><span data-stu-id="eb737-138">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

