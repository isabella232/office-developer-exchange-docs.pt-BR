---
title: SearchExpression
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
description: O SearchExpression é um elemento abstrato que representa o elemento substituído dentro de uma restrição. Todas as expressões de pesquisa derivam desse tipo de base. Este elemento não é usado em um documento de instância XML.
ms.openlocfilehash: 8e0d09aec079280816cd9dfe2c1a55c88bb959a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825286"
---
# <a name="searchexpression"></a><span data-ttu-id="47965-105">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="47965-105">SearchExpression</span></span>

<span data-ttu-id="47965-106">O **SearchExpression** é um elemento abstrato que representa o elemento substituído dentro de uma restrição.</span><span class="sxs-lookup"><span data-stu-id="47965-106">The **SearchExpression** element is an abstract element that represents the substituted element within a restriction.</span></span> <span data-ttu-id="47965-107">Todas as expressões de pesquisa derivam desse tipo de base.</span><span class="sxs-lookup"><span data-stu-id="47965-107">All search expressions derive from this base type.</span></span> <span data-ttu-id="47965-108">Este elemento não é usado em um documento de instância XML.</span><span class="sxs-lookup"><span data-stu-id="47965-108">This element is not used in an XML instance document.</span></span> 
  
```xml
<SearchExpression/>
```

 <span data-ttu-id="47965-109">**SearchExpressionType**</span><span class="sxs-lookup"><span data-stu-id="47965-109">**SearchExpressionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47965-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="47965-110">Attributes and elements</span></span>

<span data-ttu-id="47965-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="47965-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47965-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="47965-112">Attributes</span></span>

<span data-ttu-id="47965-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="47965-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47965-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="47965-114">Child elements</span></span>

<span data-ttu-id="47965-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="47965-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="47965-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="47965-116">Parent elements</span></span>

|<span data-ttu-id="47965-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="47965-117">**Element**</span></span>|<span data-ttu-id="47965-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47965-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47965-119">Restriction</span><span class="sxs-lookup"><span data-stu-id="47965-119">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="47965-120">Representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="47965-120">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="47965-121">Não</span><span class="sxs-lookup"><span data-stu-id="47965-121">Not</span></span>](not.md) <br/> |<span data-ttu-id="47965-122">Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="47965-122">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="47965-123">E</span><span class="sxs-lookup"><span data-stu-id="47965-123">And</span></span>](and.md) <br/> |<span data-ttu-id="47965-124">Representa uma expressão de pesquisa que lhe permite realizar uma operação de booleano **e** entre dois ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="47965-124">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="47965-125">O resultado da operação **e** será **true** se todas as expressões de pesquisa contidas no elemento **e** forem **verdadeiras**.</span><span class="sxs-lookup"><span data-stu-id="47965-125">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="47965-126">Ou</span><span class="sxs-lookup"><span data-stu-id="47965-126">Or</span></span>](or.md) <br/> |<span data-ttu-id="47965-127">Representa uma expressão de pesquisa que executa uma operação **OR** lógica a expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="47965-127">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="47965-128">**Ou** retornará **true** se qualquer um dos seus filhos retornam **true**.</span><span class="sxs-lookup"><span data-stu-id="47965-128">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="47965-129">**Ou** deve ter dois ou mais filhos.</span><span class="sxs-lookup"><span data-stu-id="47965-129">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="47965-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="47965-130">Remarks</span></span>

<span data-ttu-id="47965-131">Qualquer elemento de filtro que faz parte do grupo de substituição SearchExpression pode aparecer no lugar do elemento SearchExpression.</span><span class="sxs-lookup"><span data-stu-id="47965-131">Any filter element that is part of the SearchExpression substitution group can appear in place of the SearchExpression element.</span></span>
  
> [!NOTE]
> <span data-ttu-id="47965-132">Esse elemento nunca ocorrerá dentro de um documento da instância.</span><span class="sxs-lookup"><span data-stu-id="47965-132">This element will never occur directly within an instance document.</span></span> 
  
<span data-ttu-id="47965-133">Os seguintes elementos são membros do grupo de substituição SearchExpression:</span><span class="sxs-lookup"><span data-stu-id="47965-133">The following elements are members of the SearchExpression substitution group:</span></span>
  
- [<span data-ttu-id="47965-134">Existe</span><span class="sxs-lookup"><span data-stu-id="47965-134">Exists</span></span>](exists.md)
    
- [<span data-ttu-id="47965-135">Exclui</span><span class="sxs-lookup"><span data-stu-id="47965-135">Excludes</span></span>](excludes.md)
    
- [<span data-ttu-id="47965-136">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="47965-136">IsEqualTo</span></span>](isequalto.md)
    
- [<span data-ttu-id="47965-137">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="47965-137">IsNotEqualTo</span></span>](isnotequalto.md)
    
- [<span data-ttu-id="47965-138">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="47965-138">IsGreaterThan</span></span>](isgreaterthan.md)
    
- [<span data-ttu-id="47965-139">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="47965-139">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)
    
- [<span data-ttu-id="47965-140">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="47965-140">IsLessThan</span></span>](islessthan.md)
    
- [<span data-ttu-id="47965-141">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="47965-141">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)
    
- [<span data-ttu-id="47965-142">Contém</span><span class="sxs-lookup"><span data-stu-id="47965-142">Contains</span></span>](contains.md)
    
- [<span data-ttu-id="47965-143">Não</span><span class="sxs-lookup"><span data-stu-id="47965-143">Not</span></span>](not.md)
    
- [<span data-ttu-id="47965-144">E</span><span class="sxs-lookup"><span data-stu-id="47965-144">And</span></span>](and.md)
    
- [<span data-ttu-id="47965-145">Ou</span><span class="sxs-lookup"><span data-stu-id="47965-145">Or</span></span>](or.md)
    
<span data-ttu-id="47965-146">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="47965-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="47965-147">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="47965-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47965-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="47965-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="47965-149">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="47965-149">Schema Name</span></span>  <br/> |<span data-ttu-id="47965-150">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="47965-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="47965-151">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="47965-151">Validation File</span></span>  <br/> |<span data-ttu-id="47965-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="47965-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="47965-153">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="47965-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="47965-154">False</span><span class="sxs-lookup"><span data-stu-id="47965-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47965-155">Ver também</span><span class="sxs-lookup"><span data-stu-id="47965-155">See also</span></span>



- [<span data-ttu-id="47965-156">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="47965-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

