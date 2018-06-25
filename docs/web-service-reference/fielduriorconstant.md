---
title: FieldURIOrConstant
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FieldURIOrConstant
api_type:
- schema
ms.assetid: 89d7a87e-7c93-49b8-83ec-8798e08c1052
description: O elemento FieldURIOrConstant representa uma propriedade ou um valor de constante a ser usado ao comparar com outra propriedade.
ms.openlocfilehash: 5195feec2a314d9ec15dc4a25a7a014aded1696a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752245"
---
# <a name="fielduriorconstant"></a><span data-ttu-id="f188b-103">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="f188b-103">FieldURIOrConstant</span></span>

<span data-ttu-id="f188b-104">O elemento **FieldURIOrConstant** representa uma propriedade ou um valor de constante a ser usado ao comparar com outra propriedade.</span><span class="sxs-lookup"><span data-stu-id="f188b-104">The **FieldURIOrConstant** element represents either a property or a constant value to be used when comparing with another property.</span></span> 
  
```xml
<FieldURIOrConstant>
   <Constant/>
</FieldURIOrConstant>
```

 <span data-ttu-id="f188b-105">**FieldURIOrConstantType**</span><span class="sxs-lookup"><span data-stu-id="f188b-105">**FieldURIOrConstantType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f188b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f188b-106">Attributes and elements</span></span>

<span data-ttu-id="f188b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f188b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f188b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f188b-108">Attributes</span></span>

<span data-ttu-id="f188b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f188b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f188b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f188b-110">Child elements</span></span>

|<span data-ttu-id="f188b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f188b-111">**Element**</span></span>|<span data-ttu-id="f188b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f188b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f188b-113">Constante</span><span class="sxs-lookup"><span data-stu-id="f188b-113">Constant</span></span>](constant.md) <br/> |<span data-ttu-id="f188b-114">Identifica um valor de constante em uma restrição.</span><span class="sxs-lookup"><span data-stu-id="f188b-114">Identifies a constant value in a restriction.</span></span>  <br/> |
|[<span data-ttu-id="f188b-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="f188b-115">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="f188b-116">Identifica as propriedades frequentemente referenciadas pelo URI.</span><span class="sxs-lookup"><span data-stu-id="f188b-116">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="f188b-117">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="f188b-117">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="f188b-118">Identifica a membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="f188b-118">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="f188b-119">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="f188b-119">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="f188b-120">Identifica as propriedades MAPI.</span><span class="sxs-lookup"><span data-stu-id="f188b-120">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f188b-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f188b-121">Parent elements</span></span>

|<span data-ttu-id="f188b-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f188b-122">**Element**</span></span>|<span data-ttu-id="f188b-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f188b-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f188b-124">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="f188b-124">IsEqualTo</span></span>](isequalto.md) <br/> |<span data-ttu-id="f188b-125">Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retornará true se eles forem iguais.</span><span class="sxs-lookup"><span data-stu-id="f188b-125">Represents a search expression that compares a property with either a constant value or another property and evaluates to true if they are equal.</span></span>  <br/> |
|[<span data-ttu-id="f188b-126">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="f188b-126">IsGreaterThan</span></span>](isgreaterthan.md) <br/> |<span data-ttu-id="f188b-127">Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se a primeira propriedade for maior.</span><span class="sxs-lookup"><span data-stu-id="f188b-127">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is greater.</span></span>  <br/> |
|[<span data-ttu-id="f188b-128">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="f188b-128">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md) <br/> |<span data-ttu-id="f188b-129">Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se a primeira propriedade for maior que ou igual ao segundo valor ou propriedade.</span><span class="sxs-lookup"><span data-stu-id="f188b-129">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is greater than or equal to the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="f188b-130">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="f188b-130">IsLessThan</span></span>](islessthan.md) <br/> |<span data-ttu-id="f188b-131">Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se a primeira propriedade for menor que o segundo valor ou a propriedade.</span><span class="sxs-lookup"><span data-stu-id="f188b-131">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is less than the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="f188b-132">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="f188b-132">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md) <br/> |<span data-ttu-id="f188b-133">Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se a primeira propriedade for menor ou igual ao segundo valor ou propriedade.</span><span class="sxs-lookup"><span data-stu-id="f188b-133">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is less than or equal to the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="f188b-134">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="f188b-134">IsNotEqualTo</span></span>](isnotequalto.md) <br/> |<span data-ttu-id="f188b-135">Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se os valores não são iguais.</span><span class="sxs-lookup"><span data-stu-id="f188b-135">Represents a search expression that compares a property with either a constant value or another property and returns true if the values are not the same.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f188b-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="f188b-136">Remarks</span></span>

<span data-ttu-id="f188b-137">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f188b-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="f188b-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f188b-138">Example</span></span>

<span data-ttu-id="f188b-139">O exemplo XML a seguir mostra o elemento FieldURIOrConstant usado com uma constante e o URI do campo.</span><span class="sxs-lookup"><span data-stu-id="f188b-139">The following XML example shows the FieldURIOrConstant element used with both a constant and field URI.</span></span>
  
```
[xml]
<Restriction>
  <Or xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
    <IsEqualTo>
      <FieldURI FieldURI="item:DateTimeCreated"/>
      <FieldURIOrConstant>
        <FieldURI FieldURI="item:DateTimeReceived"/>
      </FieldURIOrConstant>
    </IsEqualTo>
    <IsEqualTo>
      <FieldURI FieldURI="item:Subject"/>
      <FieldURIOrConstant>
        <Constant Value="Here is a test message"/>
      </FieldURIOrConstant>
    </IsEqualTo>
  </Or>
</Restriction>
```

## <a name="element-information"></a><span data-ttu-id="f188b-140">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f188b-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f188b-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="f188b-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f188b-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f188b-142">Schema Name</span></span>  <br/> |<span data-ttu-id="f188b-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f188b-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="f188b-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f188b-144">Validation File</span></span>  <br/> |<span data-ttu-id="f188b-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f188b-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f188b-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f188b-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="f188b-147">False</span><span class="sxs-lookup"><span data-stu-id="f188b-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f188b-148">Ver também</span><span class="sxs-lookup"><span data-stu-id="f188b-148">See also</span></span>



- [<span data-ttu-id="f188b-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f188b-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

