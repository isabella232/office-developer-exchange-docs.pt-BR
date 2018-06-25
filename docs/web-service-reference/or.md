---
title: Or
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Or
api_type:
- schema
ms.assetid: 4876d83a-73a3-4953-9d95-3048e6b76ccb
description: O elemento Or representa uma expressão de pesquisa que realiza um OR lógico a expressão de pesquisa que ele contém. Ou retornará true se qualquer um dos seus filhos retornam true. Ou, deve ter filhos dois ou mais.
ms.openlocfilehash: 46cf031047aeb09e05a385150ab7587968aef345
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824661"
---
# <a name="or"></a><span data-ttu-id="4bac0-105">Or</span><span class="sxs-lookup"><span data-stu-id="4bac0-105">Or</span></span>

<span data-ttu-id="4bac0-106">O elemento **ou** representa uma expressão de pesquisa que realiza uma lógica **ou** a expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="4bac0-106">The **Or** element represents a search expression that performs a logical **OR** on the search expression that it contains.</span></span> <span data-ttu-id="4bac0-107">**Ou** retornará **true** se qualquer um dos seus filhos retornam **true**.</span><span class="sxs-lookup"><span data-stu-id="4bac0-107">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="4bac0-108">**Ou** deve ter dois ou mais filhos.</span><span class="sxs-lookup"><span data-stu-id="4bac0-108">**Or** must have two or more children.</span></span> 
  
```xml
<Or>
   <SearchExpression/>
   <SearchExpression/>
</Or>
```

 <span data-ttu-id="4bac0-109">**OrType**</span><span class="sxs-lookup"><span data-stu-id="4bac0-109">**OrType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4bac0-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4bac0-110">Attributes and elements</span></span>

<span data-ttu-id="4bac0-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4bac0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4bac0-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="4bac0-112">Attributes</span></span>

<span data-ttu-id="4bac0-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4bac0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4bac0-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4bac0-114">Child elements</span></span>

|<span data-ttu-id="4bac0-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4bac0-115">**Element**</span></span>|<span data-ttu-id="4bac0-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4bac0-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4bac0-117">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="4bac0-117">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="4bac0-118">Representa a classe base para expressões dentro de uma restrição.</span><span class="sxs-lookup"><span data-stu-id="4bac0-118">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="4bac0-119">Um dos seguintes elementos deve ser substituído por elemento **SearchExpression** :</span><span class="sxs-lookup"><span data-stu-id="4bac0-119">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="4bac0-120">- [Existe](exists.md)</span><span class="sxs-lookup"><span data-stu-id="4bac0-120">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="4bac0-121">- [Exclui](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="4bac0-121">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="4bac0-122">- [IsEqualTo](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="4bac0-122">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="4bac0-123">- [IsNotEqualTo](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="4bac0-123">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="4bac0-124">- [IsGreaterThan](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="4bac0-124">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="4bac0-125">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="4bac0-125">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="4bac0-126">- [IsLessThan](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="4bac0-126">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="4bac0-127">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="4bac0-127">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="4bac0-128">- [Contém](contains.md)</span><span class="sxs-lookup"><span data-stu-id="4bac0-128">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="4bac0-129">- [Não](not.md)</span><span class="sxs-lookup"><span data-stu-id="4bac0-129">- [Not](not.md)</span></span> <br/><span data-ttu-id="4bac0-130">- [E](and.md)</span><span class="sxs-lookup"><span data-stu-id="4bac0-130">- [And](and.md)</span></span> <br/><span data-ttu-id="4bac0-131">- **Ou**</span><span class="sxs-lookup"><span data-stu-id="4bac0-131">- **Or**</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4bac0-132">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4bac0-132">Parent elements</span></span>

|<span data-ttu-id="4bac0-133">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4bac0-133">**Element**</span></span>|<span data-ttu-id="4bac0-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4bac0-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4bac0-135">Restriction</span><span class="sxs-lookup"><span data-stu-id="4bac0-135">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="4bac0-136">Representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4bac0-136">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="4bac0-137">Não</span><span class="sxs-lookup"><span data-stu-id="4bac0-137">Not</span></span>](not.md) <br/> |<span data-ttu-id="4bac0-138">Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="4bac0-138">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="4bac0-139">E</span><span class="sxs-lookup"><span data-stu-id="4bac0-139">And</span></span>](and.md) <br/> |<span data-ttu-id="4bac0-140">Representa uma expressão de pesquisa que lhe permite realizar uma operação de booleano **e** entre dois ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4bac0-140">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="4bac0-141">O resultado da operação **e** será **true** se todas as expressões de pesquisa contidas no elemento **e** forem **verdadeiras**.</span><span class="sxs-lookup"><span data-stu-id="4bac0-141">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|<span data-ttu-id="4bac0-142">**Ou**</span><span class="sxs-lookup"><span data-stu-id="4bac0-142">**Or**</span></span> <br/> |<span data-ttu-id="4bac0-143">Representa uma expressão de pesquisa que executa uma operação **OR** lógica a expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="4bac0-143">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="4bac0-144">**Ou** retornará **true** se qualquer um dos seus filhos retornam **true**.</span><span class="sxs-lookup"><span data-stu-id="4bac0-144">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="4bac0-145">**Ou** deve ter dois ou mais filhos.</span><span class="sxs-lookup"><span data-stu-id="4bac0-145">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4bac0-146">Comentários</span><span class="sxs-lookup"><span data-stu-id="4bac0-146">Remarks</span></span>

<span data-ttu-id="4bac0-147">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="4bac0-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4bac0-148">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4bac0-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4bac0-149">Namespace</span><span class="sxs-lookup"><span data-stu-id="4bac0-149">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4bac0-150">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4bac0-150">Schema Name</span></span>  <br/> |<span data-ttu-id="4bac0-151">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4bac0-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="4bac0-152">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4bac0-152">Validation File</span></span>  <br/> |<span data-ttu-id="4bac0-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4bac0-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4bac0-154">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4bac0-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="4bac0-155">False</span><span class="sxs-lookup"><span data-stu-id="4bac0-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4bac0-156">Ver também</span><span class="sxs-lookup"><span data-stu-id="4bac0-156">See also</span></span>

- [<span data-ttu-id="4bac0-157">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4bac0-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

