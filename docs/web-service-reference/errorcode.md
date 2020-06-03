---
title: ErrorCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0bb00cee-c66b-4f34-b99d-355458f5e83b
description: O elemento ErrorCode representa um código de erro de validação de regra que descreve o que houve falha na validação de cada predicado ou ação de regra.
ms.openlocfilehash: 6432aeee786d74a9afcb346cb66765f9001257de
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460075"
---
# <a name="errorcode"></a><span data-ttu-id="5a84e-103">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="5a84e-103">ErrorCode</span></span>

<span data-ttu-id="5a84e-104">O elemento **ErrorCode** representa um código de erro de validação de regra que descreve o que houve falha na validação de cada predicado ou ação de regra.</span><span class="sxs-lookup"><span data-stu-id="5a84e-104">The **ErrorCode** element represents a rule validation error code that describes what failed validation for each rule predicate or action.</span></span> 
  
```XML
<ErrorCode/>
```

 <span data-ttu-id="5a84e-105">**RuleValidationErrorCodeType**</span><span class="sxs-lookup"><span data-stu-id="5a84e-105">**RuleValidationErrorCodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a84e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5a84e-106">Attributes and elements</span></span>

<span data-ttu-id="5a84e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5a84e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a84e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5a84e-108">Attributes</span></span>

<span data-ttu-id="5a84e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5a84e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a84e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5a84e-110">Child elements</span></span>

<span data-ttu-id="5a84e-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5a84e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5a84e-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5a84e-112">Parent elements</span></span>

|<span data-ttu-id="5a84e-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5a84e-113">**Element**</span></span>|<span data-ttu-id="5a84e-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5a84e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a84e-115">Erro</span><span class="sxs-lookup"><span data-stu-id="5a84e-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="5a84e-116">Representa um único erro de validação em um valor de propriedade de regra específico, um valor da propriedade Predicate ou um valor da propriedade Action.</span><span class="sxs-lookup"><span data-stu-id="5a84e-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5a84e-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5a84e-117">Text value</span></span>

<span data-ttu-id="5a84e-118">O valor de texto para este elemento é restrito a uma das seguintes cadeias de caracteres:</span><span class="sxs-lookup"><span data-stu-id="5a84e-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="5a84e-119">ADOperationFailure</span><span class="sxs-lookup"><span data-stu-id="5a84e-119">ADOperationFailure</span></span>
    
- <span data-ttu-id="5a84e-120">ConnectedAccountNotFound</span><span class="sxs-lookup"><span data-stu-id="5a84e-120">ConnectedAccountNotFound</span></span>
    
- <span data-ttu-id="5a84e-121">CreateWithRuleId</span><span class="sxs-lookup"><span data-stu-id="5a84e-121">CreateWithRuleId</span></span>
    
- <span data-ttu-id="5a84e-122">EmptyValueFound</span><span class="sxs-lookup"><span data-stu-id="5a84e-122">EmptyValueFound</span></span>
    
- <span data-ttu-id="5a84e-123">DuplicatedPriority</span><span class="sxs-lookup"><span data-stu-id="5a84e-123">DuplicatedPriority</span></span>
    
- <span data-ttu-id="5a84e-124">DuplicatedOperationOnTheSameRule</span><span class="sxs-lookup"><span data-stu-id="5a84e-124">DuplicatedOperationOnTheSameRule</span></span>
    
- <span data-ttu-id="5a84e-125">FolderDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="5a84e-125">FolderDoesNotExist</span></span>
    
- <span data-ttu-id="5a84e-126">InvalidAddress</span><span class="sxs-lookup"><span data-stu-id="5a84e-126">InvalidAddress</span></span>
    
- <span data-ttu-id="5a84e-127">InvalidDateRange</span><span class="sxs-lookup"><span data-stu-id="5a84e-127">InvalidDateRange</span></span>
    
- <span data-ttu-id="5a84e-128">InvalidFolderId</span><span class="sxs-lookup"><span data-stu-id="5a84e-128">InvalidFolderId</span></span>
    
- <span data-ttu-id="5a84e-129">InvalidSizeRange</span><span class="sxs-lookup"><span data-stu-id="5a84e-129">InvalidSizeRange</span></span>
    
- <span data-ttu-id="5a84e-130">Inválidos</span><span class="sxs-lookup"><span data-stu-id="5a84e-130">InvalidValue</span></span>
    
- <span data-ttu-id="5a84e-131">MessageClassificationNotFound</span><span class="sxs-lookup"><span data-stu-id="5a84e-131">MessageClassificationNotFound</span></span>
    
- <span data-ttu-id="5a84e-132">Faltandoaction</span><span class="sxs-lookup"><span data-stu-id="5a84e-132">MissingAction</span></span>
    
- <span data-ttu-id="5a84e-133">MissingParameter</span><span class="sxs-lookup"><span data-stu-id="5a84e-133">MissingParameter</span></span>
    
- <span data-ttu-id="5a84e-134">MissingRangeValue</span><span class="sxs-lookup"><span data-stu-id="5a84e-134">MissingRangeValue</span></span>
    
- <span data-ttu-id="5a84e-135">Não condefinida</span><span class="sxs-lookup"><span data-stu-id="5a84e-135">NotSettable</span></span>
    
- <span data-ttu-id="5a84e-136">RecipientDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="5a84e-136">RecipientDoesNotExist</span></span>
    
- <span data-ttu-id="5a84e-137">RuleNotFound</span><span class="sxs-lookup"><span data-stu-id="5a84e-137">RuleNotFound</span></span>
    
- <span data-ttu-id="5a84e-138">SizeLessThanZero</span><span class="sxs-lookup"><span data-stu-id="5a84e-138">SizeLessThanZero</span></span>
    
- <span data-ttu-id="5a84e-139">StringValueTooBig</span><span class="sxs-lookup"><span data-stu-id="5a84e-139">StringValueTooBig</span></span>
    
- <span data-ttu-id="5a84e-140">UnsupportedAddress</span><span class="sxs-lookup"><span data-stu-id="5a84e-140">UnsupportedAddress</span></span>
    
- <span data-ttu-id="5a84e-141">UnexpectedError</span><span class="sxs-lookup"><span data-stu-id="5a84e-141">UnexpectedError</span></span>
    
- <span data-ttu-id="5a84e-142">UnsupportedRule</span><span class="sxs-lookup"><span data-stu-id="5a84e-142">UnsupportedRule</span></span>
    
## <a name="remarks"></a><span data-ttu-id="5a84e-143">Comentários</span><span class="sxs-lookup"><span data-stu-id="5a84e-143">Remarks</span></span>

<span data-ttu-id="5a84e-144">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a84e-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a84e-145">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5a84e-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a84e-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="5a84e-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5a84e-147">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5a84e-147">Schema Name</span></span>  <br/> |<span data-ttu-id="5a84e-148">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5a84e-148">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5a84e-149">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5a84e-149">Validation File</span></span>  <br/> |<span data-ttu-id="5a84e-150">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5a84e-150">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5a84e-151">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5a84e-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a84e-152">False</span><span class="sxs-lookup"><span data-stu-id="5a84e-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a84e-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="5a84e-153">See also</span></span>



- [<span data-ttu-id="5a84e-154">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5a84e-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

