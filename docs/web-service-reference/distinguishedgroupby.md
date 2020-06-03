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
description: O elemento DistinguishedGroupBy fornece agrupamentos padrão para consultas do FindItem.
ms.openlocfilehash: 004613d55419a19f69e960203ae13d8d906b74c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463136"
---
# <a name="distinguishedgroupby"></a><span data-ttu-id="4d0c3-103">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="4d0c3-103">DistinguishedGroupBy</span></span>

<span data-ttu-id="4d0c3-104">O elemento **DistinguishedGroupBy** fornece agrupamentos padrão para consultas do FindItem.</span><span class="sxs-lookup"><span data-stu-id="4d0c3-104">The **DistinguishedGroupBy** element provides standard groupings for FindItem queries.</span></span> 
  
- [<span data-ttu-id="4d0c3-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="4d0c3-105">FindItem</span></span>](finditem.md) 
- [<span data-ttu-id="4d0c3-106">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="4d0c3-106">DistinguishedGroupBy</span></span>](distinguishedgroupby.md)
  
```xml
<DistinguishedGroupBy>
   <StandardGroupBy/>
</DistinguishedGroupBy>
```

 <span data-ttu-id="4d0c3-107">**DistinguishedGroupByType**</span><span class="sxs-lookup"><span data-stu-id="4d0c3-107">**DistinguishedGroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d0c3-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4d0c3-108">Attributes and elements</span></span>

<span data-ttu-id="4d0c3-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4d0c3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d0c3-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="4d0c3-110">Attributes</span></span>

<span data-ttu-id="4d0c3-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4d0c3-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d0c3-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4d0c3-112">Child elements</span></span>

|<span data-ttu-id="4d0c3-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4d0c3-113">**Element**</span></span>|<span data-ttu-id="4d0c3-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4d0c3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d0c3-115">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="4d0c3-115">StandardGroupBy</span></span>](standardgroupby.md) <br/> |<span data-ttu-id="4d0c3-116">Representa os mecanismos padrão de agrupamento e agregação para uma operação FindItem agrupada.</span><span class="sxs-lookup"><span data-stu-id="4d0c3-116">Represents the standard grouping and aggregating mechanisms for a grouped FindItem operation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4d0c3-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4d0c3-117">Parent elements</span></span>

|<span data-ttu-id="4d0c3-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4d0c3-118">**Element**</span></span>|<span data-ttu-id="4d0c3-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4d0c3-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d0c3-120">FindItem</span><span class="sxs-lookup"><span data-stu-id="4d0c3-120">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="4d0c3-121">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4d0c3-121">Defines a request to find items in a mailbox.</span></span><br/><br/><span data-ttu-id="4d0c3-122">A seguir está a expressão XPath para este elemento:`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="4d0c3-122">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4d0c3-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="4d0c3-123">Remarks</span></span>

<span data-ttu-id="4d0c3-124">O elemento **DistinguishedGroupBy** pode ser adicionado a uma operação FindItem quando os resultados precisam ser agrupados e quando um dos grupos padrão atende aos requisitos de agrupamento.</span><span class="sxs-lookup"><span data-stu-id="4d0c3-124">The **DistinguishedGroupBy** element can be added to a FindItem operation when the results must come backed grouped and when one of the standard groups meets the grouping requirements.</span></span> <span data-ttu-id="4d0c3-125">Se nem o elemento **DistinguishedGroupBy** nem o elemento [GroupBy](groupby.md) for especificado, os resultados do FindItem retornarão de Ungrouped.</span><span class="sxs-lookup"><span data-stu-id="4d0c3-125">If neither the **DistinguishedGroupBy** element nor the [GroupBy](groupby.md) element is specified, FindItem results will come back ungrouped.</span></span> 
  
<span data-ttu-id="4d0c3-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="4d0c3-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d0c3-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4d0c3-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d0c3-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="4d0c3-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4d0c3-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4d0c3-129">Schema Name</span></span>  <br/> |<span data-ttu-id="4d0c3-130">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="4d0c3-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4d0c3-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4d0c3-131">Validation File</span></span>  <br/> |<span data-ttu-id="4d0c3-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4d0c3-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4d0c3-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4d0c3-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="4d0c3-134">False</span><span class="sxs-lookup"><span data-stu-id="4d0c3-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d0c3-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="4d0c3-135">See also</span></span>

- [<span data-ttu-id="4d0c3-136">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="4d0c3-136">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="4d0c3-137">Localizar itens</span><span class="sxs-lookup"><span data-stu-id="4d0c3-137">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

