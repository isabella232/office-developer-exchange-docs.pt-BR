---
title: Máscara de bits
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bitmask
api_type:
- schema
ms.assetid: fc7eeac2-555f-4cbc-8b48-26d9ed67748a
description: O elemento de Bitmask representa uma máscara hexadecimal ou decimal a ser usado durante uma operação de restrição de exclusões.
ms.openlocfilehash: 86c8c61f22d8d620a9139280b2a43ed7fec4727d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751285"
---
# <a name="bitmask"></a><span data-ttu-id="e1b6f-103">Máscara de bits</span><span class="sxs-lookup"><span data-stu-id="e1b6f-103">Bitmask</span></span>

<span data-ttu-id="e1b6f-104">O elemento de **Bitmask** representa uma máscara hexadecimal ou decimal a ser usado durante uma operação de restrição de [exclusões](excludes.md) .</span><span class="sxs-lookup"><span data-stu-id="e1b6f-104">The **Bitmask** element represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> 
  
```xml
<Bitmask Value="" />
```

<span data-ttu-id="e1b6f-105">**ExcludesValueType**</span><span class="sxs-lookup"><span data-stu-id="e1b6f-105">**ExcludesValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e1b6f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e1b6f-106">Attributes and elements</span></span>

<span data-ttu-id="e1b6f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e1b6f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1b6f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e1b6f-108">Attributes</span></span>

|<span data-ttu-id="e1b6f-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="e1b6f-109">**Attribute**</span></span>|<span data-ttu-id="e1b6f-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1b6f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e1b6f-111">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e1b6f-111">**Value**</span></span> | <span data-ttu-id="e1b6f-112">Representa uma bitmask decimal ou hexadecimal.</span><span class="sxs-lookup"><span data-stu-id="e1b6f-112">Represents a decimal or hexadecimal bitmask.</span></span> <span data-ttu-id="e1b6f-113">O valor é representado pela expressão regular a seguir:</span><span class="sxs-lookup"><span data-stu-id="e1b6f-113">The value is represented by the following regular expression:</span></span><br/><span data-ttu-id="e1b6f-114">' ((0x</span><span class="sxs-lookup"><span data-stu-id="e1b6f-114">\`((0x</span></span>|<span data-ttu-id="e1b6f-115">0x)[0-9a-FA-f]\*)</span><span class="sxs-lookup"><span data-stu-id="e1b6f-115">0X)[0-9A-Fa-f]\*)</span></span>|<span data-ttu-id="e1b6f-116">([0-9] \*)'.</span><span class="sxs-lookup"><span data-stu-id="e1b6f-116">([0-9]\*)\`.</span></span><br/><br/><span data-ttu-id="e1b6f-117">A seguir estão exemplos de valores hexadecimais para este atributo:</span><span class="sxs-lookup"><span data-stu-id="e1b6f-117">The following are examples of hexadecimal values for this attribute:</span></span><br/><span data-ttu-id="e1b6f-118">-0x12AF</span><span class="sxs-lookup"><span data-stu-id="e1b6f-118">- 0x12AF</span></span><br/><span data-ttu-id="e1b6f-119">-0X334AE</span><span class="sxs-lookup"><span data-stu-id="e1b6f-119">- 0X334AE</span></span><br/><br/><span data-ttu-id="e1b6f-120">A seguir estão exemplos de decimais valores para este atributo:</span><span class="sxs-lookup"><span data-stu-id="e1b6f-120">The following are examples of decimal values for this attribute:</span></span><br/><span data-ttu-id="e1b6f-121">-10</span><span class="sxs-lookup"><span data-stu-id="e1b6f-121">- 10</span></span><br/><span data-ttu-id="e1b6f-122">-255</span><span class="sxs-lookup"><span data-stu-id="e1b6f-122">- 255</span></span><br/><span data-ttu-id="e1b6f-123">-4562</span><span class="sxs-lookup"><span data-stu-id="e1b6f-123">- 4562</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="e1b6f-124">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e1b6f-124">Child elements</span></span>

<span data-ttu-id="e1b6f-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e1b6f-125">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e1b6f-126">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e1b6f-126">Parent elements</span></span>

|<span data-ttu-id="e1b6f-127">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e1b6f-127">**Element**</span></span>|<span data-ttu-id="e1b6f-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1b6f-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1b6f-129">Exclui</span><span class="sxs-lookup"><span data-stu-id="e1b6f-129">Excludes</span></span>](excludes.md) <br/> |<span data-ttu-id="e1b6f-130">Executa uma máscara de bit a bit das propriedades.</span><span class="sxs-lookup"><span data-stu-id="e1b6f-130">Performs a bitwise mask of the properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e1b6f-131">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="e1b6f-131">Remarks</span></span>

<span data-ttu-id="e1b6f-132">Valores hexadecimais devem ter um prefixo de 0x ou 0x.</span><span class="sxs-lookup"><span data-stu-id="e1b6f-132">Hexadecimal values must have a prefix of either 0x or 0X.</span></span> <span data-ttu-id="e1b6f-133">Se esse prefixo não existir, o valor é considerado um número decimal.</span><span class="sxs-lookup"><span data-stu-id="e1b6f-133">If this prefix does not exist, the value is assumed to be a decimal number.</span></span>
  
<span data-ttu-id="e1b6f-134">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="e1b6f-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1b6f-135">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e1b6f-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1b6f-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="e1b6f-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e1b6f-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e1b6f-137">Schema name</span></span>  <br/> |<span data-ttu-id="e1b6f-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e1b6f-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="e1b6f-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e1b6f-139">Validation file</span></span>  <br/> |<span data-ttu-id="e1b6f-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e1b6f-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e1b6f-141">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e1b6f-141">Can be empty</span></span>  <br/> |<span data-ttu-id="e1b6f-142">False</span><span class="sxs-lookup"><span data-stu-id="e1b6f-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1b6f-143">Ver também</span><span class="sxs-lookup"><span data-stu-id="e1b6f-143">See also</span></span>

- [<span data-ttu-id="e1b6f-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e1b6f-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

