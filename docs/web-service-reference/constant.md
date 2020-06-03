---
title: Constant
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Constant
api_type:
- schema
ms.assetid: 340af0cd-9f12-44ab-b8f1-21d107c8d0c9
description: O elemento Constant identifica um valor de constante em uma restrição.
ms.openlocfilehash: 6cb2eaa4227a8fd0985e8ff5a15d647c3bb1cd6a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461552"
---
# <a name="constant"></a><span data-ttu-id="87cfa-103">Constant</span><span class="sxs-lookup"><span data-stu-id="87cfa-103">Constant</span></span>

<span data-ttu-id="87cfa-104">O elemento **Constant** identifica um valor de constante em uma restrição.</span><span class="sxs-lookup"><span data-stu-id="87cfa-104">The **Constant** element identifies a constant value in a restriction.</span></span> 
  
```xml
<Constant Value="" />
```

 <span data-ttu-id="87cfa-105">**ConstantValueType**</span><span class="sxs-lookup"><span data-stu-id="87cfa-105">**ConstantValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="87cfa-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="87cfa-106">Attributes and elements</span></span>

<span data-ttu-id="87cfa-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="87cfa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="87cfa-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="87cfa-108">Attributes</span></span>

|<span data-ttu-id="87cfa-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="87cfa-109">**Attribute**</span></span>|<span data-ttu-id="87cfa-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="87cfa-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="87cfa-111">**Valor**</span><span class="sxs-lookup"><span data-stu-id="87cfa-111">**Value**</span></span> <br/> |<span data-ttu-id="87cfa-112">Especifica o valor a ser comparado na restrição.</span><span class="sxs-lookup"><span data-stu-id="87cfa-112">Specifies the value to compare in the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="87cfa-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="87cfa-113">Child elements</span></span>

<span data-ttu-id="87cfa-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="87cfa-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="87cfa-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="87cfa-115">Parent elements</span></span>

|<span data-ttu-id="87cfa-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="87cfa-116">**Element**</span></span>|<span data-ttu-id="87cfa-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="87cfa-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87cfa-118">Contém</span><span class="sxs-lookup"><span data-stu-id="87cfa-118">Contains</span></span>](contains.md) <br/> |<span data-ttu-id="87cfa-119">Representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor de cadeia de caracteres constante fornecido.</span><span class="sxs-lookup"><span data-stu-id="87cfa-119">Represents a search expression that determines whether a given property contains the supplied constant string value.</span></span>  <br/> |
|[<span data-ttu-id="87cfa-120">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="87cfa-120">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="87cfa-121">Representa uma propriedade ou um valor de constante a ser usado ao comparar com outra propriedade.</span><span class="sxs-lookup"><span data-stu-id="87cfa-121">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="87cfa-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="87cfa-122">Remarks</span></span>

<span data-ttu-id="87cfa-123">O valor da cadeia de caracteres no atributo **Value** deve ser coercible no tipo que você está tentando comparar.</span><span class="sxs-lookup"><span data-stu-id="87cfa-123">The string value in the **Value** attribute must be coercible into the type you are trying to compare against.</span></span> <span data-ttu-id="87cfa-124">Por exemplo, se você estiver comparando uma propriedade data/hora em relação a um valor constante, o valor da cadeia de caracteres deverá representar uma data/hora.</span><span class="sxs-lookup"><span data-stu-id="87cfa-124">For example, if you are comparing a date/time property against a constant value, the string value must represent a date/time.</span></span> 
  
<span data-ttu-id="87cfa-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="87cfa-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="87cfa-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="87cfa-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="87cfa-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="87cfa-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="87cfa-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="87cfa-128">Schema Name</span></span>  <br/> |<span data-ttu-id="87cfa-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="87cfa-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="87cfa-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="87cfa-130">Validation File</span></span>  <br/> |<span data-ttu-id="87cfa-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="87cfa-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="87cfa-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="87cfa-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="87cfa-133">False</span><span class="sxs-lookup"><span data-stu-id="87cfa-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="87cfa-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="87cfa-134">See also</span></span>



- [<span data-ttu-id="87cfa-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="87cfa-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

