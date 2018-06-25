---
title: DistinguishedGroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedGroupBy
api_type:
- schema
ms.assetid: 6ff3ac48-02ba-40ec-a71b-c401bb2b127c
description: O elemento DistinguishedGroupBy fornece agrupamentos padrão para consultas FindItem.
ms.openlocfilehash: 0635366447675bf28dedf3af4f7d76094ee5e0a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751897"
---
# <a name="distinguishedgroupby"></a><span data-ttu-id="43cb5-103">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="43cb5-103">DistinguishedGroupBy</span></span>

<span data-ttu-id="43cb5-104">O elemento **DistinguishedGroupBy** fornece agrupamentos padrão para consultas FindItem.</span><span class="sxs-lookup"><span data-stu-id="43cb5-104">The **DistinguishedGroupBy** element provides standard groupings for FindItem queries.</span></span> 
  
- [<span data-ttu-id="43cb5-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="43cb5-105">FindItem</span></span>](finditem.md) 
- [<span data-ttu-id="43cb5-106">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="43cb5-106">DistinguishedGroupBy</span></span>](distinguishedgroupby.md)
  
```xml
<DistinguishedGroupBy>
   <StandardGroupBy/>
</DistinguishedGroupBy>
```

 <span data-ttu-id="43cb5-107">**DistinguishedGroupByType**</span><span class="sxs-lookup"><span data-stu-id="43cb5-107">**DistinguishedGroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="43cb5-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="43cb5-108">Attributes and elements</span></span>

<span data-ttu-id="43cb5-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="43cb5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="43cb5-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="43cb5-110">Attributes</span></span>

<span data-ttu-id="43cb5-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="43cb5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="43cb5-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="43cb5-112">Child elements</span></span>

|<span data-ttu-id="43cb5-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="43cb5-113">**Element**</span></span>|<span data-ttu-id="43cb5-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="43cb5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43cb5-115">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="43cb5-115">StandardGroupBy</span></span>](standardgroupby.md) <br/> |<span data-ttu-id="43cb5-116">Representa o padrão de agrupamento e agregar mecanismos para uma operação de FindItem agrupada.</span><span class="sxs-lookup"><span data-stu-id="43cb5-116">Represents the standard grouping and aggregating mechanisms for a grouped FindItem operation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="43cb5-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="43cb5-117">Parent elements</span></span>

|<span data-ttu-id="43cb5-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="43cb5-118">**Element**</span></span>|<span data-ttu-id="43cb5-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="43cb5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43cb5-120">FindItem</span><span class="sxs-lookup"><span data-stu-id="43cb5-120">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="43cb5-121">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="43cb5-121">Defines a request to find items in a mailbox.</span></span><br/><br/><span data-ttu-id="43cb5-122">Este é a expressão XPath para esse elemento:`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="43cb5-122">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="43cb5-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="43cb5-123">Remarks</span></span>

<span data-ttu-id="43cb5-124">O elemento **DistinguishedGroupBy** pode ser adicionado a uma operação FindItem quando os resultados devem vir armazenados agrupados e quando um dos grupos padrão atende aos requisitos de agrupamento.</span><span class="sxs-lookup"><span data-stu-id="43cb5-124">The **DistinguishedGroupBy** element can be added to a FindItem operation when the results must come backed grouped and when one of the standard groups meets the grouping requirements.</span></span> <span data-ttu-id="43cb5-125">Se nem o elemento **DistinguishedGroupBy** nem o elemento [GroupBy](groupby.md) for especificado, desagrupado FindItem resultados retornarão.</span><span class="sxs-lookup"><span data-stu-id="43cb5-125">If neither the **DistinguishedGroupBy** element nor the [GroupBy](groupby.md) element is specified, FindItem results will come back ungrouped.</span></span> 
  
<span data-ttu-id="43cb5-126">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="43cb5-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="43cb5-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="43cb5-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="43cb5-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="43cb5-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="43cb5-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="43cb5-129">Schema Name</span></span>  <br/> |<span data-ttu-id="43cb5-130">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="43cb5-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="43cb5-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="43cb5-131">Validation File</span></span>  <br/> |<span data-ttu-id="43cb5-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="43cb5-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="43cb5-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="43cb5-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="43cb5-134">False</span><span class="sxs-lookup"><span data-stu-id="43cb5-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="43cb5-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="43cb5-135">See also</span></span>

- [<span data-ttu-id="43cb5-136">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="43cb5-136">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="43cb5-137">Localizando itens</span><span class="sxs-lookup"><span data-stu-id="43cb5-137">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

