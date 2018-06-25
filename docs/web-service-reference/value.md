---
title: Value
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: 9a30cadd-909e-41b1-b4e9-291643dd89c6
description: O elemento de valor contém o valor de uma propriedade estendida.
ms.openlocfilehash: 4b8674d267b78f0384f9457e794e88ace8234826
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838032"
---
# <a name="value"></a><span data-ttu-id="a3af2-103">Value</span><span class="sxs-lookup"><span data-stu-id="a3af2-103">Value</span></span>

<span data-ttu-id="a3af2-104">O elemento de **valor** contém o valor de uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="a3af2-104">The **Value** element contains the value of an extended property.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="a3af2-105">**String**</span><span class="sxs-lookup"><span data-stu-id="a3af2-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a3af2-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a3af2-106">Attributes and elements</span></span>

<span data-ttu-id="a3af2-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a3af2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3af2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a3af2-108">Attributes</span></span>

<span data-ttu-id="a3af2-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a3af2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3af2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a3af2-110">Child elements</span></span>

<span data-ttu-id="a3af2-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a3af2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a3af2-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a3af2-112">Parent elements</span></span>

|<span data-ttu-id="a3af2-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a3af2-113">**Element**</span></span>|<span data-ttu-id="a3af2-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a3af2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3af2-115">Values</span><span class="sxs-lookup"><span data-stu-id="a3af2-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="a3af2-116">Contém uma coleção de valores para uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="a3af2-116">Contains a collection of values for an extended property.</span></span>  <br/> |
|[<span data-ttu-id="a3af2-117">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="a3af2-117">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="a3af2-118">Identifica as propriedades estendidas em pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="a3af2-118">Identifies extended properties on folders and items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a3af2-119">Text value</span><span class="sxs-lookup"><span data-stu-id="a3af2-119">Text value</span></span>

<span data-ttu-id="a3af2-120">O valor de texto deve ser compatível com o tipo indicado pelo atributo PropertyType do ExtendedFieldURI.</span><span class="sxs-lookup"><span data-stu-id="a3af2-120">The text value must be compatible with the type that is indicated by the PropertyType attribute of the ExtendedFieldURI.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a3af2-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="a3af2-121">Remarks</span></span>

<span data-ttu-id="a3af2-122">Um elemento de **valor** pode ocorrer em ambas as instâncias de único e vários valores de propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="a3af2-122">A **Value** element can occur in both single and multivalued extended property instances.</span></span> <span data-ttu-id="a3af2-123">Instâncias de valor único, ele existe como um filho direto do elemento [ExtendedProperty](extendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="a3af2-123">For single-valued instances, it exists as a direct child of the [ExtendedProperty](extendedproperty.md) element.</span></span> <span data-ttu-id="a3af2-124">Para uma instância multivalorada, ele existe como um filho direto do conjunto de **valores** .</span><span class="sxs-lookup"><span data-stu-id="a3af2-124">For multivalued instance, it exists as a direct child of the **Values** collection.</span></span> 
  
<span data-ttu-id="a3af2-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="a3af2-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3af2-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a3af2-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3af2-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="a3af2-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a3af2-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a3af2-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a3af2-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a3af2-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="a3af2-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a3af2-130">Validation File</span></span>  <br/> |<span data-ttu-id="a3af2-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a3af2-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a3af2-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a3af2-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a3af2-133">False</span><span class="sxs-lookup"><span data-stu-id="a3af2-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a3af2-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="a3af2-134">See also</span></span>

- [<span data-ttu-id="a3af2-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a3af2-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

