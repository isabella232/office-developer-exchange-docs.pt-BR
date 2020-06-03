---
title: Pesquisa
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchExpression
api_type:
- schema
ms.assetid: daa179b6-8c7f-4268-a312-c2acc67fa7c3
description: O elemento Searché é um elemento abstract que representa o elemento substituído dentro de uma restrição. Todas as expressões de pesquisa derivam desse tipo base. Esse elemento não é usado em um documento de instância XML.
ms.openlocfilehash: db06ce8e2faa0f2589963d58aab55073c618c171
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530349"
---
# <a name="searchexpression"></a><span data-ttu-id="5ea01-105">Pesquisa</span><span class="sxs-lookup"><span data-stu-id="5ea01-105">SearchExpression</span></span>

<span data-ttu-id="5ea01-106">O elemento **searché** é um elemento abstract que representa o elemento substituído dentro de uma restrição.</span><span class="sxs-lookup"><span data-stu-id="5ea01-106">The **SearchExpression** element is an abstract element that represents the substituted element within a restriction.</span></span> <span data-ttu-id="5ea01-107">Todas as expressões de pesquisa derivam desse tipo base.</span><span class="sxs-lookup"><span data-stu-id="5ea01-107">All search expressions derive from this base type.</span></span> <span data-ttu-id="5ea01-108">Esse elemento não é usado em um documento de instância XML.</span><span class="sxs-lookup"><span data-stu-id="5ea01-108">This element is not used in an XML instance document.</span></span> 
  
```xml
<SearchExpression/>
```

 <span data-ttu-id="5ea01-109">**SearchExpressionType**</span><span class="sxs-lookup"><span data-stu-id="5ea01-109">**SearchExpressionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ea01-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5ea01-110">Attributes and elements</span></span>

<span data-ttu-id="5ea01-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5ea01-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ea01-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="5ea01-112">Attributes</span></span>

<span data-ttu-id="5ea01-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5ea01-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5ea01-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5ea01-114">Child elements</span></span>

<span data-ttu-id="5ea01-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5ea01-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5ea01-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5ea01-116">Parent elements</span></span>

|<span data-ttu-id="5ea01-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5ea01-117">**Element**</span></span>|<span data-ttu-id="5ea01-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5ea01-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ea01-119">Restriction</span><span class="sxs-lookup"><span data-stu-id="5ea01-119">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="5ea01-120">Representa a restrição ou a consulta usada para filtrar itens ou pastas no FindItem/FindFolder e operações de pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="5ea01-120">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="5ea01-121">Not</span><span class="sxs-lookup"><span data-stu-id="5ea01-121">Not</span></span>](not.md) <br/> |<span data-ttu-id="5ea01-122">Representa uma expressão de pesquisa que nega o valor booliano da expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="5ea01-122">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="5ea01-123">And</span><span class="sxs-lookup"><span data-stu-id="5ea01-123">And</span></span>](and.md) <br/> |<span data-ttu-id="5ea01-124">Representa uma expressão de pesquisa que permite executar um Boolean **e** uma operação entre duas ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="5ea01-124">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="5ea01-125">O resultado da operação **and** será **true** se todas as expressões de pesquisa contidas no elemento **e** forem **true**.</span><span class="sxs-lookup"><span data-stu-id="5ea01-125">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="5ea01-126">Or</span><span class="sxs-lookup"><span data-stu-id="5ea01-126">Or</span></span>](or.md) <br/> |<span data-ttu-id="5ea01-127">Representa uma expressão de pesquisa que executa uma operação lógica **ou** na expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="5ea01-127">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="5ea01-128">**Ou** retornará **true** se qualquer um dos seus filhos retornar **true**.</span><span class="sxs-lookup"><span data-stu-id="5ea01-128">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="5ea01-129">**Ou** deve ter dois ou mais filhos.</span><span class="sxs-lookup"><span data-stu-id="5ea01-129">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5ea01-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="5ea01-130">Remarks</span></span>

<span data-ttu-id="5ea01-131">Qualquer elemento Filter que faz parte do grupo de substituição Searché pode aparecer no lugar do elemento Searché.</span><span class="sxs-lookup"><span data-stu-id="5ea01-131">Any filter element that is part of the SearchExpression substitution group can appear in place of the SearchExpression element.</span></span>
  
> [!NOTE]
> <span data-ttu-id="5ea01-132">Esse elemento nunca ocorrerá diretamente em um documento de instância.</span><span class="sxs-lookup"><span data-stu-id="5ea01-132">This element will never occur directly within an instance document.</span></span> 
  
<span data-ttu-id="5ea01-133">Os seguintes elementos são membros do grupo de substituição de SearchParameters:</span><span class="sxs-lookup"><span data-stu-id="5ea01-133">The following elements are members of the SearchExpression substitution group:</span></span>
  
- [<span data-ttu-id="5ea01-134">Existe</span><span class="sxs-lookup"><span data-stu-id="5ea01-134">Exists</span></span>](exists.md)
    
- [<span data-ttu-id="5ea01-135">Exclui</span><span class="sxs-lookup"><span data-stu-id="5ea01-135">Excludes</span></span>](excludes.md)
    
- [<span data-ttu-id="5ea01-136">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="5ea01-136">IsEqualTo</span></span>](isequalto.md)
    
- [<span data-ttu-id="5ea01-137">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="5ea01-137">IsNotEqualTo</span></span>](isnotequalto.md)
    
- [<span data-ttu-id="5ea01-138">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="5ea01-138">IsGreaterThan</span></span>](isgreaterthan.md)
    
- [<span data-ttu-id="5ea01-139">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="5ea01-139">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)
    
- [<span data-ttu-id="5ea01-140">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="5ea01-140">IsLessThan</span></span>](islessthan.md)
    
- [<span data-ttu-id="5ea01-141">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="5ea01-141">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)
    
- [<span data-ttu-id="5ea01-142">Contém</span><span class="sxs-lookup"><span data-stu-id="5ea01-142">Contains</span></span>](contains.md)
    
- [<span data-ttu-id="5ea01-143">Not</span><span class="sxs-lookup"><span data-stu-id="5ea01-143">Not</span></span>](not.md)
    
- [<span data-ttu-id="5ea01-144">And</span><span class="sxs-lookup"><span data-stu-id="5ea01-144">And</span></span>](and.md)
    
- [<span data-ttu-id="5ea01-145">Or</span><span class="sxs-lookup"><span data-stu-id="5ea01-145">Or</span></span>](or.md)
    
<span data-ttu-id="5ea01-146">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="5ea01-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ea01-147">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5ea01-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ea01-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="5ea01-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5ea01-149">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5ea01-149">Schema Name</span></span>  <br/> |<span data-ttu-id="5ea01-150">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5ea01-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="5ea01-151">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5ea01-151">Validation File</span></span>  <br/> |<span data-ttu-id="5ea01-152">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5ea01-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5ea01-153">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5ea01-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="5ea01-154">False</span><span class="sxs-lookup"><span data-stu-id="5ea01-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ea01-155">Confira também</span><span class="sxs-lookup"><span data-stu-id="5ea01-155">See also</span></span>



- [<span data-ttu-id="5ea01-156">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5ea01-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

