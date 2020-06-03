---
title: ValidationErrors
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ValidationErrors
api_type:
- schema
ms.assetid: 009526aa-22e7-4f5c-be88-079175aa9122
description: O elemento ValidationErrors representa uma matriz de erros de validação de regra em cada campo de regra que possui um erro.
ms.openlocfilehash: 0861425b04e03a3e2e54a47a5027d0a11264392d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530272"
---
# <a name="validationerrors"></a><span data-ttu-id="c91b1-103">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="c91b1-103">ValidationErrors</span></span>

<span data-ttu-id="c91b1-104">O elemento **ValidationErrors** representa uma matriz de erros de validação de regra em cada campo de regra que possui um erro.</span><span class="sxs-lookup"><span data-stu-id="c91b1-104">The **ValidationErrors** element represents an array of rule validation errors on each rule field that has an error.</span></span> 
  
```XML
<VaidationErrors>
   <Error/>
</ValidationErrors>
```

 <span data-ttu-id="c91b1-105">**ArrayOfRuleValidationErrorsType**</span><span class="sxs-lookup"><span data-stu-id="c91b1-105">**ArrayOfRuleValidationErrorsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c91b1-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c91b1-106">Attributes and elements</span></span>

<span data-ttu-id="c91b1-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c91b1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c91b1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c91b1-108">Attributes</span></span>

<span data-ttu-id="c91b1-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c91b1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c91b1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c91b1-110">Child elements</span></span>

|<span data-ttu-id="c91b1-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c91b1-111">**Element**</span></span>|<span data-ttu-id="c91b1-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c91b1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c91b1-113">Erro</span><span class="sxs-lookup"><span data-stu-id="c91b1-113">Error</span></span>](error.md) <br/> |<span data-ttu-id="c91b1-114">Representa um erro de validação única em um valor da propriedade regra específica, o valor da propriedade predicado ou o valor da propriedade action</span><span class="sxs-lookup"><span data-stu-id="c91b1-114">Represents a single validation error on a particular rule property value, predicate property value, or action property value</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c91b1-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c91b1-115">Parent elements</span></span>

|<span data-ttu-id="c91b1-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c91b1-116">**Element**</span></span>|<span data-ttu-id="c91b1-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c91b1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c91b1-118">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="c91b1-118">RuleOperationError</span></span>](ruleoperationerror.md) <br/> |<span data-ttu-id="c91b1-119">Representa um erro de operação de regra.</span><span class="sxs-lookup"><span data-stu-id="c91b1-119">Represents a rule operation error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c91b1-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c91b1-120">Text value</span></span>

<span data-ttu-id="c91b1-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c91b1-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c91b1-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="c91b1-122">Remarks</span></span>

<span data-ttu-id="c91b1-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c91b1-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c91b1-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c91b1-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c91b1-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="c91b1-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c91b1-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c91b1-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c91b1-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c91b1-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c91b1-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c91b1-128">Validation File</span></span>  <br/> |<span data-ttu-id="c91b1-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c91b1-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c91b1-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c91b1-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c91b1-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="c91b1-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c91b1-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="c91b1-132">See also</span></span>



- [<span data-ttu-id="c91b1-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c91b1-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

