---
title: FieldOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FieldOrder
api_type:
- schema
ms.assetid: b9364842-bbe2-4221-afef-bf5022bc89ec
description: O elemento FieldOrder representa um único campo pelo qual fazer a classificação de resultados e indica a direção para a classificação.
ms.openlocfilehash: 10e28f066f7fa6799bf6b03b694d98825f95626d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752239"
---
# <a name="fieldorder"></a><span data-ttu-id="dbc4b-103">FieldOrder</span><span class="sxs-lookup"><span data-stu-id="dbc4b-103">FieldOrder</span></span>

<span data-ttu-id="dbc4b-104">O elemento **FieldOrder** representa um único campo pelo qual fazer a classificação de resultados e indica a direção para a classificação.</span><span class="sxs-lookup"><span data-stu-id="dbc4b-104">The **FieldOrder** element represents a single field by which to sort results and indicates the direction for the sort.</span></span> 
  
```xml
<FieldOrder Order="">
   <FieldURI/>
</FieldOrder>
```

 <span data-ttu-id="dbc4b-105">**FieldOrderType**</span><span class="sxs-lookup"><span data-stu-id="dbc4b-105">**FieldOrderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dbc4b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="dbc4b-106">Attributes and elements</span></span>

<span data-ttu-id="dbc4b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dbc4b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dbc4b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="dbc4b-108">Attributes</span></span>

|<span data-ttu-id="dbc4b-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="dbc4b-109">**Attribute**</span></span>|<span data-ttu-id="dbc4b-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dbc4b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dbc4b-111">**Order**</span><span class="sxs-lookup"><span data-stu-id="dbc4b-111">**Order**</span></span> <br/> | <span data-ttu-id="dbc4b-112">Descreve a direção da ordem de classificação.</span><span class="sxs-lookup"><span data-stu-id="dbc4b-112">Describes the sort order direction.</span></span><br/><br/> <span data-ttu-id="dbc4b-113">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="dbc4b-113">The following are the possible values:</span></span> <br/> <br/><span data-ttu-id="dbc4b-114">-Crescente</span><span class="sxs-lookup"><span data-stu-id="dbc4b-114">-  Ascending</span></span>  <br/><span data-ttu-id="dbc4b-115">-Decrescente</span><span class="sxs-lookup"><span data-stu-id="dbc4b-115">-  Descending</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="dbc4b-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dbc4b-116">Child elements</span></span>

|<span data-ttu-id="dbc4b-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dbc4b-117">**Element**</span></span>|<span data-ttu-id="dbc4b-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dbc4b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbc4b-119">FieldURI</span><span class="sxs-lookup"><span data-stu-id="dbc4b-119">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="dbc4b-120">Identifica as propriedades frequentemente referenciadas pelo URI.</span><span class="sxs-lookup"><span data-stu-id="dbc4b-120">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="dbc4b-121">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="dbc4b-121">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="dbc4b-122">Identifica a membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="dbc4b-122">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="dbc4b-123">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="dbc4b-123">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="dbc4b-124">Identifica as propriedades MAPI.</span><span class="sxs-lookup"><span data-stu-id="dbc4b-124">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dbc4b-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dbc4b-125">Parent elements</span></span>

|<span data-ttu-id="dbc4b-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dbc4b-126">**Element**</span></span>|<span data-ttu-id="dbc4b-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dbc4b-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbc4b-128">SortOrder</span><span class="sxs-lookup"><span data-stu-id="dbc4b-128">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="dbc4b-129">Define como os itens são classificados em uma solicitação de FindItem.</span><span class="sxs-lookup"><span data-stu-id="dbc4b-129">Defines how items are sorted in a FindItem request.</span></span>  <br/> <span data-ttu-id="dbc4b-130">Este é a expressão XPath para esse elemento:`/FindItem/SortOrder`</span><span class="sxs-lookup"><span data-stu-id="dbc4b-130">The following is the XPath expression to this element:  `/FindItem/SortOrder`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dbc4b-131">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="dbc4b-131">Remarks</span></span>

<span data-ttu-id="dbc4b-132">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="dbc4b-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dbc4b-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="dbc4b-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dbc4b-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="dbc4b-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dbc4b-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dbc4b-135">Schema Name</span></span>  <br/> |<span data-ttu-id="dbc4b-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="dbc4b-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="dbc4b-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dbc4b-137">Validation File</span></span>  <br/> |<span data-ttu-id="dbc4b-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dbc4b-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dbc4b-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="dbc4b-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="dbc4b-140">False</span><span class="sxs-lookup"><span data-stu-id="dbc4b-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dbc4b-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="dbc4b-141">See also</span></span>

- [<span data-ttu-id="dbc4b-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="dbc4b-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

