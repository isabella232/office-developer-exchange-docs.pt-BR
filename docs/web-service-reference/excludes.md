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
description: O elemento Excludes executa uma máscara bit a bit da propriedade especificada e um valor fornecido.
ms.openlocfilehash: d5fcd8b86b454aa731bd43974b5b7d674fe76ed6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530611"
---
# <a name="excludes"></a><span data-ttu-id="50415-103">Exclui</span><span class="sxs-lookup"><span data-stu-id="50415-103">Excludes</span></span>

<span data-ttu-id="50415-104">O elemento **Excludes** executa uma máscara bit a bit da propriedade especificada e um valor fornecido.</span><span class="sxs-lookup"><span data-stu-id="50415-104">The **Excludes** element performs a bitwise mask of the specified property and a supplied value.</span></span> 
  
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

<span data-ttu-id="50415-105">**ExcludesType**</span><span class="sxs-lookup"><span data-stu-id="50415-105">**ExcludesType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="50415-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="50415-106">Attributes and elements</span></span>

<span data-ttu-id="50415-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="50415-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50415-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="50415-108">Attributes</span></span>

<span data-ttu-id="50415-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50415-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50415-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="50415-110">Child elements</span></span>

|<span data-ttu-id="50415-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="50415-111">**Element**</span></span>|<span data-ttu-id="50415-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="50415-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50415-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="50415-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="50415-114">Identifica as propriedades com frequência referenciadas por URI.</span><span class="sxs-lookup"><span data-stu-id="50415-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="50415-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="50415-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="50415-116">Identifica membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="50415-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="50415-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="50415-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="50415-118">Identifica as propriedades MAPI.</span><span class="sxs-lookup"><span data-stu-id="50415-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="50415-119">Mascara</span><span class="sxs-lookup"><span data-stu-id="50415-119">Bitmask</span></span>](bitmask.md) <br/> |<span data-ttu-id="50415-120">Representa uma máscara hexadecimal ou decimal a ser usada durante uma operação de restrição [Excludes](excludes.md) .</span><span class="sxs-lookup"><span data-stu-id="50415-120">Represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> <span data-ttu-id="50415-121">Se o bitmask representar um número hexadecimal, ele deve ser prefixado por 0x ou 0X.</span><span class="sxs-lookup"><span data-stu-id="50415-121">If the bitmask represents a hexadecimal number, it must be prefixed by 0x or 0X.</span></span> <span data-ttu-id="50415-122">Caso contrário, ele será considerado um número decimal.</span><span class="sxs-lookup"><span data-stu-id="50415-122">Otherwise, it will be considered a decimal number.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="50415-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="50415-123">Parent elements</span></span>

|<span data-ttu-id="50415-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="50415-124">**Element**</span></span>|<span data-ttu-id="50415-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="50415-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50415-126">Restriction</span><span class="sxs-lookup"><span data-stu-id="50415-126">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="50415-127">Representa a restrição ou a consulta usada para filtrar itens ou pastas no FindItem/FindFolder e operações de pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="50415-127">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="50415-128">Not</span><span class="sxs-lookup"><span data-stu-id="50415-128">Not</span></span>](not.md) <br/> |<span data-ttu-id="50415-129">Representa uma expressão de pesquisa que nega o valor booliano da expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="50415-129">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="50415-130">And</span><span class="sxs-lookup"><span data-stu-id="50415-130">And</span></span>](and.md) <br/> |<span data-ttu-id="50415-131">Representa uma expressão de pesquisa que permite executar um Boolean e uma operação entre duas ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="50415-131">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="50415-132">O resultado da operação and será **true** se todas as expressões de pesquisa contidas no e forem **true**.</span><span class="sxs-lookup"><span data-stu-id="50415-132">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="50415-133">Or</span><span class="sxs-lookup"><span data-stu-id="50415-133">Or</span></span>](or.md) <br/> |<span data-ttu-id="50415-134">Representa uma expressão de pesquisa que executa uma expressão lógica ou na expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="50415-134">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="50415-135">O elemento [ou](or.md) retornará **true** se qualquer um dos seus filhos retornar **true**.</span><span class="sxs-lookup"><span data-stu-id="50415-135">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="50415-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="50415-136">Remarks</span></span>

<span data-ttu-id="50415-137">As **exclusões** serão resolvidas como **true** se uma operação and executada no seguinte procedimento resolver para 0:</span><span class="sxs-lookup"><span data-stu-id="50415-137">**Excludes** will resolve to **true** if an AND operation performed on the following resolves to 0:</span></span> 
  
1. <span data-ttu-id="50415-138">O valor bit a bit da propriedade</span><span class="sxs-lookup"><span data-stu-id="50415-138">The bitwise value for the property</span></span>
    
2. <span data-ttu-id="50415-139">O valor de bitmask para a propriedade</span><span class="sxs-lookup"><span data-stu-id="50415-139">The bitmask value for the property</span></span>
    
<span data-ttu-id="50415-140">**Excludes** só podem ser aplicadas a uma propriedade que tenha um valor inteiro.</span><span class="sxs-lookup"><span data-stu-id="50415-140">**Excludes** can only be applied to a property that has an integer value.</span></span> <span data-ttu-id="50415-141">Se o tipo de propriedade for algo diferente de um inteiro, um código de erro de **ErrorUnsupportedPathForQuery** será retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="50415-141">If the property type is anything other than an integer, an error code of **ErrorUnsupportedPathForQuery** is returned in the response.</span></span> 
  
<span data-ttu-id="50415-142">Você pode executar a operação reversa chamando não (exclui).</span><span class="sxs-lookup"><span data-stu-id="50415-142">You can perform the reverse operation by calling Not(Excludes).</span></span>
  
<span data-ttu-id="50415-143">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="50415-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50415-144">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="50415-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50415-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="50415-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="50415-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="50415-146">Schema Name</span></span>  <br/> |<span data-ttu-id="50415-147">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="50415-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="50415-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="50415-148">Validation File</span></span>  <br/> |<span data-ttu-id="50415-149">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="50415-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="50415-150">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="50415-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="50415-151">False</span><span class="sxs-lookup"><span data-stu-id="50415-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="50415-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="50415-152">See also</span></span>

- [<span data-ttu-id="50415-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="50415-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

