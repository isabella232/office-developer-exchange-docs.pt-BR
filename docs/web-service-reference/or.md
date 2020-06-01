---
title: Ou
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
description: O elemento or representa uma expressão de pesquisa que executa uma expressão lógica OR na pesquisa que ela contém. Ou retornará true se qualquer um dos seus filhos retornar true. Ou deve ter dois ou mais filhos.
ms.openlocfilehash: 9bc676da5bbaad64f11f6717fb487c2e9bcf2d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462476"
---
# <a name="or"></a><span data-ttu-id="0ffba-105">Ou</span><span class="sxs-lookup"><span data-stu-id="0ffba-105">Or</span></span>

<span data-ttu-id="0ffba-106">O elemento **or** representa uma expressão de pesquisa que executa uma expressão lógica **or** na pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="0ffba-106">The **Or** element represents a search expression that performs a logical **OR** on the search expression that it contains.</span></span> <span data-ttu-id="0ffba-107">**Ou** retornará **true** se qualquer um dos seus filhos retornar **true**.</span><span class="sxs-lookup"><span data-stu-id="0ffba-107">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="0ffba-108">**Ou** deve ter dois ou mais filhos.</span><span class="sxs-lookup"><span data-stu-id="0ffba-108">**Or** must have two or more children.</span></span> 
  
```xml
<Or>
   <SearchExpression/>
   <SearchExpression/>
</Or>
```

 <span data-ttu-id="0ffba-109">**OrType**</span><span class="sxs-lookup"><span data-stu-id="0ffba-109">**OrType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ffba-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0ffba-110">Attributes and elements</span></span>

<span data-ttu-id="0ffba-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0ffba-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ffba-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="0ffba-112">Attributes</span></span>

<span data-ttu-id="0ffba-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ffba-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ffba-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0ffba-114">Child elements</span></span>

|<span data-ttu-id="0ffba-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0ffba-115">**Element**</span></span>|<span data-ttu-id="0ffba-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0ffba-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ffba-117">Pesquisa</span><span class="sxs-lookup"><span data-stu-id="0ffba-117">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="0ffba-118">Representa a classe base para expressões dentro de uma restrição.</span><span class="sxs-lookup"><span data-stu-id="0ffba-118">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="0ffba-119">Um dos seguintes elementos deve ser substituído pelo elemento **searché** :</span><span class="sxs-lookup"><span data-stu-id="0ffba-119">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="0ffba-120">- [Houver](exists.md)</span><span class="sxs-lookup"><span data-stu-id="0ffba-120">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="0ffba-121">- [Exclui](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="0ffba-121">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="0ffba-122">- [IsEqualTo](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="0ffba-122">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="0ffba-123">- [IsNotEqualTo](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="0ffba-123">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="0ffba-124">- [IsGreaterThan](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="0ffba-124">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="0ffba-125">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="0ffba-125">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="0ffba-126">- [IsLessThan](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="0ffba-126">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="0ffba-127">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="0ffba-127">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="0ffba-128">- [Contém](contains.md)</span><span class="sxs-lookup"><span data-stu-id="0ffba-128">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="0ffba-129">- [Sido](not.md)</span><span class="sxs-lookup"><span data-stu-id="0ffba-129">- [Not](not.md)</span></span> <br/><span data-ttu-id="0ffba-130">- [E](and.md)</span><span class="sxs-lookup"><span data-stu-id="0ffba-130">- [And](and.md)</span></span> <br/><span data-ttu-id="0ffba-131">- **Ou**</span><span class="sxs-lookup"><span data-stu-id="0ffba-131">- **Or**</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0ffba-132">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0ffba-132">Parent elements</span></span>

|<span data-ttu-id="0ffba-133">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0ffba-133">**Element**</span></span>|<span data-ttu-id="0ffba-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0ffba-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ffba-135">Restriction</span><span class="sxs-lookup"><span data-stu-id="0ffba-135">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="0ffba-136">Representa a restrição ou a consulta usada para filtrar itens ou pastas no FindItem/FindFolder e operações de pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0ffba-136">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="0ffba-137">Not</span><span class="sxs-lookup"><span data-stu-id="0ffba-137">Not</span></span>](not.md) <br/> |<span data-ttu-id="0ffba-138">Representa uma expressão de pesquisa que nega o valor booliano da expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="0ffba-138">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="0ffba-139">And</span><span class="sxs-lookup"><span data-stu-id="0ffba-139">And</span></span>](and.md) <br/> |<span data-ttu-id="0ffba-140">Representa uma expressão de pesquisa que permite executar um Boolean **e** uma operação entre duas ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0ffba-140">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="0ffba-141">O resultado da operação **and** será **true** se todas as expressões de pesquisa contidas no elemento **e** forem **true**.</span><span class="sxs-lookup"><span data-stu-id="0ffba-141">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|<span data-ttu-id="0ffba-142">**Or**</span><span class="sxs-lookup"><span data-stu-id="0ffba-142">**Or**</span></span> <br/> |<span data-ttu-id="0ffba-143">Representa uma expressão de pesquisa que executa uma operação lógica **ou** na expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="0ffba-143">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="0ffba-144">**Ou** retornará **true** se qualquer um dos seus filhos retornar **true**.</span><span class="sxs-lookup"><span data-stu-id="0ffba-144">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="0ffba-145">**Ou** deve ter dois ou mais filhos.</span><span class="sxs-lookup"><span data-stu-id="0ffba-145">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0ffba-146">Comentários</span><span class="sxs-lookup"><span data-stu-id="0ffba-146">Remarks</span></span>

<span data-ttu-id="0ffba-147">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="0ffba-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ffba-148">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0ffba-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ffba-149">Namespace</span><span class="sxs-lookup"><span data-stu-id="0ffba-149">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0ffba-150">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0ffba-150">Schema Name</span></span>  <br/> |<span data-ttu-id="0ffba-151">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0ffba-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="0ffba-152">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0ffba-152">Validation File</span></span>  <br/> |<span data-ttu-id="0ffba-153">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0ffba-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0ffba-154">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0ffba-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="0ffba-155">False</span><span class="sxs-lookup"><span data-stu-id="0ffba-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ffba-156">Confira também</span><span class="sxs-lookup"><span data-stu-id="0ffba-156">See also</span></span>

- [<span data-ttu-id="0ffba-157">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0ffba-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

