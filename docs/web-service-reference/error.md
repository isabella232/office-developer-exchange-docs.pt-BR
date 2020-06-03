---
title: Erro
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Error
api_type:
- schema
ms.assetid: b1f54673-578a-496b-99f5-0fde2c669278
description: O elemento error representa um único erro de validação em um valor de propriedade de regra específico, valor da propriedade Predicate ou valor da propriedade Action.
ms.openlocfilehash: 9c28f63aa79446d89152868c81c85ffa7b3a8b39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460677"
---
# <a name="error"></a><span data-ttu-id="aec8a-103">Erro</span><span class="sxs-lookup"><span data-stu-id="aec8a-103">Error</span></span>

<span data-ttu-id="aec8a-104">O elemento **Error** representa um único erro de validação em um valor de propriedade de regra específico, valor da propriedade Predicate ou valor da propriedade Action.</span><span class="sxs-lookup"><span data-stu-id="aec8a-104">The **Error** element represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span> 
  
```XML
<Error>
   <FieldUri/>
   <ErrorCode/>
   <ErrorMessage/>
   <FieldValue/>
</Error>
```

 <span data-ttu-id="aec8a-105">**RuleValidationErrorType**</span><span class="sxs-lookup"><span data-stu-id="aec8a-105">**RuleValidationErrorType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aec8a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="aec8a-106">Attributes and elements</span></span>

<span data-ttu-id="aec8a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="aec8a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aec8a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="aec8a-108">Attributes</span></span>

<span data-ttu-id="aec8a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aec8a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aec8a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="aec8a-110">Child elements</span></span>

|<span data-ttu-id="aec8a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aec8a-111">**Element**</span></span>|<span data-ttu-id="aec8a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aec8a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aec8a-113">FieldUri (regra)</span><span class="sxs-lookup"><span data-stu-id="aec8a-113">FieldUri (Rule)</span></span>](fielduri-rule.md) <br/> |<span data-ttu-id="aec8a-114">Especifica o URI para o campo de regra que causou o erro de validação.</span><span class="sxs-lookup"><span data-stu-id="aec8a-114">Specifies the URI to the rule field that caused the validation error.</span></span>  <br/> |
|[<span data-ttu-id="aec8a-115">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="aec8a-115">ErrorCode</span></span>](errorcode.md) <br/> |<span data-ttu-id="aec8a-116">Representa um código de erro de validação de regra que descreve o que a validação falhou para cada predicado de regra ou ação.</span><span class="sxs-lookup"><span data-stu-id="aec8a-116">Represents a rule validation error code that describes what failed validation for each rule predicate or action.</span></span>  <br/> |
|[<span data-ttu-id="aec8a-117">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="aec8a-117">ErrorMessage</span></span>](errormessage.md) <br/> |<span data-ttu-id="aec8a-118">Representa o motivo do erro de validação.</span><span class="sxs-lookup"><span data-stu-id="aec8a-118">Represents the reason for the validation error.</span></span>  <br/> |
|[<span data-ttu-id="aec8a-119">FieldValue</span><span class="sxs-lookup"><span data-stu-id="aec8a-119">FieldValue</span></span>](fieldvalue.md) <br/> |<span data-ttu-id="aec8a-120">Representa o valor do campo que causou o erro de validação.</span><span class="sxs-lookup"><span data-stu-id="aec8a-120">Represents the value of the field that caused the validation error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aec8a-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="aec8a-121">Parent elements</span></span>

|<span data-ttu-id="aec8a-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aec8a-122">**Element**</span></span>|<span data-ttu-id="aec8a-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aec8a-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aec8a-124">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="aec8a-124">ValidationErrors</span></span>](validationerrors.md) <br/> |<span data-ttu-id="aec8a-125">Representa uma matriz de erros de validação de regra em cada campo de regra que possui um erro.</span><span class="sxs-lookup"><span data-stu-id="aec8a-125">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aec8a-126">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="aec8a-126">Text value</span></span>

<span data-ttu-id="aec8a-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aec8a-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aec8a-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="aec8a-128">Remarks</span></span>

<span data-ttu-id="aec8a-129">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="aec8a-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aec8a-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="aec8a-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aec8a-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="aec8a-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aec8a-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="aec8a-132">Schema Name</span></span>  <br/> |<span data-ttu-id="aec8a-133">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="aec8a-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aec8a-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="aec8a-134">Validation File</span></span>  <br/> |<span data-ttu-id="aec8a-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="aec8a-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aec8a-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="aec8a-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="aec8a-137">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="aec8a-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aec8a-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="aec8a-138">See also</span></span>



- [<span data-ttu-id="aec8a-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="aec8a-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

