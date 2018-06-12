---
title: Condição
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Condition
api_type:
- schema
ms.assetid: 0790a3f2-cb31-4036-a757-7821aa0722cb
description: O elemento de condição identifica a condição que deve ser atendida para a parte de ação da regra a ser executada.
ms.openlocfilehash: ed605946f99aa63416337cd0e731c931176a8ed4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751415"
---
# <a name="condition"></a><span data-ttu-id="302b9-103">Condição</span><span class="sxs-lookup"><span data-stu-id="302b9-103">Condition</span></span>

<span data-ttu-id="302b9-104">O elemento de **condição** identifica a condição que deve ser atendida para a parte de ação da regra a ser executada.</span><span class="sxs-lookup"><span data-stu-id="302b9-104">The **Condition** element identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span> 
  
```xml
<Condition>
   <AllInternal/>
</Condition>
```

 <span data-ttu-id="302b9-105">**ProtectionRuleConditionType**</span><span class="sxs-lookup"><span data-stu-id="302b9-105">**ProtectionRuleConditionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="302b9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="302b9-106">Attributes and elements</span></span>

<span data-ttu-id="302b9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="302b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="302b9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="302b9-108">Attributes</span></span>

<span data-ttu-id="302b9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="302b9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="302b9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="302b9-110">Child elements</span></span>

|<span data-ttu-id="302b9-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="302b9-111">**Element**</span></span>|<span data-ttu-id="302b9-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="302b9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="302b9-113">AllInternal</span><span class="sxs-lookup"><span data-stu-id="302b9-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="302b9-114">Avaliado como **verdadeiro** se todos os destinatários de uma mensagem de email são internos para a organização do remetente.</span><span class="sxs-lookup"><span data-stu-id="302b9-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|[<span data-ttu-id="302b9-115">E (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="302b9-115">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="302b9-116">Especifica que todos os elementos filho devem corresponder para avaliar como **true**.</span><span class="sxs-lookup"><span data-stu-id="302b9-116">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="302b9-117">Especifica se deve haver mais de uma condição de filho de regra de proteção.</span><span class="sxs-lookup"><span data-stu-id="302b9-117">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
|[<span data-ttu-id="302b9-118">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="302b9-118">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="302b9-119">Especifica que qualquer destinatário da mensagem de email corresponde a qualquer um dos destinatários especificados nos elementos filho [valor (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="302b9-119">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="302b9-120">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="302b9-120">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="302b9-121">Especifica se o departamento do remetente corresponde a um dos departamentos especificados nos elementos filho [valor (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="302b9-121">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="302b9-122">True</span><span class="sxs-lookup"><span data-stu-id="302b9-122">True</span></span>](true.md) <br/> |<span data-ttu-id="302b9-123">Especifica uma condição que corresponda sempre.</span><span class="sxs-lookup"><span data-stu-id="302b9-123">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="302b9-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="302b9-124">Parent elements</span></span>

|<span data-ttu-id="302b9-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="302b9-125">**Element**</span></span>|<span data-ttu-id="302b9-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="302b9-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="302b9-127">Rule</span><span class="sxs-lookup"><span data-stu-id="302b9-127">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="302b9-128">Contém uma regra de proteção do único.</span><span class="sxs-lookup"><span data-stu-id="302b9-128">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="302b9-129">Text value</span><span class="sxs-lookup"><span data-stu-id="302b9-129">Text value</span></span>

<span data-ttu-id="302b9-130">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="302b9-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="302b9-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="302b9-131">Remarks</span></span>

<span data-ttu-id="302b9-132">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="302b9-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="302b9-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="302b9-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="302b9-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="302b9-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="302b9-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="302b9-135">Schema Name</span></span>  <br/> |<span data-ttu-id="302b9-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="302b9-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="302b9-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="302b9-137">Validation File</span></span>  <br/> |<span data-ttu-id="302b9-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="302b9-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="302b9-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="302b9-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="302b9-140">False</span><span class="sxs-lookup"><span data-stu-id="302b9-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="302b9-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="302b9-141">See also</span></span>



- [<span data-ttu-id="302b9-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="302b9-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

