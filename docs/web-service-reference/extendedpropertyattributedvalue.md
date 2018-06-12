---
title: ExtendedPropertyAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90f3c5c5-f612-4e1b-b1f5-f92dd8524179
description: O elemento ExtendedPropertyAttributedValue Especifica as propriedades estendidas para uma pessoa.
ms.openlocfilehash: 92e4ec7f192ccb36ea68d7862e66cb7b3349819a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752179"
---
# <a name="extendedpropertyattributedvalue"></a><span data-ttu-id="d1221-103">ExtendedPropertyAttributedValue</span><span class="sxs-lookup"><span data-stu-id="d1221-103">ExtendedPropertyAttributedValue</span></span>

<span data-ttu-id="d1221-104">O elemento **ExtendedPropertyAttributedValue** Especifica as propriedades estendidas para uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="d1221-104">The **ExtendedPropertyAttributedValue** element specifies extended properties for a persona.</span></span> 
  
```XML
<ExtendedPropertyAttributedValue>
    <Value/>
    <Attributions/>
</ExtendedPropertyAttributedValue>
```

 <span data-ttu-id="d1221-105">**ExtendedPropertyAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="d1221-105">**ExtendedPropertyAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d1221-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d1221-106">Attributes and elements</span></span>

<span data-ttu-id="d1221-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d1221-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1221-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d1221-108">Attributes</span></span>

<span data-ttu-id="d1221-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d1221-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1221-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d1221-110">Child elements</span></span>

|<span data-ttu-id="d1221-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d1221-111">**Element**</span></span>|<span data-ttu-id="d1221-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d1221-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1221-113">Valor (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="d1221-113">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md) <br/> |<span data-ttu-id="d1221-114">Especifica uma matriz de propriedades estendidas para uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="d1221-114">Specifies an array of extended properties for a persona.</span></span>  <br/> |
|[<span data-ttu-id="d1221-115">Atribuições (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="d1221-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="d1221-116">Especifica uma matriz de atribuições para seu elemento **valor** associado.</span><span class="sxs-lookup"><span data-stu-id="d1221-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d1221-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d1221-117">Parent elements</span></span>

|<span data-ttu-id="d1221-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d1221-118">**Element**</span></span>|<span data-ttu-id="d1221-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d1221-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1221-120">ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)</span><span class="sxs-lookup"><span data-stu-id="d1221-120">ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)</span></span>](extendedproperties-arrayofextendedpropertyattributedvaluetype.md) <br/> |<span data-ttu-id="d1221-121">Contém as propriedades estendidas usadas para operações de repositório unificado de contatos.</span><span class="sxs-lookup"><span data-stu-id="d1221-121">Contains the extended properties used for Unified Contact Store operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d1221-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="d1221-122">Remarks</span></span>

<span data-ttu-id="d1221-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d1221-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d1221-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1221-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1221-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d1221-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1221-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="d1221-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d1221-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d1221-127">Schema Name</span></span>  <br/> |<span data-ttu-id="d1221-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="d1221-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="d1221-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d1221-129">Validation File</span></span>  <br/> |<span data-ttu-id="d1221-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d1221-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d1221-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d1221-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d1221-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="d1221-132">See also</span></span>



- [<span data-ttu-id="d1221-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d1221-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

