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
description: O elemento and especifica que todos os elementos filho devem corresponder para serem avaliados como true.
ms.openlocfilehash: ba898ccd77518971afaf713d1c7c7955f46465d5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464732"
---
# <a name="and-protectionruleandtype"></a><span data-ttu-id="0b29f-103">E (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="0b29f-103">And (ProtectionRuleAndType)</span></span>

<span data-ttu-id="0b29f-104">O elemento **and** especifica que todos os elementos filho devem corresponder para serem avaliados como **true**.</span><span class="sxs-lookup"><span data-stu-id="0b29f-104">The **And** element specifies that all child elements must match to evaluate to **true**.</span></span>
  
```xml
<And>
   <AllInternal/>
   <And/>
   <RecipientIs/>
   <SenderDepartments/>
   <True/>
</And>
```

 <span data-ttu-id="0b29f-105">**ProtectionRuleAndType**</span><span class="sxs-lookup"><span data-stu-id="0b29f-105">**ProtectionRuleAndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b29f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0b29f-106">Attributes and elements</span></span>

<span data-ttu-id="0b29f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0b29f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b29f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0b29f-108">Attributes</span></span>

<span data-ttu-id="0b29f-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b29f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b29f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0b29f-110">Child elements</span></span>

|<span data-ttu-id="0b29f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0b29f-111">**Element**</span></span>|<span data-ttu-id="0b29f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b29f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b29f-113">Interno</span><span class="sxs-lookup"><span data-stu-id="0b29f-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="0b29f-114">Avalia como **true** se todos os destinatários de uma mensagem de email são internos à organização do remetente.</span><span class="sxs-lookup"><span data-stu-id="0b29f-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|<span data-ttu-id="0b29f-115">**And**</span><span class="sxs-lookup"><span data-stu-id="0b29f-115">**And**</span></span> <br/> |<span data-ttu-id="0b29f-116">Especifica que todos os elementos filho devem corresponder para serem avaliados como **true**.</span><span class="sxs-lookup"><span data-stu-id="0b29f-116">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
|[<span data-ttu-id="0b29f-117">Destinatário</span><span class="sxs-lookup"><span data-stu-id="0b29f-117">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="0b29f-118">Especifica que qualquer destinatário da mensagem de email corresponde a qualquer um dos destinatários especificados nos elementos de [valor filho (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="0b29f-118">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="0b29f-119">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="0b29f-119">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="0b29f-120">Especifica que o departamento do remetente corresponde a qualquer um dos departamentos especificados nos elementos de [valor filho (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="0b29f-120">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="0b29f-121">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="0b29f-121">True</span></span>](true.md) <br/> |<span data-ttu-id="0b29f-122">Especifica uma condição que sempre corresponde.</span><span class="sxs-lookup"><span data-stu-id="0b29f-122">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b29f-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0b29f-123">Parent elements</span></span>

|<span data-ttu-id="0b29f-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0b29f-124">**Element**</span></span>|<span data-ttu-id="0b29f-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b29f-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b29f-126">Condição</span><span class="sxs-lookup"><span data-stu-id="0b29f-126">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="0b29f-127">Identifica a condição que deve ser satisfeita para a parte de ação da regra a ser executada.</span><span class="sxs-lookup"><span data-stu-id="0b29f-127">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|<span data-ttu-id="0b29f-128">**And**</span><span class="sxs-lookup"><span data-stu-id="0b29f-128">**And**</span></span> <br/> |<span data-ttu-id="0b29f-129">Especifica que todos os elementos filho devem corresponder para serem avaliados como **true**.</span><span class="sxs-lookup"><span data-stu-id="0b29f-129">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0b29f-130">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="0b29f-130">Text value</span></span>

<span data-ttu-id="0b29f-131">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0b29f-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0b29f-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="0b29f-132">Remarks</span></span>

<span data-ttu-id="0b29f-133">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b29f-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b29f-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0b29f-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b29f-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="0b29f-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0b29f-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0b29f-136">Schema Name</span></span>  <br/> |<span data-ttu-id="0b29f-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0b29f-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="0b29f-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0b29f-138">Validation File</span></span>  <br/> |<span data-ttu-id="0b29f-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0b29f-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0b29f-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0b29f-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b29f-141">False</span><span class="sxs-lookup"><span data-stu-id="0b29f-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b29f-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="0b29f-142">See also</span></span>

- [<span data-ttu-id="0b29f-143">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0b29f-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

