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
description: O elemento e representa uma expressão de pesquisa que permite executar um Boolean e uma operação entre duas ou mais expressões de pesquisa. O resultado da operação AND será true se todas as expressões de pesquisa contidas no elemento e forem true.
ms.openlocfilehash: f5239f19c2b5a931eefa9ff4a9dd8ed9d775bae2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464718"
---
# <a name="and"></a><span data-ttu-id="85e0f-104">And</span><span class="sxs-lookup"><span data-stu-id="85e0f-104">And</span></span>

<span data-ttu-id="85e0f-105">O elemento **e** representa uma expressão de pesquisa que permite executar um Boolean **e** uma operação entre duas ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="85e0f-105">The **And** element represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="85e0f-106">O resultado da operação **and** será **true** se todas as expressões de pesquisa contidas no elemento **e** forem **true**.</span><span class="sxs-lookup"><span data-stu-id="85e0f-106">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>
  
```xml
<And>
   <SearchExpression/>
   <SearchExpression/>
</And>
```

 <span data-ttu-id="85e0f-107">**AndType**</span><span class="sxs-lookup"><span data-stu-id="85e0f-107">**AndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85e0f-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="85e0f-108">Attributes and elements</span></span>

<span data-ttu-id="85e0f-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="85e0f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85e0f-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="85e0f-110">Attributes</span></span>

<span data-ttu-id="85e0f-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="85e0f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85e0f-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="85e0f-112">Child elements</span></span>

|<span data-ttu-id="85e0f-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="85e0f-113">**Element**</span></span>|<span data-ttu-id="85e0f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="85e0f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85e0f-115">Pesquisa</span><span class="sxs-lookup"><span data-stu-id="85e0f-115">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="85e0f-116">Representa a classe base para expressões dentro de uma restrição.</span><span class="sxs-lookup"><span data-stu-id="85e0f-116">Represents the base class for expressions within a restriction.</span></span> <span data-ttu-id="85e0f-117">Deve haver duas ou mais expressões de pesquisa em uma operação and.</span><span class="sxs-lookup"><span data-stu-id="85e0f-117">There must be two or more search expressions in an And operation.</span></span><br/><br/>  <span data-ttu-id="85e0f-118">Um dos seguintes elementos deve ser substituído pelo elemento **searché** :</span><span class="sxs-lookup"><span data-stu-id="85e0f-118">One of the following elements must be substituted for the **SearchExpression** element:</span></span><ul><li> [<span data-ttu-id="85e0f-119">Existe</span><span class="sxs-lookup"><span data-stu-id="85e0f-119">Exists</span></span>](exists.md)</li><li>[<span data-ttu-id="85e0f-120">Exclui</span><span class="sxs-lookup"><span data-stu-id="85e0f-120">Excludes</span></span>](excludes.md)</li><li>[<span data-ttu-id="85e0f-121">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="85e0f-121">IsEqualTo</span></span>](isequalto.md)</li><li>[<span data-ttu-id="85e0f-122">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="85e0f-122">IsNotEqualTo</span></span>](isnotequalto.md)</li><li>[<span data-ttu-id="85e0f-123">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="85e0f-123">IsGreaterThan</span></span>](isgreaterthan.md)</li><li>[<span data-ttu-id="85e0f-124">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="85e0f-124">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)</li><li>[<span data-ttu-id="85e0f-125">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="85e0f-125">IsLessThan</span></span>](islessthan.md)</li><li>[<span data-ttu-id="85e0f-126">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="85e0f-126">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)</li><li>[<span data-ttu-id="85e0f-127">Contém</span><span class="sxs-lookup"><span data-stu-id="85e0f-127">Contains</span></span>](contains.md)</li><li>[<span data-ttu-id="85e0f-128">Not</span><span class="sxs-lookup"><span data-stu-id="85e0f-128">Not</span></span>](not.md)</li><li><span data-ttu-id="85e0f-129">**And**</span><span class="sxs-lookup"><span data-stu-id="85e0f-129">**And**</span></span></li><li>[<span data-ttu-id="85e0f-130">Or</span><span class="sxs-lookup"><span data-stu-id="85e0f-130">Or</span></span>](or.md) </li></ul> |
   
### <a name="parent-elements"></a><span data-ttu-id="85e0f-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="85e0f-131">Parent elements</span></span>

|<span data-ttu-id="85e0f-132">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="85e0f-132">**Element**</span></span>|<span data-ttu-id="85e0f-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="85e0f-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85e0f-134">Restriction</span><span class="sxs-lookup"><span data-stu-id="85e0f-134">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="85e0f-135">Representa a restrição ou a consulta usada para filtrar itens ou pastas no FindItem/FindFolder e operações de pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="85e0f-135">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="85e0f-136">Not</span><span class="sxs-lookup"><span data-stu-id="85e0f-136">Not</span></span>](not.md) <br/> |<span data-ttu-id="85e0f-137">Representa uma expressão de pesquisa que nega o valor booliano da expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="85e0f-137">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|<span data-ttu-id="85e0f-138">**And**</span><span class="sxs-lookup"><span data-stu-id="85e0f-138">**And**</span></span> <br/> |<span data-ttu-id="85e0f-139">Representa uma expressão de pesquisa que permite executar um Boolean **e** uma operação entre duas ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="85e0f-139">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="85e0f-140">O resultado da operação **and** será **true** se todas as expressões de pesquisa contidas no elemento **e** forem **true**.</span><span class="sxs-lookup"><span data-stu-id="85e0f-140">The result of the **AND** operation is **true** if all of the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="85e0f-141">Or</span><span class="sxs-lookup"><span data-stu-id="85e0f-141">Or</span></span>](or.md) <br/> |<span data-ttu-id="85e0f-142">Representa uma expressão de pesquisa que executa uma operação lógica **ou** na expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="85e0f-142">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="85e0f-143">**Ou** retornará **true** se qualquer um dos seus filhos retornar **true**.</span><span class="sxs-lookup"><span data-stu-id="85e0f-143">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="85e0f-144">**Ou** deve ter dois ou mais filhos.</span><span class="sxs-lookup"><span data-stu-id="85e0f-144">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="85e0f-145">Comentários</span><span class="sxs-lookup"><span data-stu-id="85e0f-145">Remarks</span></span>

<span data-ttu-id="85e0f-146">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="85e0f-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85e0f-147">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="85e0f-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85e0f-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="85e0f-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85e0f-149">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="85e0f-149">Schema Name</span></span>  <br/> |<span data-ttu-id="85e0f-150">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="85e0f-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="85e0f-151">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="85e0f-151">Validation File</span></span>  <br/> |<span data-ttu-id="85e0f-152">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="85e0f-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85e0f-153">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="85e0f-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="85e0f-154">False</span><span class="sxs-lookup"><span data-stu-id="85e0f-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85e0f-155">Confira também</span><span class="sxs-lookup"><span data-stu-id="85e0f-155">See also</span></span>

- [<span data-ttu-id="85e0f-156">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="85e0f-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

