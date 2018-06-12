---
title: RuleOperationError
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RuleOperationError
api_type:
- schema
ms.assetid: b447e610-d37c-40d3-9158-aa108a9f248e
description: O elemento RuleOperationError representa um erro de operação de regra.
ms.openlocfilehash: ff42addea0f55b13794e2c910d4d865ad0b17bc3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825265"
---
# <a name="ruleoperationerror"></a><span data-ttu-id="4084f-103">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="4084f-103">RuleOperationError</span></span>

<span data-ttu-id="4084f-104">O elemento **RuleOperationError** representa um erro de operação de regra.</span><span class="sxs-lookup"><span data-stu-id="4084f-104">The **RuleOperationError** element represents a rule operation error.</span></span> 
  
```XML
<RuleOperationError>
    <OperationIndex/>
    <ValidationErrors/>
</RuleOperationError>
```

 <span data-ttu-id="4084f-105">**RuleOperationErrorType**</span><span class="sxs-lookup"><span data-stu-id="4084f-105">**RuleOperationErrorType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4084f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4084f-106">Attributes and elements</span></span>

<span data-ttu-id="4084f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4084f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4084f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4084f-108">Attributes</span></span>

<span data-ttu-id="4084f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4084f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4084f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4084f-110">Child elements</span></span>

|<span data-ttu-id="4084f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4084f-111">**Element**</span></span>|<span data-ttu-id="4084f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4084f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4084f-113">OperationIndex</span><span class="sxs-lookup"><span data-stu-id="4084f-113">OperationIndex</span></span>](operationindex.md) <br/> |<span data-ttu-id="4084f-114">Indica o índice da operação na solicitação que causou o erro de operação de regra.</span><span class="sxs-lookup"><span data-stu-id="4084f-114">Indicates the index of the operation in the request that caused the rule operation error.</span></span>  <br/> |
|[<span data-ttu-id="4084f-115">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="4084f-115">ValidationErrors</span></span>](validationerrors.md) <br/> |<span data-ttu-id="4084f-116">Representa uma matriz de erros de validação de regra em cada campo de regra que possui um erro.</span><span class="sxs-lookup"><span data-stu-id="4084f-116">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4084f-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4084f-117">Parent elements</span></span>

|<span data-ttu-id="4084f-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4084f-118">**Element**</span></span>|<span data-ttu-id="4084f-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4084f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4084f-120">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="4084f-120">RuleOperationErrors</span></span>](ruleoperationerrors.md) <br/> |<span data-ttu-id="4084f-121">Representa uma matriz de erros de validação de regra em cada campo de regra que possui um erro.</span><span class="sxs-lookup"><span data-stu-id="4084f-121">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4084f-122">Text value</span><span class="sxs-lookup"><span data-stu-id="4084f-122">Text value</span></span>

<span data-ttu-id="4084f-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4084f-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4084f-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="4084f-124">Remarks</span></span>

<span data-ttu-id="4084f-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4084f-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4084f-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4084f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4084f-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="4084f-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4084f-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4084f-128">Schema Name</span></span>  <br/> |<span data-ttu-id="4084f-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="4084f-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4084f-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4084f-130">Validation File</span></span>  <br/> |<span data-ttu-id="4084f-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4084f-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4084f-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4084f-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="4084f-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="4084f-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4084f-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="4084f-134">See also</span></span>



- [<span data-ttu-id="4084f-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4084f-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

