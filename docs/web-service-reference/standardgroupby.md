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
description: O elemento StandardGroupBy representa o padrão de agrupamento e agregar mecanismos para uma operação de FindItem agrupada.
ms.openlocfilehash: 8e2ec72a79ebafc2e5757d6dcebb27c0c53ec0b5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825542"
---
# <a name="standardgroupby"></a><span data-ttu-id="04885-103">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="04885-103">StandardGroupBy</span></span>

<span data-ttu-id="04885-104">O elemento **StandardGroupBy** representa o padrão de agrupamento e agregar mecanismos para uma operação de FindItem agrupada.</span><span class="sxs-lookup"><span data-stu-id="04885-104">The **StandardGroupBy** element represents the standard grouping and aggregating mechanisms for a grouped FindItem operation.</span></span> 
  
[<span data-ttu-id="04885-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="04885-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="04885-106">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="04885-106">DistinguishedGroupBy</span></span>](distinguishedgroupby.md)
  
[<span data-ttu-id="04885-107">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="04885-107">StandardGroupBy</span></span>](standardgroupby.md)
  
```xml
<StandardGroupBy/>
```

 <span data-ttu-id="04885-108">**StandardGroupByType**</span><span class="sxs-lookup"><span data-stu-id="04885-108">**StandardGroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04885-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="04885-109">Attributes and elements</span></span>

<span data-ttu-id="04885-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="04885-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04885-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="04885-111">Attributes</span></span>

<span data-ttu-id="04885-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="04885-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04885-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="04885-113">Child elements</span></span>

<span data-ttu-id="04885-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="04885-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="04885-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="04885-115">Parent elements</span></span>

|<span data-ttu-id="04885-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="04885-116">**Element**</span></span>|<span data-ttu-id="04885-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="04885-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04885-118">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="04885-118">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="04885-119">Fornece agrupamentos padrão para consultas FindItem.</span><span class="sxs-lookup"><span data-stu-id="04885-119">Provides standard groupings for FindItem queries.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="04885-120">Text value</span><span class="sxs-lookup"><span data-stu-id="04885-120">Text value</span></span>

<span data-ttu-id="04885-121">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="04885-121">A text value is required.</span></span> <span data-ttu-id="04885-122">O único valor que pode ser usado para esse elemento é **ConversationTopic**.</span><span class="sxs-lookup"><span data-stu-id="04885-122">The only value that can be used for this element is **ConversationTopic**.</span></span> <span data-ttu-id="04885-123">Grupos de **ConversationTopic** por mensagem: ConversationTopic e agregados no item: DateTimeReceived (máximo).</span><span class="sxs-lookup"><span data-stu-id="04885-123">**ConversationTopic** groups by message:ConversationTopic and aggregates on item:DateTimeReceived (maximum).</span></span> <span data-ttu-id="04885-124">Para obter mais informações sobre agregação de lista segura, consulte [AggregateOn](aggregateon.md).</span><span class="sxs-lookup"><span data-stu-id="04885-124">For more information about aggregation, see [AggregateOn](aggregateon.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="04885-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="04885-125">Remarks</span></span>

<span data-ttu-id="04885-126">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="04885-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04885-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="04885-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04885-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="04885-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04885-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="04885-129">Schema Name</span></span>  <br/> |<span data-ttu-id="04885-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="04885-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="04885-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="04885-131">Validation File</span></span>  <br/> |<span data-ttu-id="04885-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="04885-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04885-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="04885-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="04885-134">False</span><span class="sxs-lookup"><span data-stu-id="04885-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04885-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="04885-135">See also</span></span>



[<span data-ttu-id="04885-136">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="04885-136">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="04885-137">FindItem</span><span class="sxs-lookup"><span data-stu-id="04885-137">FindItem</span></span>](finditem.md)


[<span data-ttu-id="04885-138">Localizando itens</span><span class="sxs-lookup"><span data-stu-id="04885-138">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

