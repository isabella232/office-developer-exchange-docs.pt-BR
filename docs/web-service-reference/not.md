---
title: Não
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Not
api_type:
- schema
ms.assetid: 1aa16318-7e90-4b19-bce8-dd1a20a66223
description: O elemento não representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.
ms.openlocfilehash: f5bc709d8b1e77a13b3598905651ac1750436f03
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824553"
---
# <a name="not"></a><span data-ttu-id="c2a5d-103">Não</span><span class="sxs-lookup"><span data-stu-id="c2a5d-103">Not</span></span>

<span data-ttu-id="c2a5d-104">O elemento **não** representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="c2a5d-104">The **Not** element represents a search expression that negates the Boolean value of the search expression that it contains.</span></span> 
  
```xml
<Not>
   <SearchExpression/>
</Not>
```

 <span data-ttu-id="c2a5d-105">**NotType**</span><span class="sxs-lookup"><span data-stu-id="c2a5d-105">**NotType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2a5d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c2a5d-106">Attributes and elements</span></span>

<span data-ttu-id="c2a5d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c2a5d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2a5d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c2a5d-108">Attributes</span></span>

<span data-ttu-id="c2a5d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c2a5d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2a5d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c2a5d-110">Child elements</span></span>

|<span data-ttu-id="c2a5d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c2a5d-111">**Element**</span></span>|<span data-ttu-id="c2a5d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c2a5d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2a5d-113">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="c2a5d-113">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="c2a5d-114">Representa a classe base para expressões dentro de uma restrição.</span><span class="sxs-lookup"><span data-stu-id="c2a5d-114">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="c2a5d-115">Um dos seguintes elementos deve ser substituído por elemento **SearchExpression** :</span><span class="sxs-lookup"><span data-stu-id="c2a5d-115">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="c2a5d-116">- [Existe](exists.md)</span><span class="sxs-lookup"><span data-stu-id="c2a5d-116">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="c2a5d-117">- [Exclui](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="c2a5d-117">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="c2a5d-118">- [IsEqualTo](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="c2a5d-118">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="c2a5d-119">- [IsNotEqualTo](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="c2a5d-119">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="c2a5d-120">- [IsGreaterThan](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="c2a5d-120">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="c2a5d-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="c2a5d-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="c2a5d-122">- [IsLessThan](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="c2a5d-122">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="c2a5d-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="c2a5d-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="c2a5d-124">- [Contém](contains.md)</span><span class="sxs-lookup"><span data-stu-id="c2a5d-124">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="c2a5d-125">- **Não**</span><span class="sxs-lookup"><span data-stu-id="c2a5d-125">- **Not**</span></span> <br/><span data-ttu-id="c2a5d-126">- [E](and.md)</span><span class="sxs-lookup"><span data-stu-id="c2a5d-126">- [And](and.md)</span></span> <br/><span data-ttu-id="c2a5d-127">- [Ou](or.md)</span><span class="sxs-lookup"><span data-stu-id="c2a5d-127">- [Or](or.md)</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c2a5d-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c2a5d-128">Parent elements</span></span>

|<span data-ttu-id="c2a5d-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c2a5d-129">**Element**</span></span>|<span data-ttu-id="c2a5d-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c2a5d-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2a5d-131">Restriction</span><span class="sxs-lookup"><span data-stu-id="c2a5d-131">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="c2a5d-132">Representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c2a5d-132">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|<span data-ttu-id="c2a5d-133">**Não**</span><span class="sxs-lookup"><span data-stu-id="c2a5d-133">**Not**</span></span> <br/> |<span data-ttu-id="c2a5d-134">Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="c2a5d-134">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="c2a5d-135">E</span><span class="sxs-lookup"><span data-stu-id="c2a5d-135">And</span></span>](and.md) <br/> |<span data-ttu-id="c2a5d-136">Representa uma expressão de pesquisa que lhe permite realizar uma operação de booleano **e** entre dois ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c2a5d-136">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="c2a5d-137">O resultado da operação **e** será **true** se todas as expressões de pesquisa contidas no elemento **e** forem **verdadeiras**.</span><span class="sxs-lookup"><span data-stu-id="c2a5d-137">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="c2a5d-138">Ou</span><span class="sxs-lookup"><span data-stu-id="c2a5d-138">Or</span></span>](or.md) <br/> |<span data-ttu-id="c2a5d-139">Representa uma expressão de pesquisa que executa uma operação **OR** lógica a expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="c2a5d-139">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="c2a5d-140">**Ou** retornará **true** se qualquer um dos seus filhos retornam **true**.</span><span class="sxs-lookup"><span data-stu-id="c2a5d-140">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="c2a5d-141">**Ou** deve ter dois ou mais filhos.</span><span class="sxs-lookup"><span data-stu-id="c2a5d-141">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c2a5d-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="c2a5d-142">Remarks</span></span>

<span data-ttu-id="c2a5d-143">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="c2a5d-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2a5d-144">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c2a5d-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2a5d-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="c2a5d-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c2a5d-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c2a5d-146">Schema Name</span></span>  <br/> |<span data-ttu-id="c2a5d-147">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c2a5d-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="c2a5d-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c2a5d-148">Validation File</span></span>  <br/> |<span data-ttu-id="c2a5d-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c2a5d-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c2a5d-150">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c2a5d-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2a5d-151">False</span><span class="sxs-lookup"><span data-stu-id="c2a5d-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2a5d-152">Ver também</span><span class="sxs-lookup"><span data-stu-id="c2a5d-152">See also</span></span>

- [<span data-ttu-id="c2a5d-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c2a5d-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

