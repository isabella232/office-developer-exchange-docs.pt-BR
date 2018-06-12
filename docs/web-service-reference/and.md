---
title: And
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- And
api_type:
- schema
ms.assetid: 790246c2-37ad-49a8-91b9-6186d743b011
description: O elemento And representa uma expressão de pesquisa que permite realizar uma operação Boolean e entre dois ou mais expressões de pesquisa. O resultado da operação e será true se todas as expressões de pesquisa contidas no elemento And forem verdadeiras.
ms.openlocfilehash: d287d57d68aeca7127325dc8fb65fd0190e5b5eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751091"
---
# <a name="and"></a><span data-ttu-id="825d1-104">And</span><span class="sxs-lookup"><span data-stu-id="825d1-104">And</span></span>

<span data-ttu-id="825d1-105">O elemento **e** representa uma expressão de pesquisa que lhe permite realizar uma operação de booleano **e** entre dois ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="825d1-105">The **And** element represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="825d1-106">O resultado da operação **e** será **true** se todas as expressões de pesquisa contidas no elemento **e** forem **verdadeiras**.</span><span class="sxs-lookup"><span data-stu-id="825d1-106">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>
  
```xml
<And>
   <SearchExpression/>
   <SearchExpression/>
</And>
```

 <span data-ttu-id="825d1-107">**AndType**</span><span class="sxs-lookup"><span data-stu-id="825d1-107">**AndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="825d1-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="825d1-108">Attributes and elements</span></span>

<span data-ttu-id="825d1-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="825d1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="825d1-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="825d1-110">Attributes</span></span>

<span data-ttu-id="825d1-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="825d1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="825d1-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="825d1-112">Child elements</span></span>

|<span data-ttu-id="825d1-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="825d1-113">**Element**</span></span>|<span data-ttu-id="825d1-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="825d1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="825d1-115">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="825d1-115">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="825d1-116">Representa a classe base para expressões dentro de uma restrição.</span><span class="sxs-lookup"><span data-stu-id="825d1-116">Represents the base class for expressions within a restriction.</span></span> <span data-ttu-id="825d1-117">Deve haver dois ou mais expressões de pesquisa em uma operação And.</span><span class="sxs-lookup"><span data-stu-id="825d1-117">There must be two or more search expressions in an And operation.</span></span><br/><br/>  <span data-ttu-id="825d1-118">Um dos seguintes elementos deve ser substituído por elemento **SearchExpression** :</span><span class="sxs-lookup"><span data-stu-id="825d1-118">One of the following elements must be substituted for the **SearchExpression** element:</span></span><ul><li> [<span data-ttu-id="825d1-119">Existe</span><span class="sxs-lookup"><span data-stu-id="825d1-119">Exists</span></span>](exists.md)</li><li>[<span data-ttu-id="825d1-120">Exclui</span><span class="sxs-lookup"><span data-stu-id="825d1-120">Excludes</span></span>](excludes.md)</li><li>[<span data-ttu-id="825d1-121">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="825d1-121">IsEqualTo</span></span>](isequalto.md)</li><li>[<span data-ttu-id="825d1-122">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="825d1-122">IsNotEqualTo</span></span>](isnotequalto.md)</li><li>[<span data-ttu-id="825d1-123">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="825d1-123">IsGreaterThan</span></span>](isgreaterthan.md)</li><li>[<span data-ttu-id="825d1-124">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="825d1-124">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)</li><li>[<span data-ttu-id="825d1-125">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="825d1-125">IsLessThan</span></span>](islessthan.md)</li><li>[<span data-ttu-id="825d1-126">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="825d1-126">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)</li><li>[<span data-ttu-id="825d1-127">Contém</span><span class="sxs-lookup"><span data-stu-id="825d1-127">Contains</span></span>](contains.md)</li><li>[<span data-ttu-id="825d1-128">Não</span><span class="sxs-lookup"><span data-stu-id="825d1-128">Not</span></span>](not.md)</li><li><span data-ttu-id="825d1-129">**E**</span><span class="sxs-lookup"><span data-stu-id="825d1-129">**And**</span></span></li><li>[<span data-ttu-id="825d1-130">Ou</span><span class="sxs-lookup"><span data-stu-id="825d1-130">Or</span></span>](or.md) </li></ul> |
   
### <a name="parent-elements"></a><span data-ttu-id="825d1-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="825d1-131">Parent elements</span></span>

|<span data-ttu-id="825d1-132">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="825d1-132">**Element**</span></span>|<span data-ttu-id="825d1-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="825d1-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="825d1-134">Restriction</span><span class="sxs-lookup"><span data-stu-id="825d1-134">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="825d1-135">Representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="825d1-135">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="825d1-136">Não</span><span class="sxs-lookup"><span data-stu-id="825d1-136">Not</span></span>](not.md) <br/> |<span data-ttu-id="825d1-137">Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="825d1-137">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|<span data-ttu-id="825d1-138">**E**</span><span class="sxs-lookup"><span data-stu-id="825d1-138">**And**</span></span> <br/> |<span data-ttu-id="825d1-139">Representa uma expressão de pesquisa que lhe permite realizar uma operação de booleano **e** entre dois ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="825d1-139">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="825d1-140">O resultado da operação **e** será **true** se todas as expressões de pesquisa contidas no elemento **e** forem **verdadeiras**.</span><span class="sxs-lookup"><span data-stu-id="825d1-140">The result of the **AND** operation is **true** if all of the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="825d1-141">Ou</span><span class="sxs-lookup"><span data-stu-id="825d1-141">Or</span></span>](or.md) <br/> |<span data-ttu-id="825d1-142">Representa uma expressão de pesquisa que executa uma operação **OR** lógica a expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="825d1-142">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="825d1-143">**Ou** retornará **true** se qualquer um dos seus filhos retornam **true**.</span><span class="sxs-lookup"><span data-stu-id="825d1-143">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="825d1-144">**Ou** deve ter dois ou mais filhos.</span><span class="sxs-lookup"><span data-stu-id="825d1-144">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="825d1-145">Comentários</span><span class="sxs-lookup"><span data-stu-id="825d1-145">Remarks</span></span>

<span data-ttu-id="825d1-146">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="825d1-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="825d1-147">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="825d1-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="825d1-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="825d1-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="825d1-149">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="825d1-149">Schema Name</span></span>  <br/> |<span data-ttu-id="825d1-150">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="825d1-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="825d1-151">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="825d1-151">Validation File</span></span>  <br/> |<span data-ttu-id="825d1-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="825d1-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="825d1-153">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="825d1-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="825d1-154">False</span><span class="sxs-lookup"><span data-stu-id="825d1-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="825d1-155">Ver também</span><span class="sxs-lookup"><span data-stu-id="825d1-155">See also</span></span>

- [<span data-ttu-id="825d1-156">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="825d1-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

