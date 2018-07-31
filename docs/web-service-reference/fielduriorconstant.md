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
ms.openlocfilehash: a24c2fa044e03d0ac6f900625e325600903df8d0
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354222"
---
# <a name="fielduriorconstant"></a><span data-ttu-id="90aa5-103">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="90aa5-103">FieldURIOrConstant</span></span>

<span data-ttu-id="90aa5-104">O elemento **FieldURIOrConstant** representa uma propriedade ou um valor de constante a ser usado ao comparar com outra propriedade.</span><span class="sxs-lookup"><span data-stu-id="90aa5-104">The **FieldURIOrConstant** element represents either a property or a constant value to be used when comparing with another property.</span></span> 
  
```xml
<FieldURIOrConstant>
   <Constant/>
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
    <IndexedFieldURI/> 
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
   <FieldURI/>
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
   <ExtendedFieldURI/> 
</FieldURIOrConstant>
```

<span data-ttu-id="90aa5-105">**FieldURIOrConstantType**</span><span class="sxs-lookup"><span data-stu-id="90aa5-105">**FieldURIOrConstantType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="90aa5-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="90aa5-106">Attributes and elements</span></span>

<span data-ttu-id="90aa5-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="90aa5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90aa5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="90aa5-108">Attributes</span></span>

<span data-ttu-id="90aa5-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="90aa5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90aa5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="90aa5-110">Child elements</span></span>

|<span data-ttu-id="90aa5-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="90aa5-111">**Element**</span></span>|<span data-ttu-id="90aa5-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90aa5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90aa5-113">Constante</span><span class="sxs-lookup"><span data-stu-id="90aa5-113">Constant</span></span>](constant.md) <br/> |<span data-ttu-id="90aa5-114">Identifica um valor de constante em uma restrição.</span><span class="sxs-lookup"><span data-stu-id="90aa5-114">Identifies a constant value in a restriction.</span></span>  <br/> |
|[<span data-ttu-id="90aa5-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="90aa5-115">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="90aa5-116">Identifica as propriedades frequentemente referenciadas pelo URI.</span><span class="sxs-lookup"><span data-stu-id="90aa5-116">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="90aa5-117">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="90aa5-117">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="90aa5-118">Identifica a membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="90aa5-118">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="90aa5-119">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="90aa5-119">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="90aa5-120">Identifica as propriedades MAPI.</span><span class="sxs-lookup"><span data-stu-id="90aa5-120">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90aa5-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="90aa5-121">Parent elements</span></span>

|<span data-ttu-id="90aa5-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="90aa5-122">**Element**</span></span>|<span data-ttu-id="90aa5-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90aa5-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90aa5-124">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="90aa5-124">IsEqualTo</span></span>](isequalto.md) <br/> |<span data-ttu-id="90aa5-125">Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retornará true se eles forem iguais.</span><span class="sxs-lookup"><span data-stu-id="90aa5-125">Represents a search expression that compares a property with either a constant value or another property and evaluates to true if they are equal.</span></span>  <br/> |
|[<span data-ttu-id="90aa5-126">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="90aa5-126">IsGreaterThan</span></span>](isgreaterthan.md) <br/> |<span data-ttu-id="90aa5-127">Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se a primeira propriedade for maior.</span><span class="sxs-lookup"><span data-stu-id="90aa5-127">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is greater.</span></span>  <br/> |
|[<span data-ttu-id="90aa5-128">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="90aa5-128">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md) <br/> |<span data-ttu-id="90aa5-129">Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se a primeira propriedade for maior que ou igual ao segundo valor ou propriedade.</span><span class="sxs-lookup"><span data-stu-id="90aa5-129">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is greater than or equal to the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="90aa5-130">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="90aa5-130">IsLessThan</span></span>](islessthan.md) <br/> |<span data-ttu-id="90aa5-131">Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se a primeira propriedade for menor que o segundo valor ou a propriedade.</span><span class="sxs-lookup"><span data-stu-id="90aa5-131">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is less than the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="90aa5-132">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="90aa5-132">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md) <br/> |<span data-ttu-id="90aa5-133">Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se a primeira propriedade for menor ou igual ao segundo valor ou propriedade.</span><span class="sxs-lookup"><span data-stu-id="90aa5-133">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is less than or equal to the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="90aa5-134">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="90aa5-134">IsNotEqualTo</span></span>](isnotequalto.md) <br/> |<span data-ttu-id="90aa5-135">Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se os valores não são iguais.</span><span class="sxs-lookup"><span data-stu-id="90aa5-135">Represents a search expression that compares a property with either a constant value or another property and returns true if the values are not the same.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="90aa5-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="90aa5-136">Remarks</span></span>

<span data-ttu-id="90aa5-137">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="90aa5-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="90aa5-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90aa5-138">Example</span></span>

<span data-ttu-id="90aa5-139">O exemplo XML a seguir mostra o elemento FieldURIOrConstant usado com uma constante e o URI do campo.</span><span class="sxs-lookup"><span data-stu-id="90aa5-139">The following XML example shows the FieldURIOrConstant element used with both a constant and field URI.</span></span>
  
```xml
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

## <a name="element-information"></a><span data-ttu-id="90aa5-140">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="90aa5-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90aa5-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="90aa5-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="90aa5-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="90aa5-142">Schema Name</span></span>  <br/> |<span data-ttu-id="90aa5-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="90aa5-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="90aa5-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="90aa5-144">Validation File</span></span>  <br/> |<span data-ttu-id="90aa5-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="90aa5-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="90aa5-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="90aa5-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="90aa5-147">False</span><span class="sxs-lookup"><span data-stu-id="90aa5-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90aa5-148">Ver também</span><span class="sxs-lookup"><span data-stu-id="90aa5-148">See also</span></span>

- [<span data-ttu-id="90aa5-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="90aa5-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

