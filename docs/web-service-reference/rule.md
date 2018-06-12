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
description: O elemento de regra contém uma regra de proteção do único.
ms.openlocfilehash: 9abbb70381c214211172d2d5ba1ed43ee4797f17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825263"
---
# <a name="rule"></a><span data-ttu-id="61343-103">Rule</span><span class="sxs-lookup"><span data-stu-id="61343-103">Rule</span></span>

<span data-ttu-id="61343-104">O elemento de **regra** contém uma regra de proteção do único.</span><span class="sxs-lookup"><span data-stu-id="61343-104">The **Rule** element contains a single protection rule.</span></span> 
  
```XML
<Rule Name="" UserOverridable=="" Priority="">
   <Condition/>
   <Action/>
</Rule>
```

 <span data-ttu-id="61343-105">**ProtectionRuleType**</span><span class="sxs-lookup"><span data-stu-id="61343-105">**ProtectionRuleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61343-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="61343-106">Attributes and elements</span></span>

<span data-ttu-id="61343-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="61343-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61343-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="61343-108">Attributes</span></span>

|<span data-ttu-id="61343-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="61343-109">**Attribute**</span></span>|<span data-ttu-id="61343-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="61343-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="61343-111">**Name**</span><span class="sxs-lookup"><span data-stu-id="61343-111">**Name**</span></span> <br/> |<span data-ttu-id="61343-112">Identifica o nome da regra.</span><span class="sxs-lookup"><span data-stu-id="61343-112">Identifies the name of the rule.</span></span> <span data-ttu-id="61343-113">Um atributo necessário do tipo cadeia de caracteres com um tamanho mínimo de 1.</span><span class="sxs-lookup"><span data-stu-id="61343-113">A required attribute of type string with a minimum length of 1.</span></span>  <br/> |
|<span data-ttu-id="61343-114">**UserOverridable**</span><span class="sxs-lookup"><span data-stu-id="61343-114">**UserOverridable**</span></span> <br/> |<span data-ttu-id="61343-115">Especifica se a regra é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="61343-115">Specifies whether the rule is mandatory.</span></span> <span data-ttu-id="61343-116">Se a regra é obrigatória, este valor do atributo deve ser **false**.</span><span class="sxs-lookup"><span data-stu-id="61343-116">If the rule is mandatory, this attribute value must be **false**.</span></span> <span data-ttu-id="61343-117">Um atributo necessário do tipo booleano.</span><span class="sxs-lookup"><span data-stu-id="61343-117">A required attribute of type Boolean.</span></span>  <br/> |
|<span data-ttu-id="61343-118">**Priority**</span><span class="sxs-lookup"><span data-stu-id="61343-118">**Priority**</span></span> <br/> |<span data-ttu-id="61343-119">Especifica a prioridade da regra.</span><span class="sxs-lookup"><span data-stu-id="61343-119">Specifies the rule priority.</span></span> <span data-ttu-id="61343-120">Um atributo necessário do tipo int com um valor mínimo de 1.</span><span class="sxs-lookup"><span data-stu-id="61343-120">A required attribute of type int with a minimum value of 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="61343-121">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="61343-121">Child elements</span></span>

|<span data-ttu-id="61343-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="61343-122">**Element**</span></span>|<span data-ttu-id="61343-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="61343-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61343-124">Condição</span><span class="sxs-lookup"><span data-stu-id="61343-124">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="61343-125">Identifica a condição que deve ser atendida para a parte de ação da regra a ser executada.</span><span class="sxs-lookup"><span data-stu-id="61343-125">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="61343-126">Ação (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="61343-126">Action (ProtectionRuleActionType)</span></span>](action-protectionruleactiontype.md) <br/> |<span data-ttu-id="61343-127">Identifica a ação que deve ser executada se corresponder a parte de condição da regra.</span><span class="sxs-lookup"><span data-stu-id="61343-127">Identifies what action must be executed if the condition part of the rule matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="61343-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="61343-128">Parent elements</span></span>

|<span data-ttu-id="61343-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="61343-129">**Element**</span></span>|<span data-ttu-id="61343-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="61343-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61343-131">Regras</span><span class="sxs-lookup"><span data-stu-id="61343-131">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="61343-132">Contém uma matriz de regras de proteção.</span><span class="sxs-lookup"><span data-stu-id="61343-132">Contains an array of protection rules.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="61343-133">Text value</span><span class="sxs-lookup"><span data-stu-id="61343-133">Text value</span></span>

<span data-ttu-id="61343-134">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="61343-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="61343-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="61343-135">Remarks</span></span>

<span data-ttu-id="61343-136">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="61343-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61343-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="61343-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61343-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="61343-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="61343-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="61343-139">Schema Name</span></span>  <br/> |<span data-ttu-id="61343-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="61343-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="61343-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="61343-141">Validation File</span></span>  <br/> |<span data-ttu-id="61343-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="61343-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="61343-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="61343-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="61343-144">False</span><span class="sxs-lookup"><span data-stu-id="61343-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="61343-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="61343-145">See also</span></span>



- [<span data-ttu-id="61343-146">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="61343-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

