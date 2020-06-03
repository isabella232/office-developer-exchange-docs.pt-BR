---
title: Mascara
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
description: O elemento bitmask representa uma máscara hexadecimal ou decimal a ser usada durante uma operação de restrição Excludes.
ms.openlocfilehash: f05be466d05b13f8f362afb5fc0552653a532475
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458807"
---
# <a name="bitmask"></a><span data-ttu-id="235f1-103">Mascara</span><span class="sxs-lookup"><span data-stu-id="235f1-103">Bitmask</span></span>

<span data-ttu-id="235f1-104">O elemento **bitmask** representa uma máscara hexadecimal ou decimal a ser usada durante uma operação de restrição [Excludes](excludes.md) .</span><span class="sxs-lookup"><span data-stu-id="235f1-104">The **Bitmask** element represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> 
  
```xml
<Bitmask Value="" />
```

<span data-ttu-id="235f1-105">**ExcludesValueType**</span><span class="sxs-lookup"><span data-stu-id="235f1-105">**ExcludesValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="235f1-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="235f1-106">Attributes and elements</span></span>

<span data-ttu-id="235f1-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="235f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="235f1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="235f1-108">Attributes</span></span>

|<span data-ttu-id="235f1-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="235f1-109">**Attribute**</span></span>|<span data-ttu-id="235f1-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="235f1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="235f1-111">**Valor**</span><span class="sxs-lookup"><span data-stu-id="235f1-111">**Value**</span></span> | <span data-ttu-id="235f1-112">Representa um bitmask decimal ou hexadecimal.</span><span class="sxs-lookup"><span data-stu-id="235f1-112">Represents a decimal or hexadecimal bitmask.</span></span> <span data-ttu-id="235f1-113">O valor é representado pela seguinte expressão regular:</span><span class="sxs-lookup"><span data-stu-id="235f1-113">The value is represented by the following regular expression:</span></span><br/><span data-ttu-id="235f1-114">`((0x|0X)[0-9A-Fa-f]*)|([0-9]*)`.</span><span class="sxs-lookup"><span data-stu-id="235f1-114">`((0x|0X)[0-9A-Fa-f]*)|([0-9]*)`.</span></span><br/><br/><span data-ttu-id="235f1-115">Estes são exemplos de valores hexadecimais para este atributo:</span><span class="sxs-lookup"><span data-stu-id="235f1-115">The following are examples of hexadecimal values for this attribute:</span></span><br/><span data-ttu-id="235f1-116">- 0x12AF</span><span class="sxs-lookup"><span data-stu-id="235f1-116">- 0x12AF</span></span><br/><span data-ttu-id="235f1-117">- 0X334AE</span><span class="sxs-lookup"><span data-stu-id="235f1-117">- 0X334AE</span></span><br/><br/><span data-ttu-id="235f1-118">Estes são exemplos de valores decimais para este atributo:</span><span class="sxs-lookup"><span data-stu-id="235f1-118">The following are examples of decimal values for this attribute:</span></span><br/><span data-ttu-id="235f1-119">-10</span><span class="sxs-lookup"><span data-stu-id="235f1-119">- 10</span></span><br/><span data-ttu-id="235f1-120">-255</span><span class="sxs-lookup"><span data-stu-id="235f1-120">- 255</span></span><br/><span data-ttu-id="235f1-121">-4562</span><span class="sxs-lookup"><span data-stu-id="235f1-121">- 4562</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="235f1-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="235f1-122">Child elements</span></span>

<span data-ttu-id="235f1-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="235f1-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="235f1-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="235f1-124">Parent elements</span></span>

|<span data-ttu-id="235f1-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="235f1-125">**Element**</span></span>|<span data-ttu-id="235f1-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="235f1-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="235f1-127">Exclui</span><span class="sxs-lookup"><span data-stu-id="235f1-127">Excludes</span></span>](excludes.md) <br/> |<span data-ttu-id="235f1-128">Executa uma máscara de bits bit das propriedades.</span><span class="sxs-lookup"><span data-stu-id="235f1-128">Performs a bitwise mask of the properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="235f1-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="235f1-129">Remarks</span></span>

<span data-ttu-id="235f1-130">Os valores hexadecimais devem ter um prefixo de 0x ou 0X.</span><span class="sxs-lookup"><span data-stu-id="235f1-130">Hexadecimal values must have a prefix of either 0x or 0X.</span></span> <span data-ttu-id="235f1-131">Se esse prefixo não existir, o valor será considerado um número decimal.</span><span class="sxs-lookup"><span data-stu-id="235f1-131">If this prefix does not exist, the value is assumed to be a decimal number.</span></span>
  
<span data-ttu-id="235f1-132">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="235f1-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="235f1-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="235f1-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="235f1-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="235f1-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="235f1-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="235f1-135">Schema name</span></span>  <br/> |<span data-ttu-id="235f1-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="235f1-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="235f1-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="235f1-137">Validation file</span></span>  <br/> |<span data-ttu-id="235f1-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="235f1-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="235f1-139">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="235f1-139">Can be empty</span></span>  <br/> |<span data-ttu-id="235f1-140">False</span><span class="sxs-lookup"><span data-stu-id="235f1-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="235f1-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="235f1-141">See also</span></span>

- [<span data-ttu-id="235f1-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="235f1-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

