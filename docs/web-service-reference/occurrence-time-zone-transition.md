---
title: Ocorrência (transição de fuso horário)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Occurrence
api_type:
- schema
ms.assetid: 5c1142b1-c51f-42e1-bbb2-57e00cad0fdb
description: O elemento de ocorrência representa a ocorrência do dia da semana do mês em que ocorre a transição do fuso horário.
ms.openlocfilehash: bc5160480cc6881bb9d724aa61323f5717d1f2fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824636"
---
# <a name="occurrence-time-zone-transition"></a><span data-ttu-id="c28dd-103">Ocorrência (transição de fuso horário)</span><span class="sxs-lookup"><span data-stu-id="c28dd-103">Occurrence (Time Zone Transition)</span></span>

<span data-ttu-id="c28dd-104">O elemento de **ocorrência** representa a ocorrência do dia da semana do mês em que ocorre a transição do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="c28dd-104">The **Occurrence** element represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span> 
  
```xml
<Occurrence/>
```

<span data-ttu-id="c28dd-105">**int**</span><span class="sxs-lookup"><span data-stu-id="c28dd-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c28dd-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c28dd-106">Attributes and elements</span></span>

<span data-ttu-id="c28dd-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c28dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c28dd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c28dd-108">Attributes</span></span>

<span data-ttu-id="c28dd-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c28dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c28dd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c28dd-110">Child elements</span></span>

<span data-ttu-id="c28dd-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c28dd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c28dd-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c28dd-112">Parent elements</span></span>

|<span data-ttu-id="c28dd-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c28dd-113">**Element**</span></span>|<span data-ttu-id="c28dd-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c28dd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c28dd-115">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="c28dd-115">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="c28dd-116">Representa uma transição de fuso horário que ocorre no mesmo dia cada ano.</span><span class="sxs-lookup"><span data-stu-id="c28dd-116">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c28dd-117">Text value</span><span class="sxs-lookup"><span data-stu-id="c28dd-117">Text value</span></span>

<span data-ttu-id="c28dd-118">O valor de texto é um inteiro que representa a ocorrência do dia da semana do mês em que ocorre a transição do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="c28dd-118">The text value is an integer that represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span> <span data-ttu-id="c28dd-119">A tabela a seguir lista os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="c28dd-119">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="c28dd-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="c28dd-120">**Value**</span></span>|<span data-ttu-id="c28dd-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c28dd-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c28dd-122">1</span><span class="sxs-lookup"><span data-stu-id="c28dd-122">1</span></span>  <br/> |<span data-ttu-id="c28dd-123">A primeira ocorrência do dia da semana desde o início do mês especificado.</span><span class="sxs-lookup"><span data-stu-id="c28dd-123">The first occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="c28dd-124">2</span><span class="sxs-lookup"><span data-stu-id="c28dd-124">2</span></span>  <br/> |<span data-ttu-id="c28dd-125">A segunda ocorrência do dia da semana desde o início do mês especificado.</span><span class="sxs-lookup"><span data-stu-id="c28dd-125">The second occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="c28dd-126">3</span><span class="sxs-lookup"><span data-stu-id="c28dd-126">3</span></span>  <br/> |<span data-ttu-id="c28dd-127">A terceira ocorrência do dia da semana desde o início do mês especificado.</span><span class="sxs-lookup"><span data-stu-id="c28dd-127">The third occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="c28dd-128">4</span><span class="sxs-lookup"><span data-stu-id="c28dd-128">4</span></span>  <br/> |<span data-ttu-id="c28dd-129">A quarta ocorrência do dia da semana desde o início do mês especificado.</span><span class="sxs-lookup"><span data-stu-id="c28dd-129">The fourth occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="c28dd-130">-1</span><span class="sxs-lookup"><span data-stu-id="c28dd-130">-1</span></span>  <br/> |<span data-ttu-id="c28dd-131">A primeira ocorrência do dia da semana do final do mês especificado.</span><span class="sxs-lookup"><span data-stu-id="c28dd-131">The first occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="c28dd-132">-2</span><span class="sxs-lookup"><span data-stu-id="c28dd-132">-2</span></span>  <br/> |<span data-ttu-id="c28dd-133">A segunda ocorrência do dia da semana do final do mês especificado.</span><span class="sxs-lookup"><span data-stu-id="c28dd-133">The second occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="c28dd-134">-3</span><span class="sxs-lookup"><span data-stu-id="c28dd-134">-3</span></span>  <br/> |<span data-ttu-id="c28dd-135">A terceira ocorrência do dia da semana do final do mês especificado.</span><span class="sxs-lookup"><span data-stu-id="c28dd-135">The third occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="c28dd-136">-4</span><span class="sxs-lookup"><span data-stu-id="c28dd-136">-4</span></span>  <br/> |<span data-ttu-id="c28dd-137">A quarta ocorrência do dia da semana do final do mês especificado.</span><span class="sxs-lookup"><span data-stu-id="c28dd-137">The fourth occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c28dd-138">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="c28dd-138">Remarks</span></span>

<span data-ttu-id="c28dd-139">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="c28dd-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c28dd-140">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c28dd-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c28dd-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="c28dd-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c28dd-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c28dd-142">Schema Name</span></span>  <br/> |<span data-ttu-id="c28dd-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c28dd-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="c28dd-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c28dd-144">Validation File</span></span>  <br/> |<span data-ttu-id="c28dd-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c28dd-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c28dd-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c28dd-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="c28dd-147">False</span><span class="sxs-lookup"><span data-stu-id="c28dd-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c28dd-148">Ver também</span><span class="sxs-lookup"><span data-stu-id="c28dd-148">See also</span></span>

- [<span data-ttu-id="c28dd-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c28dd-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

