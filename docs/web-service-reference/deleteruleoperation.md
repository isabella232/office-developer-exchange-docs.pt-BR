---
title: DeleteRuleOperation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteRuleOperation
api_type:
- schema
ms.assetid: c5e251af-f795-43cc-baaf-95d84475677c
description: O elemento DeleteRuleOperation contém uma operação para excluir uma regra de caixa de entrada existente.
ms.openlocfilehash: 3410361e0b896fb0ef01c1873c9f8b0ac99afe58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751761"
---
# <a name="deleteruleoperation"></a><span data-ttu-id="7b113-103">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="7b113-103">DeleteRuleOperation</span></span>

<span data-ttu-id="7b113-104">O elemento **DeleteRuleOperation** contém uma operação para excluir uma regra de caixa de entrada existente.</span><span class="sxs-lookup"><span data-stu-id="7b113-104">The **DeleteRuleOperation** element contains an operation to delete an existing Inbox rule.</span></span> 
  
- [<span data-ttu-id="7b113-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="7b113-105">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="7b113-106">Operations</span><span class="sxs-lookup"><span data-stu-id="7b113-106">Operations</span></span>](operations.md)
  
```XML
<DeleteRuleOperation>
    <RuleId/>
</DeleteRuleOperation>
```

 <span data-ttu-id="7b113-107">**DeleteRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="7b113-107">**DeleteRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b113-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7b113-108">Attributes and elements</span></span>

<span data-ttu-id="7b113-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7b113-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b113-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="7b113-110">Attributes</span></span>

<span data-ttu-id="7b113-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7b113-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b113-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7b113-112">Child elements</span></span>

|<span data-ttu-id="7b113-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7b113-113">**Element**</span></span>|<span data-ttu-id="7b113-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7b113-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b113-115">RuleId</span><span class="sxs-lookup"><span data-stu-id="7b113-115">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="7b113-116">Especifica o identificador da regra a excluir.</span><span class="sxs-lookup"><span data-stu-id="7b113-116">Specifies the identifier of the rule to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7b113-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7b113-117">Parent elements</span></span>

|<span data-ttu-id="7b113-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7b113-118">**Element**</span></span>|<span data-ttu-id="7b113-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7b113-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b113-120">Operations</span><span class="sxs-lookup"><span data-stu-id="7b113-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="7b113-121">Contém uma matriz das operações de regra que podem ser executadas em uma caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="7b113-121">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7b113-122">Text value</span><span class="sxs-lookup"><span data-stu-id="7b113-122">Text value</span></span>

<span data-ttu-id="7b113-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7b113-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7b113-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="7b113-124">Remarks</span></span>

<span data-ttu-id="7b113-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7b113-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b113-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7b113-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b113-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="7b113-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7b113-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7b113-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7b113-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7b113-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="7b113-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7b113-130">Validation File</span></span>  <br/> |<span data-ttu-id="7b113-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7b113-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7b113-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7b113-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7b113-133">False</span><span class="sxs-lookup"><span data-stu-id="7b113-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7b113-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="7b113-134">See also</span></span>

- [<span data-ttu-id="7b113-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="7b113-135">UpdateInboxRules</span></span>](updateinboxrules.md) 
- [<span data-ttu-id="7b113-136">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="7b113-136">SetRuleOperation</span></span>](setruleoperation.md) 
- [<span data-ttu-id="7b113-137">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="7b113-137">CreateRuleOperation</span></span>](createruleoperation.md)
- [<span data-ttu-id="7b113-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7b113-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

