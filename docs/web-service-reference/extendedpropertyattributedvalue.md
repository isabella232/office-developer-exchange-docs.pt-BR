---
title: ExtendedPropertyAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90f3c5c5-f612-4e1b-b1f5-f92dd8524179
description: O elemento ExtendedPropertyAttributedValue especifica as propriedades estendidas para uma pessoa.
ms.openlocfilehash: 5c2ad5918d7ac666d5e26af6597b2c4c3dde6202
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460124"
---
# <a name="extendedpropertyattributedvalue"></a><span data-ttu-id="355a2-103">ExtendedPropertyAttributedValue</span><span class="sxs-lookup"><span data-stu-id="355a2-103">ExtendedPropertyAttributedValue</span></span>

<span data-ttu-id="355a2-104">O elemento **ExtendedPropertyAttributedValue** especifica as propriedades estendidas para uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="355a2-104">The **ExtendedPropertyAttributedValue** element specifies extended properties for a persona.</span></span> 
  
```XML
<ExtendedPropertyAttributedValue>
    <Value/>
    <Attributions/>
</ExtendedPropertyAttributedValue>
```

 <span data-ttu-id="355a2-105">**ExtendedPropertyAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="355a2-105">**ExtendedPropertyAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="355a2-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="355a2-106">Attributes and elements</span></span>

<span data-ttu-id="355a2-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="355a2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="355a2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="355a2-108">Attributes</span></span>

<span data-ttu-id="355a2-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="355a2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="355a2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="355a2-110">Child elements</span></span>

|<span data-ttu-id="355a2-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="355a2-111">**Element**</span></span>|<span data-ttu-id="355a2-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="355a2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="355a2-113">Valor (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="355a2-113">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md) <br/> |<span data-ttu-id="355a2-114">Especifica uma matriz de propriedades estendidas para uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="355a2-114">Specifies an array of extended properties for a persona.</span></span>  <br/> |
|[<span data-ttu-id="355a2-115">Atribuições (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="355a2-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="355a2-116">Especifica uma matriz de atribuições para o elemento de **valor** associado.</span><span class="sxs-lookup"><span data-stu-id="355a2-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="355a2-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="355a2-117">Parent elements</span></span>

|<span data-ttu-id="355a2-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="355a2-118">**Element**</span></span>|<span data-ttu-id="355a2-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="355a2-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="355a2-120">ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)</span><span class="sxs-lookup"><span data-stu-id="355a2-120">ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)</span></span>](extendedproperties-arrayofextendedpropertyattributedvaluetype.md) <br/> |<span data-ttu-id="355a2-121">Contém as propriedades estendidas usadas para operações do repositório unificado de contatos.</span><span class="sxs-lookup"><span data-stu-id="355a2-121">Contains the extended properties used for Unified Contact Store operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="355a2-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="355a2-122">Remarks</span></span>

<span data-ttu-id="355a2-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="355a2-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="355a2-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="355a2-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="355a2-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="355a2-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="355a2-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="355a2-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="355a2-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="355a2-127">Schema Name</span></span>  <br/> |<span data-ttu-id="355a2-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="355a2-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="355a2-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="355a2-129">Validation File</span></span>  <br/> |<span data-ttu-id="355a2-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="355a2-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="355a2-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="355a2-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="355a2-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="355a2-132">See also</span></span>



- [<span data-ttu-id="355a2-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="355a2-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

