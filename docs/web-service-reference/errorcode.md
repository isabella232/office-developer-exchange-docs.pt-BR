---
title: ErrorCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0bb00cee-c66b-4f34-b99d-355458f5e83b
description: O elemento ErrorCode representa um código de erro de validação de regra que descreve o que falha na validação para cada predicado regra ou ação.
ms.openlocfilehash: ed8e2fa72b0eb007925742e6d194f3a391b3f3cb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752094"
---
# <a name="errorcode"></a><span data-ttu-id="495d5-103">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="495d5-103">ErrorCode</span></span>

<span data-ttu-id="495d5-104">O elemento **ErrorCode** representa um código de erro de validação de regra que descreve o que falha na validação para cada predicado regra ou ação.</span><span class="sxs-lookup"><span data-stu-id="495d5-104">The **ErrorCode** element represents a rule validation error code that describes what failed validation for each rule predicate or action.</span></span> 
  
```XML
<ErrorCode/>
```

 <span data-ttu-id="495d5-105">**RuleValidationErrorCodeType**</span><span class="sxs-lookup"><span data-stu-id="495d5-105">**RuleValidationErrorCodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="495d5-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="495d5-106">Attributes and elements</span></span>

<span data-ttu-id="495d5-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="495d5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="495d5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="495d5-108">Attributes</span></span>

<span data-ttu-id="495d5-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="495d5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="495d5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="495d5-110">Child elements</span></span>

<span data-ttu-id="495d5-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="495d5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="495d5-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="495d5-112">Parent elements</span></span>

|<span data-ttu-id="495d5-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="495d5-113">**Element**</span></span>|<span data-ttu-id="495d5-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="495d5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="495d5-115">Erro</span><span class="sxs-lookup"><span data-stu-id="495d5-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="495d5-116">Representa um erro de validação exclusivo em um valor da propriedade regra específica, o valor da propriedade predicado ou o valor da propriedade action.</span><span class="sxs-lookup"><span data-stu-id="495d5-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="495d5-117">Text value</span><span class="sxs-lookup"><span data-stu-id="495d5-117">Text value</span></span>

<span data-ttu-id="495d5-118">O valor de texto para esse elemento é restrito a uma das cadeias de caracteres seguintes:</span><span class="sxs-lookup"><span data-stu-id="495d5-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="495d5-119">ADOperationFailure</span><span class="sxs-lookup"><span data-stu-id="495d5-119">ADOperationFailure</span></span>
    
- <span data-ttu-id="495d5-120">ConnectedAccountNotFound</span><span class="sxs-lookup"><span data-stu-id="495d5-120">ConnectedAccountNotFound</span></span>
    
- <span data-ttu-id="495d5-121">CreateWithRuleId</span><span class="sxs-lookup"><span data-stu-id="495d5-121">CreateWithRuleId</span></span>
    
- <span data-ttu-id="495d5-122">EmptyValueFound</span><span class="sxs-lookup"><span data-stu-id="495d5-122">EmptyValueFound</span></span>
    
- <span data-ttu-id="495d5-123">DuplicatedPriority</span><span class="sxs-lookup"><span data-stu-id="495d5-123">DuplicatedPriority</span></span>
    
- <span data-ttu-id="495d5-124">DuplicatedOperationOnTheSameRule</span><span class="sxs-lookup"><span data-stu-id="495d5-124">DuplicatedOperationOnTheSameRule</span></span>
    
- <span data-ttu-id="495d5-125">FolderDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="495d5-125">FolderDoesNotExist</span></span>
    
- <span data-ttu-id="495d5-126">InvalidAddress</span><span class="sxs-lookup"><span data-stu-id="495d5-126">InvalidAddress</span></span>
    
- <span data-ttu-id="495d5-127">InvalidDateRange</span><span class="sxs-lookup"><span data-stu-id="495d5-127">InvalidDateRange</span></span>
    
- <span data-ttu-id="495d5-128">InvalidFolderId</span><span class="sxs-lookup"><span data-stu-id="495d5-128">InvalidFolderId</span></span>
    
- <span data-ttu-id="495d5-129">InvalidSizeRange</span><span class="sxs-lookup"><span data-stu-id="495d5-129">InvalidSizeRange</span></span>
    
- <span data-ttu-id="495d5-130">InvalidValue</span><span class="sxs-lookup"><span data-stu-id="495d5-130">InvalidValue</span></span>
    
- <span data-ttu-id="495d5-131">MessageClassificationNotFound</span><span class="sxs-lookup"><span data-stu-id="495d5-131">MessageClassificationNotFound</span></span>
    
- <span data-ttu-id="495d5-132">MissingAction</span><span class="sxs-lookup"><span data-stu-id="495d5-132">MissingAction</span></span>
    
- <span data-ttu-id="495d5-133">MissingParameter</span><span class="sxs-lookup"><span data-stu-id="495d5-133">MissingParameter</span></span>
    
- <span data-ttu-id="495d5-134">MissingRangeValue</span><span class="sxs-lookup"><span data-stu-id="495d5-134">MissingRangeValue</span></span>
    
- <span data-ttu-id="495d5-135">NotSettable</span><span class="sxs-lookup"><span data-stu-id="495d5-135">NotSettable</span></span>
    
- <span data-ttu-id="495d5-136">RecipientDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="495d5-136">RecipientDoesNotExist</span></span>
    
- <span data-ttu-id="495d5-137">RuleNotFound</span><span class="sxs-lookup"><span data-stu-id="495d5-137">RuleNotFound</span></span>
    
- <span data-ttu-id="495d5-138">SizeLessThanZero</span><span class="sxs-lookup"><span data-stu-id="495d5-138">SizeLessThanZero</span></span>
    
- <span data-ttu-id="495d5-139">StringValueTooBig</span><span class="sxs-lookup"><span data-stu-id="495d5-139">StringValueTooBig</span></span>
    
- <span data-ttu-id="495d5-140">UnsupportedAddress</span><span class="sxs-lookup"><span data-stu-id="495d5-140">UnsupportedAddress</span></span>
    
- <span data-ttu-id="495d5-141">UnexpectedError</span><span class="sxs-lookup"><span data-stu-id="495d5-141">UnexpectedError</span></span>
    
- <span data-ttu-id="495d5-142">UnsupportedRule</span><span class="sxs-lookup"><span data-stu-id="495d5-142">UnsupportedRule</span></span>
    
## <a name="remarks"></a><span data-ttu-id="495d5-143">Comentários</span><span class="sxs-lookup"><span data-stu-id="495d5-143">Remarks</span></span>

<span data-ttu-id="495d5-144">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="495d5-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="495d5-145">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="495d5-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="495d5-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="495d5-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="495d5-147">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="495d5-147">Schema Name</span></span>  <br/> |<span data-ttu-id="495d5-148">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="495d5-148">Messages schema</span></span>  <br/> |
|<span data-ttu-id="495d5-149">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="495d5-149">Validation File</span></span>  <br/> |<span data-ttu-id="495d5-150">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="495d5-150">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="495d5-151">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="495d5-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="495d5-152">False</span><span class="sxs-lookup"><span data-stu-id="495d5-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="495d5-153">Ver também</span><span class="sxs-lookup"><span data-stu-id="495d5-153">See also</span></span>



- [<span data-ttu-id="495d5-154">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="495d5-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

