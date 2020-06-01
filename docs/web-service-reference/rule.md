---
title: Rule
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rule
api_type:
- schema
ms.assetid: c30f3851-bd56-4473-9106-dc85e9619486
description: O elemento Rule contém uma única regra de proteção.
ms.openlocfilehash: 6c18a2bd026893cd333bc7007203abf04a6f0be7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44464998"
---
# <a name="rule"></a><span data-ttu-id="ff7d6-103">Rule</span><span class="sxs-lookup"><span data-stu-id="ff7d6-103">Rule</span></span>

<span data-ttu-id="ff7d6-104">O elemento **Rule** contém uma única regra de proteção.</span><span class="sxs-lookup"><span data-stu-id="ff7d6-104">The **Rule** element contains a single protection rule.</span></span> 
  
```XML
<Rule Name="" UserOverridable=="" Priority="">
   <Condition/>
   <Action/>
</Rule>
```

 <span data-ttu-id="ff7d6-105">**ProtectionRuleType**</span><span class="sxs-lookup"><span data-stu-id="ff7d6-105">**ProtectionRuleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff7d6-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ff7d6-106">Attributes and elements</span></span>

<span data-ttu-id="ff7d6-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ff7d6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff7d6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ff7d6-108">Attributes</span></span>

|<span data-ttu-id="ff7d6-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="ff7d6-109">**Attribute**</span></span>|<span data-ttu-id="ff7d6-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ff7d6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ff7d6-111">**Nome**</span><span class="sxs-lookup"><span data-stu-id="ff7d6-111">**Name**</span></span> <br/> |<span data-ttu-id="ff7d6-112">Identifica o nome da regra.</span><span class="sxs-lookup"><span data-stu-id="ff7d6-112">Identifies the name of the rule.</span></span> <span data-ttu-id="ff7d6-113">Um atributo necessário do tipo cadeia de caracteres com um tamanho mínimo de 1.</span><span class="sxs-lookup"><span data-stu-id="ff7d6-113">A required attribute of type string with a minimum length of 1.</span></span>  <br/> |
|<span data-ttu-id="ff7d6-114">**Useroverridable**</span><span class="sxs-lookup"><span data-stu-id="ff7d6-114">**UserOverridable**</span></span> <br/> |<span data-ttu-id="ff7d6-115">Especifica se a regra é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="ff7d6-115">Specifies whether the rule is mandatory.</span></span> <span data-ttu-id="ff7d6-116">Se a regra for obrigatória, esse valor de atributo deve ser **false**.</span><span class="sxs-lookup"><span data-stu-id="ff7d6-116">If the rule is mandatory, this attribute value must be **false**.</span></span> <span data-ttu-id="ff7d6-117">Um atributo necessário do tipo Boolean.</span><span class="sxs-lookup"><span data-stu-id="ff7d6-117">A required attribute of type Boolean.</span></span>  <br/> |
|<span data-ttu-id="ff7d6-118">**Prioridade**</span><span class="sxs-lookup"><span data-stu-id="ff7d6-118">**Priority**</span></span> <br/> |<span data-ttu-id="ff7d6-119">Especifica a prioridade da regra.</span><span class="sxs-lookup"><span data-stu-id="ff7d6-119">Specifies the rule priority.</span></span> <span data-ttu-id="ff7d6-120">Um atributo necessário do tipo int com um valor mínimo de 1.</span><span class="sxs-lookup"><span data-stu-id="ff7d6-120">A required attribute of type int with a minimum value of 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ff7d6-121">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ff7d6-121">Child elements</span></span>

|<span data-ttu-id="ff7d6-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ff7d6-122">**Element**</span></span>|<span data-ttu-id="ff7d6-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ff7d6-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff7d6-124">Condição</span><span class="sxs-lookup"><span data-stu-id="ff7d6-124">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="ff7d6-125">Identifica a condição que deve ser satisfeita para a parte de ação da regra a ser executada.</span><span class="sxs-lookup"><span data-stu-id="ff7d6-125">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="ff7d6-126">Ação (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="ff7d6-126">Action (ProtectionRuleActionType)</span></span>](action-protectionruleactiontype.md) <br/> |<span data-ttu-id="ff7d6-127">Identifica qual ação deve ser executada se a condição da condição da regra corresponder.</span><span class="sxs-lookup"><span data-stu-id="ff7d6-127">Identifies what action must be executed if the condition part of the rule matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ff7d6-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ff7d6-128">Parent elements</span></span>

|<span data-ttu-id="ff7d6-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ff7d6-129">**Element**</span></span>|<span data-ttu-id="ff7d6-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ff7d6-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff7d6-131">Regras</span><span class="sxs-lookup"><span data-stu-id="ff7d6-131">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ff7d6-132">Contém uma matriz de regras de proteção.</span><span class="sxs-lookup"><span data-stu-id="ff7d6-132">Contains an array of protection rules.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ff7d6-133">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ff7d6-133">Text value</span></span>

<span data-ttu-id="ff7d6-134">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ff7d6-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ff7d6-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="ff7d6-135">Remarks</span></span>

<span data-ttu-id="ff7d6-136">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff7d6-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff7d6-137">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ff7d6-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff7d6-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="ff7d6-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ff7d6-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ff7d6-139">Schema Name</span></span>  <br/> |<span data-ttu-id="ff7d6-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ff7d6-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="ff7d6-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ff7d6-141">Validation File</span></span>  <br/> |<span data-ttu-id="ff7d6-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ff7d6-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ff7d6-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ff7d6-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff7d6-144">False</span><span class="sxs-lookup"><span data-stu-id="ff7d6-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff7d6-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="ff7d6-145">See also</span></span>



- [<span data-ttu-id="ff7d6-146">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ff7d6-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

