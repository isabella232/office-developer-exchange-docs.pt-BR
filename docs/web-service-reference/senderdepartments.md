---
title: SenderDepartments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SenderDepartments
api_type:
- schema
ms.assetid: b016cdde-d597-40ac-87c4-63ca68bd539d
description: O elemento SenderDepartments Especifica se o departamento do remetente corresponde a um dos departamentos especificados nos elementos filho valor (ProtectionRuleValueType).
ms.openlocfilehash: d40e6299bd46ede559cc2cce3bcc9d1611e96bd7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825331"
---
# <a name="senderdepartments"></a><span data-ttu-id="c7d0e-103">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="c7d0e-103">SenderDepartments</span></span>

<span data-ttu-id="c7d0e-104">O elemento **SenderDepartments** Especifica se o departamento do remetente corresponde a um dos departamentos especificados nos elementos filho [valor (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="c7d0e-104">The **SenderDepartments** element specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span> 
  
```XML
<SenderDepartments>
   <Value/>
</SenderDepartments>
```

 <span data-ttu-id="c7d0e-105">**ProtectionRuleSenderDepartmentsType**</span><span class="sxs-lookup"><span data-stu-id="c7d0e-105">**ProtectionRuleSenderDepartmentsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c7d0e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c7d0e-106">Attributes and elements</span></span>

<span data-ttu-id="c7d0e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c7d0e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7d0e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c7d0e-108">Attributes</span></span>

<span data-ttu-id="c7d0e-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c7d0e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c7d0e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c7d0e-110">Child elements</span></span>

|<span data-ttu-id="c7d0e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c7d0e-111">**Element**</span></span>|<span data-ttu-id="c7d0e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c7d0e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7d0e-113">Valor (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="c7d0e-113">Value (ProtectionRuleValueType)</span></span>](value-protectionrulevaluetype.md) <br/> |<span data-ttu-id="c7d0e-114">Identifica um departamento de remetente único.</span><span class="sxs-lookup"><span data-stu-id="c7d0e-114">Identifies a single sender department.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c7d0e-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c7d0e-115">Parent elements</span></span>

|<span data-ttu-id="c7d0e-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c7d0e-116">**Element**</span></span>|<span data-ttu-id="c7d0e-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c7d0e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7d0e-118">Condição</span><span class="sxs-lookup"><span data-stu-id="c7d0e-118">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="c7d0e-119">Identifica a condição que deve ser atendida para a parte de ação da regra a ser executada.</span><span class="sxs-lookup"><span data-stu-id="c7d0e-119">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="c7d0e-120">E (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="c7d0e-120">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="c7d0e-121">Especifica que todos os elementos filho devem corresponder para avaliar como **true**.</span><span class="sxs-lookup"><span data-stu-id="c7d0e-121">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="c7d0e-122">Especifica se deve haver mais de uma condição de filho de regra de proteção.</span><span class="sxs-lookup"><span data-stu-id="c7d0e-122">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c7d0e-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="c7d0e-123">Remarks</span></span>

<span data-ttu-id="c7d0e-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7d0e-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c7d0e-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c7d0e-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7d0e-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="c7d0e-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c7d0e-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c7d0e-127">Schema Name</span></span>  <br/> |<span data-ttu-id="c7d0e-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c7d0e-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="c7d0e-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c7d0e-129">Validation File</span></span>  <br/> |<span data-ttu-id="c7d0e-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c7d0e-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c7d0e-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c7d0e-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="c7d0e-132">False</span><span class="sxs-lookup"><span data-stu-id="c7d0e-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c7d0e-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="c7d0e-133">See also</span></span>



- [<span data-ttu-id="c7d0e-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c7d0e-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

