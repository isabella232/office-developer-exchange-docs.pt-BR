---
title: Regra (RuleType)
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
ms.assetid: 259a1f62-b235-4964-88bf-2d1f1c05a563
description: O elemento Rule contém uma única regra e representa uma regra na caixa de correio de um usuário.
ms.openlocfilehash: cdbd21df235a62a9e201e1eaae1d82a8ac10cdd2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465076"
---
# <a name="rule-ruletype"></a><span data-ttu-id="8cb52-103">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="8cb52-103">Rule (RuleType)</span></span>

<span data-ttu-id="8cb52-104">O elemento **Rule** contém uma única regra e representa uma regra na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8cb52-104">The **Rule** element contains a single rule and represents a rule in a user's mailbox.</span></span> 
  
```XML
<Rule>
    <RuleId>
    <DisplayName>
    <Priority>
    <IsEnabled>
    <IsNotSupported>
    <IsInError>
    <Conditions>
    <Exceptions>
    <Actions>
</Rule>
```

 <span data-ttu-id="8cb52-105">**RuleType**</span><span class="sxs-lookup"><span data-stu-id="8cb52-105">**RuleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8cb52-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8cb52-106">Attributes and elements</span></span>

<span data-ttu-id="8cb52-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8cb52-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8cb52-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8cb52-108">Attributes</span></span>

<span data-ttu-id="8cb52-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8cb52-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8cb52-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8cb52-110">Child elements</span></span>

|<span data-ttu-id="8cb52-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8cb52-111">**Element**</span></span>|<span data-ttu-id="8cb52-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8cb52-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8cb52-113">RuleId</span><span class="sxs-lookup"><span data-stu-id="8cb52-113">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="8cb52-114">Especifica o identificador de regra.</span><span class="sxs-lookup"><span data-stu-id="8cb52-114">Specifies the rule identifier.</span></span>  <br/> |
|[<span data-ttu-id="8cb52-115">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="8cb52-115">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="8cb52-116">Contém o nome de exibição de uma regra.</span><span class="sxs-lookup"><span data-stu-id="8cb52-116">Contains the display name of a rule.</span></span>  <br/> |
|[<span data-ttu-id="8cb52-117">Prioridade</span><span class="sxs-lookup"><span data-stu-id="8cb52-117">Priority</span></span>](priority.md) <br/> |<span data-ttu-id="8cb52-118">Indica a ordem na qual uma regra deve ser executada.</span><span class="sxs-lookup"><span data-stu-id="8cb52-118">Indicates the order in which a rule is to be run.</span></span>  <br/> |
|[<span data-ttu-id="8cb52-119">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="8cb52-119">IsEnabled</span></span>](isenabled.md) <br/> |<span data-ttu-id="8cb52-120">Indica se a regra está habilitada.</span><span class="sxs-lookup"><span data-stu-id="8cb52-120">Indicates whether the rule is enabled.</span></span>  <br/> |
|[<span data-ttu-id="8cb52-121">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="8cb52-121">IsNotSupported</span></span>](isnotsupported.md) <br/> |<span data-ttu-id="8cb52-122">Indica se a regra não pode ser modificada com as APIs de código gerenciado.</span><span class="sxs-lookup"><span data-stu-id="8cb52-122">Indicates whether the rule cannot be modified with the managed code APIs.</span></span>  <br/> |
|[<span data-ttu-id="8cb52-123">IsInError</span><span class="sxs-lookup"><span data-stu-id="8cb52-123">IsInError</span></span>](isinerror.md) <br/> |<span data-ttu-id="8cb52-124">Indica se a regra está em uma condição de erro.</span><span class="sxs-lookup"><span data-stu-id="8cb52-124">Indicates whether the rule is in an error condition.</span></span>  <br/> |
|[<span data-ttu-id="8cb52-125">Condições</span><span class="sxs-lookup"><span data-stu-id="8cb52-125">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="8cb52-126">Identifica as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="8cb52-126">Identifies the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="8cb52-127">Exceções</span><span class="sxs-lookup"><span data-stu-id="8cb52-127">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="8cb52-128">Identifica as exceções que representam todas as condições de exceção de regra disponíveis para a regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="8cb52-128">Identifies the exceptions that represent all the available rule exception conditions for the inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="8cb52-129">Actions</span><span class="sxs-lookup"><span data-stu-id="8cb52-129">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="8cb52-130">Representa as ações a serem realizadas em uma mensagem quando as condições forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="8cb52-130">Represents the actions to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8cb52-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8cb52-131">Parent elements</span></span>

|<span data-ttu-id="8cb52-132">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8cb52-132">**Element**</span></span>|<span data-ttu-id="8cb52-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8cb52-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8cb52-134">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="8cb52-134">CreateRuleOperation</span></span>](createruleoperation.md) <br/> |<span data-ttu-id="8cb52-135">Representa uma operação para criar uma nova regra.</span><span class="sxs-lookup"><span data-stu-id="8cb52-135">Represents an operation to create a new rule.</span></span>  <br/> |
|[<span data-ttu-id="8cb52-136">InboxRules</span><span class="sxs-lookup"><span data-stu-id="8cb52-136">InboxRules</span></span>](inboxrules.md) <br/> |<span data-ttu-id="8cb52-137">Representa uma matriz de regras na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="8cb52-137">Represents an array of rules in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8cb52-138">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="8cb52-138">SetRuleOperation</span></span>](setruleoperation.md) <br/> |<span data-ttu-id="8cb52-139">Representa uma operação para atualizar uma regra existente.</span><span class="sxs-lookup"><span data-stu-id="8cb52-139">Represents an operation to update an existing rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8cb52-140">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8cb52-140">Text value</span></span>

<span data-ttu-id="8cb52-141">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8cb52-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8cb52-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="8cb52-142">Remarks</span></span>

<span data-ttu-id="8cb52-143">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8cb52-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8cb52-144">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8cb52-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8cb52-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="8cb52-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8cb52-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8cb52-146">Schema Name</span></span>  <br/> |<span data-ttu-id="8cb52-147">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8cb52-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="8cb52-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8cb52-148">Validation File</span></span>  <br/> |<span data-ttu-id="8cb52-149">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8cb52-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8cb52-150">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8cb52-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="8cb52-151">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="8cb52-151">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8cb52-152">Também consulte</span><span class="sxs-lookup"><span data-stu-id="8cb52-152">See also</span></span>



[<span data-ttu-id="8cb52-153">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="8cb52-153">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="8cb52-154">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="8cb52-154">SetRuleOperation</span></span>](setruleoperation.md)
  
[<span data-ttu-id="8cb52-155">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="8cb52-155">CreateRuleOperation</span></span>](createruleoperation.md)


- [<span data-ttu-id="8cb52-156">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8cb52-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

