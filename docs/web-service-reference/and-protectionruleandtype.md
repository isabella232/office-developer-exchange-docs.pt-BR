---
title: E (ProtectionRuleAndType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- And
api_type:
- schema
ms.assetid: 7fafd1c8-cd29-43a0-b383-f6595f934f48
description: O elemento e especifica que todos os elementos filho devem corresponder para avaliar como true.
ms.openlocfilehash: 9e0128ee3fa2b6ffdc5975946694475afec53c25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751089"
---
# <a name="and-protectionruleandtype"></a><span data-ttu-id="491cb-103">E (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="491cb-103">And (ProtectionRuleAndType)</span></span>

<span data-ttu-id="491cb-104">O elemento **e** Especifica que todos os elementos filho devem corresponder para avaliar como **true**.</span><span class="sxs-lookup"><span data-stu-id="491cb-104">The **And** element specifies that all child elements must match to evaluate to **true**.</span></span>
  
```xml
<And>
   <AllInternal/>
   <And/>
   <RecipientIs/>
   <SenderDepartments/>
   <True/>
</And>
```

 <span data-ttu-id="491cb-105">**ProtectionRuleAndType**</span><span class="sxs-lookup"><span data-stu-id="491cb-105">**ProtectionRuleAndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="491cb-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="491cb-106">Attributes and elements</span></span>

<span data-ttu-id="491cb-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="491cb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="491cb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="491cb-108">Attributes</span></span>

<span data-ttu-id="491cb-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="491cb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="491cb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="491cb-110">Child elements</span></span>

|<span data-ttu-id="491cb-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="491cb-111">**Element**</span></span>|<span data-ttu-id="491cb-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="491cb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="491cb-113">AllInternal</span><span class="sxs-lookup"><span data-stu-id="491cb-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="491cb-114">Avaliado como **verdadeiro** se todos os destinatários de uma mensagem de email são internos para a organização do remetente.</span><span class="sxs-lookup"><span data-stu-id="491cb-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|<span data-ttu-id="491cb-115">**E**</span><span class="sxs-lookup"><span data-stu-id="491cb-115">**And**</span></span> <br/> |<span data-ttu-id="491cb-116">Especifica que todos os elementos filho devem corresponder para avaliar como **true**.</span><span class="sxs-lookup"><span data-stu-id="491cb-116">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
|[<span data-ttu-id="491cb-117">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="491cb-117">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="491cb-118">Especifica que qualquer destinatário da mensagem de email corresponde a qualquer um dos destinatários especificados nos elementos filho [valor (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="491cb-118">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="491cb-119">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="491cb-119">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="491cb-120">Especifica se o departamento do remetente corresponde a um dos departamentos especificados nos elementos filho [valor (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="491cb-120">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="491cb-121">True</span><span class="sxs-lookup"><span data-stu-id="491cb-121">True</span></span>](true.md) <br/> |<span data-ttu-id="491cb-122">Especifica uma condição que corresponda sempre.</span><span class="sxs-lookup"><span data-stu-id="491cb-122">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="491cb-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="491cb-123">Parent elements</span></span>

|<span data-ttu-id="491cb-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="491cb-124">**Element**</span></span>|<span data-ttu-id="491cb-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="491cb-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="491cb-126">Condição</span><span class="sxs-lookup"><span data-stu-id="491cb-126">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="491cb-127">Identifica a condição que deve ser atendida para a parte de ação da regra a ser executada.</span><span class="sxs-lookup"><span data-stu-id="491cb-127">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|<span data-ttu-id="491cb-128">**E**</span><span class="sxs-lookup"><span data-stu-id="491cb-128">**And**</span></span> <br/> |<span data-ttu-id="491cb-129">Especifica que todos os elementos filho devem corresponder para avaliar como **true**.</span><span class="sxs-lookup"><span data-stu-id="491cb-129">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="491cb-130">Text value</span><span class="sxs-lookup"><span data-stu-id="491cb-130">Text value</span></span>

<span data-ttu-id="491cb-131">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="491cb-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="491cb-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="491cb-132">Remarks</span></span>

<span data-ttu-id="491cb-133">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="491cb-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="491cb-134">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="491cb-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="491cb-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="491cb-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="491cb-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="491cb-136">Schema Name</span></span>  <br/> |<span data-ttu-id="491cb-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="491cb-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="491cb-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="491cb-138">Validation File</span></span>  <br/> |<span data-ttu-id="491cb-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="491cb-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="491cb-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="491cb-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="491cb-141">False</span><span class="sxs-lookup"><span data-stu-id="491cb-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="491cb-142">Ver também</span><span class="sxs-lookup"><span data-stu-id="491cb-142">See also</span></span>

- [<span data-ttu-id="491cb-143">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="491cb-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

