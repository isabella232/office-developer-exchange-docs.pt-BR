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
description: O elemento Condition identifica a condição que deve ser satisfeita para a parte de ação da regra a ser executada.
ms.openlocfilehash: 2aea11197f072a4dbe21292bb47075d6f273d31b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463220"
---
# <a name="condition"></a><span data-ttu-id="9ff64-103">Condição</span><span class="sxs-lookup"><span data-stu-id="9ff64-103">Condition</span></span>

<span data-ttu-id="9ff64-104">O elemento **Condition** identifica a condição que deve ser satisfeita para a parte de ação da regra a ser executada.</span><span class="sxs-lookup"><span data-stu-id="9ff64-104">The **Condition** element identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span> 
  
```xml
<Condition>
   <AllInternal/>
</Condition>
```

```xml
<Condition> 
    <SenderDepartments/> 
</Condition>
```

```xml
<Condition> 
    <True/> 
</Condition>
```

```xml
<Condition> 
    <Recipients/> 
</Condition>
```

```xml
<Condition> 
    <And/> 
</Condition>
```

<span data-ttu-id="9ff64-105">**ProtectionRuleConditionType**</span><span class="sxs-lookup"><span data-stu-id="9ff64-105">**ProtectionRuleConditionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9ff64-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9ff64-106">Attributes and elements</span></span>

<span data-ttu-id="9ff64-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9ff64-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ff64-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9ff64-108">Attributes</span></span>

<span data-ttu-id="9ff64-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ff64-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ff64-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9ff64-110">Child elements</span></span>

|<span data-ttu-id="9ff64-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9ff64-111">**Element**</span></span>|<span data-ttu-id="9ff64-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9ff64-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ff64-113">Interno</span><span class="sxs-lookup"><span data-stu-id="9ff64-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="9ff64-114">Avalia como **true** se todos os destinatários de uma mensagem de email são internos à organização do remetente.</span><span class="sxs-lookup"><span data-stu-id="9ff64-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|[<span data-ttu-id="9ff64-115">E (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="9ff64-115">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="9ff64-116">Especifica que todos os elementos filho devem corresponder para serem avaliados como **true**.</span><span class="sxs-lookup"><span data-stu-id="9ff64-116">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="9ff64-117">Especifica que deve haver mais de uma condição filha de regra de proteção.</span><span class="sxs-lookup"><span data-stu-id="9ff64-117">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
|[<span data-ttu-id="9ff64-118">Destinatário</span><span class="sxs-lookup"><span data-stu-id="9ff64-118">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="9ff64-119">Especifica que qualquer destinatário da mensagem de email corresponde a qualquer um dos destinatários especificados nos elementos de [valor filho (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="9ff64-119">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="9ff64-120">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="9ff64-120">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="9ff64-121">Especifica que o departamento do remetente corresponde a qualquer um dos departamentos especificados nos elementos de [valor filho (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="9ff64-121">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="9ff64-122">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="9ff64-122">True</span></span>](true.md) <br/> |<span data-ttu-id="9ff64-123">Especifica uma condição que sempre corresponde.</span><span class="sxs-lookup"><span data-stu-id="9ff64-123">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ff64-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9ff64-124">Parent elements</span></span>

|<span data-ttu-id="9ff64-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9ff64-125">**Element**</span></span>|<span data-ttu-id="9ff64-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9ff64-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ff64-127">Rule</span><span class="sxs-lookup"><span data-stu-id="9ff64-127">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="9ff64-128">Contém uma única regra de proteção.</span><span class="sxs-lookup"><span data-stu-id="9ff64-128">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9ff64-129">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="9ff64-129">Text value</span></span>

<span data-ttu-id="9ff64-130">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9ff64-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9ff64-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="9ff64-131">Remarks</span></span>

<span data-ttu-id="9ff64-132">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9ff64-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ff64-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9ff64-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ff64-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="9ff64-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9ff64-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9ff64-135">Schema Name</span></span>  <br/> |<span data-ttu-id="9ff64-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9ff64-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="9ff64-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9ff64-137">Validation File</span></span>  <br/> |<span data-ttu-id="9ff64-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9ff64-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9ff64-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9ff64-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ff64-140">False</span><span class="sxs-lookup"><span data-stu-id="9ff64-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ff64-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="9ff64-141">See also</span></span>

- [<span data-ttu-id="9ff64-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9ff64-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

