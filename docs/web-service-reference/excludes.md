---
title: Excludes
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
ms.openlocfilehash: febd4171210319d8f7e475f9879c5f895f508713
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354383"
---
# <a name="excludes"></a><span data-ttu-id="34057-103">Excludes</span><span class="sxs-lookup"><span data-stu-id="34057-103">Excludes</span></span>

<span data-ttu-id="34057-104">O elemento de **exclusões** realiza uma máscara de bit a bit da propriedade especificada e um valor fornecido.</span><span class="sxs-lookup"><span data-stu-id="34057-104">The **Excludes** element performs a bitwise mask of the specified property and a supplied value.</span></span> 
  
```xml
<Excludes>
   <FieldURI/>
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <ExtendedFieldURI/> 
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <IndexedFieldURI/> 
   <Bitmask/>
</Excludes>
```

<span data-ttu-id="34057-105">**ExcludesType**</span><span class="sxs-lookup"><span data-stu-id="34057-105">**ExcludesType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="34057-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="34057-106">Attributes and elements</span></span>

<span data-ttu-id="34057-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="34057-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34057-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="34057-108">Attributes</span></span>

<span data-ttu-id="34057-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="34057-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="34057-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="34057-110">Child elements</span></span>

|<span data-ttu-id="34057-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="34057-111">**Element**</span></span>|<span data-ttu-id="34057-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="34057-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34057-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="34057-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="34057-114">Identifica as propriedades frequentemente referenciadas pelo URI.</span><span class="sxs-lookup"><span data-stu-id="34057-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="34057-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="34057-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="34057-116">Identifica a membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="34057-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="34057-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="34057-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="34057-118">Identifica as propriedades MAPI.</span><span class="sxs-lookup"><span data-stu-id="34057-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="34057-119">Bitmask</span><span class="sxs-lookup"><span data-stu-id="34057-119">Bitmask</span></span>](bitmask.md) <br/> |<span data-ttu-id="34057-120">Representa uma máscara hexadecimal ou decimal a ser usado durante uma operação de restrição de [exclusões](excludes.md) .</span><span class="sxs-lookup"><span data-stu-id="34057-120">Represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> <span data-ttu-id="34057-121">Se o bitmask representar um número hexadecimal, devem ser precedido por 0x ou 0x.</span><span class="sxs-lookup"><span data-stu-id="34057-121">If the bitmask represents a hexadecimal number, it must be prefixed by 0x or 0X.</span></span> <span data-ttu-id="34057-122">Caso contrário, ele será considerado um número decimal.</span><span class="sxs-lookup"><span data-stu-id="34057-122">Otherwise, it will be considered a decimal number.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="34057-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="34057-123">Parent elements</span></span>

|<span data-ttu-id="34057-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="34057-124">**Element**</span></span>|<span data-ttu-id="34057-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="34057-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34057-126">Restriction</span><span class="sxs-lookup"><span data-stu-id="34057-126">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="34057-127">Representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="34057-127">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="34057-128">Não</span><span class="sxs-lookup"><span data-stu-id="34057-128">Not</span></span>](not.md) <br/> |<span data-ttu-id="34057-129">Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="34057-129">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="34057-130">E</span><span class="sxs-lookup"><span data-stu-id="34057-130">And</span></span>](and.md) <br/> |<span data-ttu-id="34057-131">Representa uma expressão de pesquisa que permite realizar uma operação Boolean e entre dois ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="34057-131">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="34057-132">O resultado da operação e será **true** se todas as expressões de pesquisa contidas And forem **verdadeiras**.</span><span class="sxs-lookup"><span data-stu-id="34057-132">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="34057-133">Ou</span><span class="sxs-lookup"><span data-stu-id="34057-133">Or</span></span>](or.md) <br/> |<span data-ttu-id="34057-134">Representa uma expressão de pesquisa que realiza um OR lógico a expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="34057-134">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="34057-135">O elemento [ou](or.md) retornará **true** se qualquer um dos seus filhos retornam **true**.</span><span class="sxs-lookup"><span data-stu-id="34057-135">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="34057-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="34057-136">Remarks</span></span>

<span data-ttu-id="34057-137">**Exclui** resolverá como **true** se uma operação de AND realizada no seguinte for resolvido como 0:</span><span class="sxs-lookup"><span data-stu-id="34057-137">**Excludes** will resolve to **true** if an AND operation performed on the following resolves to 0:</span></span> 
  
1. <span data-ttu-id="34057-138">O valor da propriedade bit a bit</span><span class="sxs-lookup"><span data-stu-id="34057-138">The bitwise value for the property</span></span>
    
2. <span data-ttu-id="34057-139">O valor de bitmask para a propriedade</span><span class="sxs-lookup"><span data-stu-id="34057-139">The bitmask value for the property</span></span>
    
<span data-ttu-id="34057-140">**Exclui** só podem ser aplicadas a uma propriedade que tem um valor inteiro.</span><span class="sxs-lookup"><span data-stu-id="34057-140">**Excludes** can only be applied to a property that has an integer value.</span></span> <span data-ttu-id="34057-141">Se o tipo da propriedade for algo diferente de um número inteiro, um código de erro de **ErrorUnsupportedPathForQuery** será retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="34057-141">If the property type is anything other than an integer, an error code of **ErrorUnsupportedPathForQuery** is returned in the response.</span></span> 
  
<span data-ttu-id="34057-142">Você pode executar a operação inversa chamando Not(Excludes).</span><span class="sxs-lookup"><span data-stu-id="34057-142">You can perform the reverse operation by calling Not(Excludes).</span></span>
  
<span data-ttu-id="34057-143">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="34057-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34057-144">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="34057-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34057-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="34057-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="34057-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="34057-146">Schema Name</span></span>  <br/> |<span data-ttu-id="34057-147">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="34057-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="34057-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="34057-148">Validation File</span></span>  <br/> |<span data-ttu-id="34057-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="34057-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="34057-150">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="34057-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="34057-151">False</span><span class="sxs-lookup"><span data-stu-id="34057-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="34057-152">Ver também</span><span class="sxs-lookup"><span data-stu-id="34057-152">See also</span></span>

- [<span data-ttu-id="34057-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="34057-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

