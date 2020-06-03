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
description: O elemento SenderDepartments especifica que o departamento do remetente corresponde a qualquer um dos departamentos especificados nos elementos de valor filho (ProtectionRuleValueType).
ms.openlocfilehash: cf15b974b9c0cfb09767661f17334defc4041e43
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530342"
---
# <a name="senderdepartments"></a><span data-ttu-id="fe48a-103">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="fe48a-103">SenderDepartments</span></span>

<span data-ttu-id="fe48a-104">O elemento **SenderDepartments** especifica que o departamento do remetente corresponde a qualquer um dos departamentos especificados nos elementos de [valor filho (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="fe48a-104">The **SenderDepartments** element specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span> 
  
```XML
<SenderDepartments>
   <Value/>
</SenderDepartments>
```

 <span data-ttu-id="fe48a-105">**ProtectionRuleSenderDepartmentsType**</span><span class="sxs-lookup"><span data-stu-id="fe48a-105">**ProtectionRuleSenderDepartmentsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fe48a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fe48a-106">Attributes and elements</span></span>

<span data-ttu-id="fe48a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fe48a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fe48a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fe48a-108">Attributes</span></span>

<span data-ttu-id="fe48a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fe48a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fe48a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fe48a-110">Child elements</span></span>

|<span data-ttu-id="fe48a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fe48a-111">**Element**</span></span>|<span data-ttu-id="fe48a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fe48a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe48a-113">Valor (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="fe48a-113">Value (ProtectionRuleValueType)</span></span>](value-protectionrulevaluetype.md) <br/> |<span data-ttu-id="fe48a-114">Identifica um único departamento de remetente.</span><span class="sxs-lookup"><span data-stu-id="fe48a-114">Identifies a single sender department.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fe48a-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fe48a-115">Parent elements</span></span>

|<span data-ttu-id="fe48a-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fe48a-116">**Element**</span></span>|<span data-ttu-id="fe48a-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fe48a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe48a-118">Condição</span><span class="sxs-lookup"><span data-stu-id="fe48a-118">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="fe48a-119">Identifica a condição que deve ser satisfeita para a parte de ação da regra a ser executada.</span><span class="sxs-lookup"><span data-stu-id="fe48a-119">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="fe48a-120">E (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="fe48a-120">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="fe48a-121">Especifica que todos os elementos filho devem corresponder para serem avaliados como **true**.</span><span class="sxs-lookup"><span data-stu-id="fe48a-121">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="fe48a-122">Especifica que deve haver mais de uma condição filha de regra de proteção.</span><span class="sxs-lookup"><span data-stu-id="fe48a-122">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fe48a-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="fe48a-123">Remarks</span></span>

<span data-ttu-id="fe48a-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe48a-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fe48a-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fe48a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fe48a-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="fe48a-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fe48a-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fe48a-127">Schema Name</span></span>  <br/> |<span data-ttu-id="fe48a-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="fe48a-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="fe48a-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fe48a-129">Validation File</span></span>  <br/> |<span data-ttu-id="fe48a-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fe48a-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fe48a-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fe48a-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="fe48a-132">False</span><span class="sxs-lookup"><span data-stu-id="fe48a-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fe48a-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="fe48a-133">See also</span></span>



- [<span data-ttu-id="fe48a-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fe48a-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

