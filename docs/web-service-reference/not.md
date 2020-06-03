---
title: Not
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
description: O elemento not representa uma expressão de pesquisa que nega o valor booliano da expressão de pesquisa que ela contém.
ms.openlocfilehash: 84c64a6d9d39f260d416fc32e4e5f5fcdef027e5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466714"
---
# <a name="not"></a><span data-ttu-id="9f194-103">Not</span><span class="sxs-lookup"><span data-stu-id="9f194-103">Not</span></span>

<span data-ttu-id="9f194-104">O elemento **not** representa uma expressão de pesquisa que nega o valor booliano da expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="9f194-104">The **Not** element represents a search expression that negates the Boolean value of the search expression that it contains.</span></span> 
  
```xml
<Not>
   <SearchExpression/>
</Not>
```

 <span data-ttu-id="9f194-105">**Não tipo**</span><span class="sxs-lookup"><span data-stu-id="9f194-105">**NotType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f194-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9f194-106">Attributes and elements</span></span>

<span data-ttu-id="9f194-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9f194-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f194-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9f194-108">Attributes</span></span>

<span data-ttu-id="9f194-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f194-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f194-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9f194-110">Child elements</span></span>

|<span data-ttu-id="9f194-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9f194-111">**Element**</span></span>|<span data-ttu-id="9f194-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9f194-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f194-113">Pesquisa</span><span class="sxs-lookup"><span data-stu-id="9f194-113">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="9f194-114">Representa a classe base para expressões dentro de uma restrição.</span><span class="sxs-lookup"><span data-stu-id="9f194-114">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="9f194-115">Um dos seguintes elementos deve ser substituído pelo elemento **searché** :</span><span class="sxs-lookup"><span data-stu-id="9f194-115">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="9f194-116">- [Houver](exists.md)</span><span class="sxs-lookup"><span data-stu-id="9f194-116">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="9f194-117">- [Exclui](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="9f194-117">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="9f194-118">- [IsEqualTo](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="9f194-118">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="9f194-119">- [IsNotEqualTo](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="9f194-119">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="9f194-120">- [IsGreaterThan](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="9f194-120">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="9f194-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="9f194-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="9f194-122">- [IsLessThan](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="9f194-122">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="9f194-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="9f194-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="9f194-124">- [Contém](contains.md)</span><span class="sxs-lookup"><span data-stu-id="9f194-124">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="9f194-125">- **Sido**</span><span class="sxs-lookup"><span data-stu-id="9f194-125">- **Not**</span></span> <br/><span data-ttu-id="9f194-126">- [E](and.md)</span><span class="sxs-lookup"><span data-stu-id="9f194-126">- [And](and.md)</span></span> <br/><span data-ttu-id="9f194-127">- [Ou](or.md)</span><span class="sxs-lookup"><span data-stu-id="9f194-127">- [Or](or.md)</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f194-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9f194-128">Parent elements</span></span>

|<span data-ttu-id="9f194-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9f194-129">**Element**</span></span>|<span data-ttu-id="9f194-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9f194-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f194-131">Restriction</span><span class="sxs-lookup"><span data-stu-id="9f194-131">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="9f194-132">Representa a restrição ou a consulta usada para filtrar itens ou pastas no FindItem/FindFolder e operações de pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="9f194-132">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|<span data-ttu-id="9f194-133">**Not**</span><span class="sxs-lookup"><span data-stu-id="9f194-133">**Not**</span></span> <br/> |<span data-ttu-id="9f194-134">Representa uma expressão de pesquisa que nega o valor booliano da expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="9f194-134">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="9f194-135">And</span><span class="sxs-lookup"><span data-stu-id="9f194-135">And</span></span>](and.md) <br/> |<span data-ttu-id="9f194-136">Representa uma expressão de pesquisa que permite executar um Boolean **e** uma operação entre duas ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="9f194-136">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="9f194-137">O resultado da operação **and** será **true** se todas as expressões de pesquisa contidas no elemento **e** forem **true**.</span><span class="sxs-lookup"><span data-stu-id="9f194-137">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="9f194-138">Or</span><span class="sxs-lookup"><span data-stu-id="9f194-138">Or</span></span>](or.md) <br/> |<span data-ttu-id="9f194-139">Representa uma expressão de pesquisa que executa uma operação lógica **ou** na expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="9f194-139">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="9f194-140">**Ou** retornará **true** se qualquer um dos seus filhos retornar **true**.</span><span class="sxs-lookup"><span data-stu-id="9f194-140">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="9f194-141">**Ou** deve ter dois ou mais filhos.</span><span class="sxs-lookup"><span data-stu-id="9f194-141">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9f194-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="9f194-142">Remarks</span></span>

<span data-ttu-id="9f194-143">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="9f194-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f194-144">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9f194-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f194-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="9f194-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9f194-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9f194-146">Schema Name</span></span>  <br/> |<span data-ttu-id="9f194-147">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9f194-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="9f194-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9f194-148">Validation File</span></span>  <br/> |<span data-ttu-id="9f194-149">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9f194-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9f194-150">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9f194-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="9f194-151">False</span><span class="sxs-lookup"><span data-stu-id="9f194-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f194-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="9f194-152">See also</span></span>

- [<span data-ttu-id="9f194-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9f194-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

