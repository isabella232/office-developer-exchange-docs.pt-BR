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
ms.openlocfilehash: b5e0105a1fdb1564b3115a4c3a8411019f725483
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44464956"
---
# <a name="ruleoperationerror"></a><span data-ttu-id="01696-103">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="01696-103">RuleOperationError</span></span>

<span data-ttu-id="01696-104">O elemento **RuleOperationError** representa um erro de operação de regra.</span><span class="sxs-lookup"><span data-stu-id="01696-104">The **RuleOperationError** element represents a rule operation error.</span></span> 
  
```XML
<RuleOperationError>
    <OperationIndex/>
    <ValidationErrors/>
</RuleOperationError>
```

 <span data-ttu-id="01696-105">**RuleOperationErrorType**</span><span class="sxs-lookup"><span data-stu-id="01696-105">**RuleOperationErrorType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01696-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="01696-106">Attributes and elements</span></span>

<span data-ttu-id="01696-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="01696-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01696-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="01696-108">Attributes</span></span>

<span data-ttu-id="01696-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="01696-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01696-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="01696-110">Child elements</span></span>

|<span data-ttu-id="01696-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="01696-111">**Element**</span></span>|<span data-ttu-id="01696-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="01696-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01696-113">OperationIndex</span><span class="sxs-lookup"><span data-stu-id="01696-113">OperationIndex</span></span>](operationindex.md) <br/> |<span data-ttu-id="01696-114">Indica o índice da operação na solicitação que causou o erro de operação de regra.</span><span class="sxs-lookup"><span data-stu-id="01696-114">Indicates the index of the operation in the request that caused the rule operation error.</span></span>  <br/> |
|[<span data-ttu-id="01696-115">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="01696-115">ValidationErrors</span></span>](validationerrors.md) <br/> |<span data-ttu-id="01696-116">Representa uma matriz de erros de validação de regra em cada campo de regra que possui um erro.</span><span class="sxs-lookup"><span data-stu-id="01696-116">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="01696-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="01696-117">Parent elements</span></span>

|<span data-ttu-id="01696-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="01696-118">**Element**</span></span>|<span data-ttu-id="01696-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="01696-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01696-120">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="01696-120">RuleOperationErrors</span></span>](ruleoperationerrors.md) <br/> |<span data-ttu-id="01696-121">Representa uma matriz de erros de validação de regra em cada campo de regra que possui um erro.</span><span class="sxs-lookup"><span data-stu-id="01696-121">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="01696-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="01696-122">Text value</span></span>

<span data-ttu-id="01696-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="01696-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="01696-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="01696-124">Remarks</span></span>

<span data-ttu-id="01696-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="01696-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01696-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="01696-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01696-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="01696-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="01696-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="01696-128">Schema Name</span></span>  <br/> |<span data-ttu-id="01696-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="01696-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="01696-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="01696-130">Validation File</span></span>  <br/> |<span data-ttu-id="01696-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="01696-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="01696-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="01696-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="01696-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="01696-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01696-134">Também consulte</span><span class="sxs-lookup"><span data-stu-id="01696-134">See also</span></span>



- [<span data-ttu-id="01696-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="01696-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

