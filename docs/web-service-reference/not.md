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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824553"
---
# <a name="not"></a><span data-ttu-id="f7859-103">Não</span><span class="sxs-lookup"><span data-stu-id="f7859-103">Not</span></span>

<span data-ttu-id="f7859-104">O elemento **não** representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="f7859-104">The **Not** element represents a search expression that negates the Boolean value of the search expression that it contains.</span></span> 
  
```xml
<Not>
   <SearchExpression/>
</Not>
```

 <span data-ttu-id="f7859-105">**NotType**</span><span class="sxs-lookup"><span data-stu-id="f7859-105">**NotType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7859-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f7859-106">Attributes and elements</span></span>

<span data-ttu-id="f7859-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f7859-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7859-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f7859-108">Attributes</span></span>

<span data-ttu-id="f7859-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f7859-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7859-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f7859-110">Child elements</span></span>

|<span data-ttu-id="f7859-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f7859-111">**Element**</span></span>|<span data-ttu-id="f7859-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f7859-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7859-113">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="f7859-113">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="f7859-114">Representa a classe base para expressões dentro de uma restrição.</span><span class="sxs-lookup"><span data-stu-id="f7859-114">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="f7859-115">Um dos seguintes elementos deve ser substituído por elemento **SearchExpression** :</span><span class="sxs-lookup"><span data-stu-id="f7859-115">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="f7859-116">- [Existe](exists.md)</span><span class="sxs-lookup"><span data-stu-id="f7859-116">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="f7859-117">- [Exclui](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="f7859-117">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="f7859-118">- [IsEqualTo](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="f7859-118">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="f7859-119">- [IsNotEqualTo](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="f7859-119">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="f7859-120">- [IsGreaterThan](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="f7859-120">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="f7859-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="f7859-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="f7859-122">- [IsLessThan](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="f7859-122">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="f7859-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="f7859-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="f7859-124">- [Contém](contains.md)</span><span class="sxs-lookup"><span data-stu-id="f7859-124">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="f7859-125">- **Não**</span><span class="sxs-lookup"><span data-stu-id="f7859-125">- **Not**</span></span> <br/><span data-ttu-id="f7859-126">- [E](and.md)</span><span class="sxs-lookup"><span data-stu-id="f7859-126">- [And](and.md)</span></span> <br/><span data-ttu-id="f7859-127">- [Ou](or.md)</span><span class="sxs-lookup"><span data-stu-id="f7859-127">- [Or](or.md)</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f7859-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f7859-128">Parent elements</span></span>

|<span data-ttu-id="f7859-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f7859-129">**Element**</span></span>|<span data-ttu-id="f7859-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f7859-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7859-131">Restriction</span><span class="sxs-lookup"><span data-stu-id="f7859-131">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="f7859-132">Representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="f7859-132">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|<span data-ttu-id="f7859-133">**Não**</span><span class="sxs-lookup"><span data-stu-id="f7859-133">**Not**</span></span> <br/> |<span data-ttu-id="f7859-134">Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="f7859-134">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="f7859-135">E</span><span class="sxs-lookup"><span data-stu-id="f7859-135">And</span></span>](and.md) <br/> |<span data-ttu-id="f7859-136">Representa uma expressão de pesquisa que lhe permite realizar uma operação de booleano **e** entre dois ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="f7859-136">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="f7859-137">O resultado da operação **e** será **true** se todas as expressões de pesquisa contidas no elemento **e** forem **verdadeiras**.</span><span class="sxs-lookup"><span data-stu-id="f7859-137">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="f7859-138">Ou</span><span class="sxs-lookup"><span data-stu-id="f7859-138">Or</span></span>](or.md) <br/> |<span data-ttu-id="f7859-139">Representa uma expressão de pesquisa que executa uma operação **OR** lógica a expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="f7859-139">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="f7859-140">**Ou** retornará **true** se qualquer um dos seus filhos retornam **true**.</span><span class="sxs-lookup"><span data-stu-id="f7859-140">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="f7859-141">**Ou** deve ter dois ou mais filhos.</span><span class="sxs-lookup"><span data-stu-id="f7859-141">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f7859-142">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="f7859-142">Remarks</span></span>

<span data-ttu-id="f7859-143">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f7859-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7859-144">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f7859-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7859-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="f7859-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f7859-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f7859-146">Schema Name</span></span>  <br/> |<span data-ttu-id="f7859-147">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f7859-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="f7859-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f7859-148">Validation File</span></span>  <br/> |<span data-ttu-id="f7859-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f7859-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f7859-150">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f7859-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="f7859-151">False</span><span class="sxs-lookup"><span data-stu-id="f7859-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f7859-152">Ver também</span><span class="sxs-lookup"><span data-stu-id="f7859-152">See also</span></span>

- [<span data-ttu-id="f7859-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f7859-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

