---
title: Exclui
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Excludes
api_type:
- schema
ms.assetid: bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1
description: O elemento de exclusões realiza uma máscara de bit a bit da propriedade especificada e um valor fornecido.
ms.openlocfilehash: 73e4eb782a4f54c113ea9a9b67fcf185a9028153
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752133"
---
# <a name="excludes"></a><span data-ttu-id="c6498-103">Exclui</span><span class="sxs-lookup"><span data-stu-id="c6498-103">Excludes</span></span>

<span data-ttu-id="c6498-104">O elemento de **exclusões** realiza uma máscara de bit a bit da propriedade especificada e um valor fornecido.</span><span class="sxs-lookup"><span data-stu-id="c6498-104">The **Excludes** element performs a bitwise mask of the specified property and a supplied value.</span></span> 
  
```xml
<Excludes>
   <FieldURI/>
   <Bitmask/>
</Excludes>
```

 <span data-ttu-id="c6498-105">**ExcludesType**</span><span class="sxs-lookup"><span data-stu-id="c6498-105">**ExcludesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6498-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c6498-106">Attributes and elements</span></span>

<span data-ttu-id="c6498-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c6498-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6498-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c6498-108">Attributes</span></span>

<span data-ttu-id="c6498-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c6498-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6498-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c6498-110">Child elements</span></span>

|<span data-ttu-id="c6498-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c6498-111">**Element**</span></span>|<span data-ttu-id="c6498-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c6498-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6498-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="c6498-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="c6498-114">Identifica as propriedades frequentemente referenciadas pelo URI.</span><span class="sxs-lookup"><span data-stu-id="c6498-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="c6498-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c6498-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="c6498-116">Identifica a membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="c6498-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="c6498-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c6498-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="c6498-118">Identifica as propriedades MAPI.</span><span class="sxs-lookup"><span data-stu-id="c6498-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="c6498-119">Máscara de bits</span><span class="sxs-lookup"><span data-stu-id="c6498-119">Bitmask</span></span>](bitmask.md) <br/> |<span data-ttu-id="c6498-120">Representa uma máscara hexadecimal ou decimal a ser usado durante uma operação de restrição de [exclusões](excludes.md) .</span><span class="sxs-lookup"><span data-stu-id="c6498-120">Represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> <span data-ttu-id="c6498-121">Se o bitmask representar um número hexadecimal, devem ser precedido por 0x ou 0x.</span><span class="sxs-lookup"><span data-stu-id="c6498-121">If the bitmask represents a hexadecimal number, it must be prefixed by 0x or 0X.</span></span> <span data-ttu-id="c6498-122">Caso contrário, ele será considerado um número decimal.</span><span class="sxs-lookup"><span data-stu-id="c6498-122">Otherwise, it will be considered a decimal number.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c6498-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c6498-123">Parent elements</span></span>

|<span data-ttu-id="c6498-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c6498-124">**Element**</span></span>|<span data-ttu-id="c6498-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c6498-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6498-126">Restriction</span><span class="sxs-lookup"><span data-stu-id="c6498-126">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="c6498-127">Representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c6498-127">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="c6498-128">Não</span><span class="sxs-lookup"><span data-stu-id="c6498-128">Not</span></span>](not.md) <br/> |<span data-ttu-id="c6498-129">Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="c6498-129">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="c6498-130">E</span><span class="sxs-lookup"><span data-stu-id="c6498-130">And</span></span>](and.md) <br/> |<span data-ttu-id="c6498-131">Representa uma expressão de pesquisa que permite realizar uma operação Boolean e entre dois ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c6498-131">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="c6498-132">O resultado da operação e será **true** se todas as expressões de pesquisa contidas And forem **verdadeiras**.</span><span class="sxs-lookup"><span data-stu-id="c6498-132">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="c6498-133">Ou</span><span class="sxs-lookup"><span data-stu-id="c6498-133">Or</span></span>](or.md) <br/> |<span data-ttu-id="c6498-134">Representa uma expressão de pesquisa que realiza um OR lógico a expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="c6498-134">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="c6498-135">O elemento [ou](or.md) retornará **true** se qualquer um dos seus filhos retornam **true**.</span><span class="sxs-lookup"><span data-stu-id="c6498-135">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c6498-136">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="c6498-136">Remarks</span></span>

 <span data-ttu-id="c6498-137">**Exclui** resolverá como **true** se uma operação de AND realizada no seguinte for resolvido como 0:</span><span class="sxs-lookup"><span data-stu-id="c6498-137">**Excludes** will resolve to **true** if an AND operation performed on the following resolves to 0:</span></span> 
  
1. <span data-ttu-id="c6498-138">O valor da propriedade bit a bit</span><span class="sxs-lookup"><span data-stu-id="c6498-138">The bitwise value for the property</span></span>
    
2. <span data-ttu-id="c6498-139">O valor de bitmask para a propriedade</span><span class="sxs-lookup"><span data-stu-id="c6498-139">The bitmask value for the property</span></span>
    
 <span data-ttu-id="c6498-140">**Exclui** só podem ser aplicadas a uma propriedade que tem um valor inteiro.</span><span class="sxs-lookup"><span data-stu-id="c6498-140">**Excludes** can only be applied to a property that has an integer value.</span></span> <span data-ttu-id="c6498-141">Se o tipo da propriedade for algo diferente de um número inteiro, um código de erro de **ErrorUnsupportedPathForQuery** será retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="c6498-141">If the property type is anything other than an integer, an error code of **ErrorUnsupportedPathForQuery** is returned in the response.</span></span> 
  
<span data-ttu-id="c6498-142">Você pode executar a operação inversa chamando Not(Excludes).</span><span class="sxs-lookup"><span data-stu-id="c6498-142">You can perform the reverse operation by calling Not(Excludes).</span></span>
  
<span data-ttu-id="c6498-143">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="c6498-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c6498-144">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c6498-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6498-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="c6498-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c6498-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c6498-146">Schema Name</span></span>  <br/> |<span data-ttu-id="c6498-147">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c6498-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="c6498-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c6498-148">Validation File</span></span>  <br/> |<span data-ttu-id="c6498-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c6498-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c6498-150">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c6498-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="c6498-151">False</span><span class="sxs-lookup"><span data-stu-id="c6498-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6498-152">Ver também</span><span class="sxs-lookup"><span data-stu-id="c6498-152">See also</span></span>



- [<span data-ttu-id="c6498-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c6498-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

