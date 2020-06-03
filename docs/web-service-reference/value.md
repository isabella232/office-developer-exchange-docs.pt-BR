---
title: Valor
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
description: O elemento Value contém o valor de uma propriedade estendida.
ms.openlocfilehash: 5de1528dda6d58ea772d050e709c0720e389fae6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465209"
---
# <a name="value"></a><span data-ttu-id="cd66b-103">Valor</span><span class="sxs-lookup"><span data-stu-id="cd66b-103">Value</span></span>

<span data-ttu-id="cd66b-104">O elemento **Value** contém o valor de uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="cd66b-104">The **Value** element contains the value of an extended property.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="cd66b-105">**String**</span><span class="sxs-lookup"><span data-stu-id="cd66b-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="cd66b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cd66b-106">Attributes and elements</span></span>

<span data-ttu-id="cd66b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cd66b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd66b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cd66b-108">Attributes</span></span>

<span data-ttu-id="cd66b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd66b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cd66b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cd66b-110">Child elements</span></span>

<span data-ttu-id="cd66b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cd66b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cd66b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cd66b-112">Parent elements</span></span>

|<span data-ttu-id="cd66b-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cd66b-113">**Element**</span></span>|<span data-ttu-id="cd66b-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cd66b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd66b-115">Valores</span><span class="sxs-lookup"><span data-stu-id="cd66b-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="cd66b-116">Contém uma coleção de valores para uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="cd66b-116">Contains a collection of values for an extended property.</span></span>  <br/> |
|[<span data-ttu-id="cd66b-117">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="cd66b-117">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="cd66b-118">Identifica as propriedades estendidas em pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="cd66b-118">Identifies extended properties on folders and items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cd66b-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="cd66b-119">Text value</span></span>

<span data-ttu-id="cd66b-120">O valor de texto deve ser compatível com o tipo indicado pelo atributo Recordtypepropriedade de ExtendedFieldURI.</span><span class="sxs-lookup"><span data-stu-id="cd66b-120">The text value must be compatible with the type that is indicated by the PropertyType attribute of the ExtendedFieldURI.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cd66b-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="cd66b-121">Remarks</span></span>

<span data-ttu-id="cd66b-122">Um elemento **Value** pode ocorrer em instâncias de propriedade estendidas com um ou vários valores.</span><span class="sxs-lookup"><span data-stu-id="cd66b-122">A **Value** element can occur in both single and multivalued extended property instances.</span></span> <span data-ttu-id="cd66b-123">Para instâncias de valor único, ela existe como um filho direto do elemento [Extended](extendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="cd66b-123">For single-valued instances, it exists as a direct child of the [ExtendedProperty](extendedproperty.md) element.</span></span> <span data-ttu-id="cd66b-124">Para uma instância com vários valores, ela existe como um filho direto da coleção **Values** .</span><span class="sxs-lookup"><span data-stu-id="cd66b-124">For multivalued instance, it exists as a direct child of the **Values** collection.</span></span> 
  
<span data-ttu-id="cd66b-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="cd66b-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd66b-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cd66b-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd66b-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="cd66b-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cd66b-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cd66b-128">Schema Name</span></span>  <br/> |<span data-ttu-id="cd66b-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="cd66b-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="cd66b-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cd66b-130">Validation File</span></span>  <br/> |<span data-ttu-id="cd66b-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cd66b-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cd66b-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cd66b-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="cd66b-133">False</span><span class="sxs-lookup"><span data-stu-id="cd66b-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cd66b-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="cd66b-134">See also</span></span>

- [<span data-ttu-id="cd66b-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cd66b-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

