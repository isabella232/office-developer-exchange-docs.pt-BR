---
title: RuleOperationErrors
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f15c7b9e-a670-4a11-bb62-2a298c91f142
description: O elemento RuleOperationErrors representa uma matriz de erros de validação de regra em cada campo de regra que possui um erro.
ms.openlocfilehash: d547155f3cbf9eedd0f9bfac7bf3768b3630b50e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44464949"
---
# <a name="ruleoperationerrors"></a><span data-ttu-id="f733e-103">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="f733e-103">RuleOperationErrors</span></span>

<span data-ttu-id="f733e-104">O elemento **RuleOperationErrors** representa uma matriz de erros de validação de regra em cada campo de regra que possui um erro.</span><span class="sxs-lookup"><span data-stu-id="f733e-104">The **RuleOperationErrors** element represents an array of rule validation errors on each rule field that has an error.</span></span> 
  
[<span data-ttu-id="f733e-105">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="f733e-105">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
  
[<span data-ttu-id="f733e-106">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="f733e-106">RuleOperationErrors</span></span>](ruleoperationerrors.md)
  
```XML
<RuleOperationErrors>
    <RuleOperationError>
</RuleOperationErrors>
```

 <span data-ttu-id="f733e-107">**ArrayOfRuleOperationErrorsType**</span><span class="sxs-lookup"><span data-stu-id="f733e-107">**ArrayOfRuleOperationErrorsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f733e-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f733e-108">Attributes and elements</span></span>

<span data-ttu-id="f733e-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f733e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f733e-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="f733e-110">Attributes</span></span>

<span data-ttu-id="f733e-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f733e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f733e-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f733e-112">Child elements</span></span>

|<span data-ttu-id="f733e-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f733e-113">**Element**</span></span>|<span data-ttu-id="f733e-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f733e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f733e-115">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="f733e-115">RuleOperationError</span></span>](ruleoperationerror.md) <br/> |<span data-ttu-id="f733e-116">Representa um erro de operação de regra.</span><span class="sxs-lookup"><span data-stu-id="f733e-116">Represents a rule operation error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f733e-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f733e-117">Parent elements</span></span>

|<span data-ttu-id="f733e-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f733e-118">**Element**</span></span>|<span data-ttu-id="f733e-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f733e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f733e-120">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="f733e-120">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md) <br/> |<span data-ttu-id="f733e-121">Define uma resposta a uma solicitação [UpdateInboxRules](updateinboxrules.md) .</span><span class="sxs-lookup"><span data-stu-id="f733e-121">Defines a response to an [UpdateInboxRules](updateinboxrules.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f733e-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f733e-122">Text value</span></span>

<span data-ttu-id="f733e-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f733e-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f733e-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="f733e-124">Remarks</span></span>

<span data-ttu-id="f733e-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f733e-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f733e-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f733e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f733e-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="f733e-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f733e-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f733e-128">Schema name</span></span>  <br/> |<span data-ttu-id="f733e-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f733e-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f733e-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f733e-130">Validation file</span></span>  <br/> |<span data-ttu-id="f733e-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f733e-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f733e-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f733e-132">Can be empty</span></span>  <br/> |<span data-ttu-id="f733e-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="f733e-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f733e-134">Também consulte</span><span class="sxs-lookup"><span data-stu-id="f733e-134">See also</span></span>



[<span data-ttu-id="f733e-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="f733e-135">UpdateInboxRules</span></span>](updateinboxrules.md)


- [<span data-ttu-id="f733e-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f733e-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

