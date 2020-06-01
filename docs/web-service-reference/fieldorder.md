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
description: O elemento FieldOrder representa um único campo pelo qual classificar os resultados e indica a direção da classificação.
ms.openlocfilehash: 19dee7175d541dd99b53e004ea8ccd785b619184
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461258"
---
# <a name="fieldorder"></a><span data-ttu-id="1615a-103">FieldOrder</span><span class="sxs-lookup"><span data-stu-id="1615a-103">FieldOrder</span></span>

<span data-ttu-id="1615a-104">O elemento **FieldOrder** representa um único campo pelo qual classificar os resultados e indica a direção da classificação.</span><span class="sxs-lookup"><span data-stu-id="1615a-104">The **FieldOrder** element represents a single field by which to sort results and indicates the direction for the sort.</span></span> 
  
```xml
<FieldOrder Order="">
   <FieldURI/>
</FieldOrder>
```

```xml
<FieldOrder Order="">
   <ExtendedFieldURI/> 
</FieldOrder>
```

```xml
<FieldOrder Order="">
   <IndexedFieldURI/>
</FieldOrder>
```

<span data-ttu-id="1615a-105">**FieldOrderType**</span><span class="sxs-lookup"><span data-stu-id="1615a-105">**FieldOrderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1615a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1615a-106">Attributes and elements</span></span>

<span data-ttu-id="1615a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1615a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1615a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1615a-108">Attributes</span></span>

|<span data-ttu-id="1615a-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="1615a-109">**Attribute**</span></span>|<span data-ttu-id="1615a-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1615a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1615a-111">**Order**</span><span class="sxs-lookup"><span data-stu-id="1615a-111">**Order**</span></span> <br/> | <span data-ttu-id="1615a-112">Descreve a direção da ordem de classificação.</span><span class="sxs-lookup"><span data-stu-id="1615a-112">Describes the sort order direction.</span></span><br/><br/> <span data-ttu-id="1615a-113">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="1615a-113">The following are the possible values:</span></span> <br/> <br/><span data-ttu-id="1615a-114">– Crescente</span><span class="sxs-lookup"><span data-stu-id="1615a-114">-  Ascending</span></span>  <br/><span data-ttu-id="1615a-115">-Decrescente</span><span class="sxs-lookup"><span data-stu-id="1615a-115">-  Descending</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1615a-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1615a-116">Child elements</span></span>

|<span data-ttu-id="1615a-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1615a-117">**Element**</span></span>|<span data-ttu-id="1615a-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1615a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1615a-119">FieldURI</span><span class="sxs-lookup"><span data-stu-id="1615a-119">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="1615a-120">Identifica as propriedades com frequência referenciadas por URI.</span><span class="sxs-lookup"><span data-stu-id="1615a-120">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="1615a-121">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="1615a-121">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="1615a-122">Identifica membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="1615a-122">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="1615a-123">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="1615a-123">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="1615a-124">Identifica as propriedades MAPI.</span><span class="sxs-lookup"><span data-stu-id="1615a-124">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1615a-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1615a-125">Parent elements</span></span>

|<span data-ttu-id="1615a-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1615a-126">**Element**</span></span>|<span data-ttu-id="1615a-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1615a-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1615a-128">SortOrder</span><span class="sxs-lookup"><span data-stu-id="1615a-128">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="1615a-129">Define como os itens são classificados em uma solicitação FindItem.</span><span class="sxs-lookup"><span data-stu-id="1615a-129">Defines how items are sorted in a FindItem request.</span></span>  <br/> <span data-ttu-id="1615a-130">A seguir está a expressão XPath para este elemento:`/FindItem/SortOrder`</span><span class="sxs-lookup"><span data-stu-id="1615a-130">The following is the XPath expression to this element:  `/FindItem/SortOrder`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1615a-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="1615a-131">Remarks</span></span>

<span data-ttu-id="1615a-132">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="1615a-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1615a-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1615a-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1615a-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="1615a-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1615a-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1615a-135">Schema Name</span></span>  <br/> |<span data-ttu-id="1615a-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1615a-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="1615a-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1615a-137">Validation File</span></span>  <br/> |<span data-ttu-id="1615a-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1615a-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1615a-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1615a-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="1615a-140">False</span><span class="sxs-lookup"><span data-stu-id="1615a-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1615a-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="1615a-141">See also</span></span>

- [<span data-ttu-id="1615a-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1615a-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

