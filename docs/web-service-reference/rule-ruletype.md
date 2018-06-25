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
description: O elemento de regra contém uma única regra e representa uma regra de caixa de correio do usuário.
ms.openlocfilehash: b1f9f058213543633335db11f03729964baf98ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825259"
---
# <a name="rule-ruletype"></a><span data-ttu-id="8fa18-103">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="8fa18-103">Rule (RuleType)</span></span>

<span data-ttu-id="8fa18-104">O elemento de **regra** contém uma única regra e representa uma regra de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="8fa18-104">The **Rule** element contains a single rule and represents a rule in a user's mailbox.</span></span> 
  
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

 <span data-ttu-id="8fa18-105">**RuleType**</span><span class="sxs-lookup"><span data-stu-id="8fa18-105">**RuleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8fa18-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8fa18-106">Attributes and elements</span></span>

<span data-ttu-id="8fa18-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8fa18-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8fa18-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8fa18-108">Attributes</span></span>

<span data-ttu-id="8fa18-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8fa18-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8fa18-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8fa18-110">Child elements</span></span>

|<span data-ttu-id="8fa18-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8fa18-111">**Element**</span></span>|<span data-ttu-id="8fa18-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8fa18-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8fa18-113">RuleId</span><span class="sxs-lookup"><span data-stu-id="8fa18-113">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="8fa18-114">Especifica o identificador da regra.</span><span class="sxs-lookup"><span data-stu-id="8fa18-114">Specifies the rule identifier.</span></span>  <br/> |
|[<span data-ttu-id="8fa18-115">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="8fa18-115">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="8fa18-116">Contém o nome de exibição de uma regra.</span><span class="sxs-lookup"><span data-stu-id="8fa18-116">Contains the display name of a rule.</span></span>  <br/> |
|[<span data-ttu-id="8fa18-117">Priority</span><span class="sxs-lookup"><span data-stu-id="8fa18-117">Priority</span></span>](priority.md) <br/> |<span data-ttu-id="8fa18-118">Indica a ordem na qual uma regra será executada.</span><span class="sxs-lookup"><span data-stu-id="8fa18-118">Indicates the order in which a rule is to be run.</span></span>  <br/> |
|[<span data-ttu-id="8fa18-119">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="8fa18-119">IsEnabled</span></span>](isenabled.md) <br/> |<span data-ttu-id="8fa18-120">Indica se a regra está habilitada.</span><span class="sxs-lookup"><span data-stu-id="8fa18-120">Indicates whether the rule is enabled.</span></span>  <br/> |
|[<span data-ttu-id="8fa18-121">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="8fa18-121">IsNotSupported</span></span>](isnotsupported.md) <br/> |<span data-ttu-id="8fa18-122">Indica se a regra não pode ser modificada com os APIs de código gerenciado.</span><span class="sxs-lookup"><span data-stu-id="8fa18-122">Indicates whether the rule cannot be modified with the managed code APIs.</span></span>  <br/> |
|[<span data-ttu-id="8fa18-123">IsInError</span><span class="sxs-lookup"><span data-stu-id="8fa18-123">IsInError</span></span>](isinerror.md) <br/> |<span data-ttu-id="8fa18-124">Indica se a regra está em uma condição de erro.</span><span class="sxs-lookup"><span data-stu-id="8fa18-124">Indicates whether the rule is in an error condition.</span></span>  <br/> |
|[<span data-ttu-id="8fa18-125">Condições</span><span class="sxs-lookup"><span data-stu-id="8fa18-125">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="8fa18-126">Identifica as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="8fa18-126">Identifies the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="8fa18-127">Exceções</span><span class="sxs-lookup"><span data-stu-id="8fa18-127">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="8fa18-128">Identifica as exceções que representam todas as condições de exceção de regra disponíveis para a regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="8fa18-128">Identifies the exceptions that represent all the available rule exception conditions for the inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="8fa18-129">Ações</span><span class="sxs-lookup"><span data-stu-id="8fa18-129">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="8fa18-130">Representa as ações a serem tomadas em uma mensagem quando as condições são atendidas.</span><span class="sxs-lookup"><span data-stu-id="8fa18-130">Represents the actions to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8fa18-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8fa18-131">Parent elements</span></span>

|<span data-ttu-id="8fa18-132">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8fa18-132">**Element**</span></span>|<span data-ttu-id="8fa18-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8fa18-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8fa18-134">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="8fa18-134">CreateRuleOperation</span></span>](createruleoperation.md) <br/> |<span data-ttu-id="8fa18-135">Representa uma operação para criar uma nova regra.</span><span class="sxs-lookup"><span data-stu-id="8fa18-135">Represents an operation to create a new rule.</span></span>  <br/> |
|[<span data-ttu-id="8fa18-136">InboxRules</span><span class="sxs-lookup"><span data-stu-id="8fa18-136">InboxRules</span></span>](inboxrules.md) <br/> |<span data-ttu-id="8fa18-137">Representa uma matriz de regras da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="8fa18-137">Represents an array of rules in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8fa18-138">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="8fa18-138">SetRuleOperation</span></span>](setruleoperation.md) <br/> |<span data-ttu-id="8fa18-139">Representa uma operação de atualização de uma regra existente.</span><span class="sxs-lookup"><span data-stu-id="8fa18-139">Represents an operation to update an existing rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8fa18-140">Text value</span><span class="sxs-lookup"><span data-stu-id="8fa18-140">Text value</span></span>

<span data-ttu-id="8fa18-141">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8fa18-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8fa18-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="8fa18-142">Remarks</span></span>

<span data-ttu-id="8fa18-143">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8fa18-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8fa18-144">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8fa18-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8fa18-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="8fa18-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8fa18-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8fa18-146">Schema Name</span></span>  <br/> |<span data-ttu-id="8fa18-147">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8fa18-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="8fa18-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8fa18-148">Validation File</span></span>  <br/> |<span data-ttu-id="8fa18-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8fa18-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8fa18-150">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8fa18-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="8fa18-151">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="8fa18-151">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8fa18-152">Ver também</span><span class="sxs-lookup"><span data-stu-id="8fa18-152">See also</span></span>



[<span data-ttu-id="8fa18-153">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="8fa18-153">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="8fa18-154">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="8fa18-154">SetRuleOperation</span></span>](setruleoperation.md)
  
[<span data-ttu-id="8fa18-155">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="8fa18-155">CreateRuleOperation</span></span>](createruleoperation.md)


- [<span data-ttu-id="8fa18-156">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8fa18-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

