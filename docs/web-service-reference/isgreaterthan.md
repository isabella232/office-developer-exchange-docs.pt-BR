---
title: IsGreaterThan
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsGreaterThan
api_type:
- schema
ms.assetid: a6e9d462-cfa7-40ec-903e-128c95050352
description: O elemento IsGreaterThan representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna true se a primeira propriedade é maior.
ms.openlocfilehash: 52f2c1b84e4072649092637de091c0dbd8187032
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530040"
---
# <a name="isgreaterthan"></a><span data-ttu-id="00142-103">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="00142-103">IsGreaterThan</span></span>

<span data-ttu-id="00142-104">O elemento **IsGreaterThan** representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se a primeira propriedade é maior.</span><span class="sxs-lookup"><span data-stu-id="00142-104">The **IsGreaterThan** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater.</span></span> 
  
```xml
<IsGreaterThan>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsGreaterThan>
```

```xml
<IsGreaterThan>
   <IndexedFieldURI/> 
   <FieldURIOrConstant/>
</IsGreaterThan>
```

```xml
<IsGreaterThan>
   <ExtendedFieldURI/>
   <FieldURIOrConstant/>
</IsGreaterThan>
```

<span data-ttu-id="00142-105">**IsGreaterThanType**</span><span class="sxs-lookup"><span data-stu-id="00142-105">**IsGreaterThanType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="00142-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="00142-106">Attributes and elements</span></span>

<span data-ttu-id="00142-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="00142-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00142-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="00142-108">Attributes</span></span>

<span data-ttu-id="00142-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="00142-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00142-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="00142-110">Child elements</span></span>

|<span data-ttu-id="00142-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="00142-111">**Element**</span></span>|<span data-ttu-id="00142-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="00142-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00142-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="00142-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="00142-114">Identifica as propriedades com frequência referenciadas por URI.</span><span class="sxs-lookup"><span data-stu-id="00142-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="00142-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="00142-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="00142-116">Identifica membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="00142-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="00142-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="00142-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="00142-118">Identifica as propriedades MAPI.</span><span class="sxs-lookup"><span data-stu-id="00142-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="00142-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="00142-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="00142-120">Representa uma propriedade ou um valor de constante a ser usado ao comparar com outra propriedade.</span><span class="sxs-lookup"><span data-stu-id="00142-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00142-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="00142-121">Parent elements</span></span>

|<span data-ttu-id="00142-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="00142-122">**Element**</span></span>|<span data-ttu-id="00142-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="00142-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00142-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="00142-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="00142-125">Representa a restrição ou a consulta usada para filtrar itens ou pastas no FindItem/FindFolder e operações de pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="00142-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="00142-126">Not</span><span class="sxs-lookup"><span data-stu-id="00142-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="00142-127">Representa uma expressão de pesquisa que nega o valor booliano da expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="00142-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="00142-128">And</span><span class="sxs-lookup"><span data-stu-id="00142-128">And</span></span>](and.md) <br/> |<span data-ttu-id="00142-129">Representa uma expressão de pesquisa que permite que você execute um Boolean e uma operação entre duas ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="00142-129">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="00142-130">O resultado da operação and será **true** se todas as expressões de pesquisa contidas no e forem **true**.</span><span class="sxs-lookup"><span data-stu-id="00142-130">The result of the And operation is **true** if all the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="00142-131">Or</span><span class="sxs-lookup"><span data-stu-id="00142-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="00142-132">Representa uma expressão de pesquisa que executa uma expressão lógica ou na expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="00142-132">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="00142-133">[Ou](or.md) retornará **true** se qualquer um dos seus filhos retornar **true**.</span><span class="sxs-lookup"><span data-stu-id="00142-133">[Or](or.md) will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="00142-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="00142-134">Remarks</span></span>

<span data-ttu-id="00142-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="00142-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00142-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="00142-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00142-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="00142-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="00142-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="00142-138">Schema Name</span></span>  <br/> |<span data-ttu-id="00142-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="00142-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="00142-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="00142-140">Validation File</span></span>  <br/> |<span data-ttu-id="00142-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="00142-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="00142-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="00142-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="00142-143">False</span><span class="sxs-lookup"><span data-stu-id="00142-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00142-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="00142-144">See also</span></span>

- [<span data-ttu-id="00142-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="00142-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

