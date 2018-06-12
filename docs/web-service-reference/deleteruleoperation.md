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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751761"
---
# <a name="deleteruleoperation"></a><span data-ttu-id="9d413-103">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="9d413-103">DeleteRuleOperation</span></span>

<span data-ttu-id="9d413-104">O elemento **DeleteRuleOperation** contém uma operação para excluir uma regra de caixa de entrada existente.</span><span class="sxs-lookup"><span data-stu-id="9d413-104">The **DeleteRuleOperation** element contains an operation to delete an existing Inbox rule.</span></span> 
  
- [<span data-ttu-id="9d413-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="9d413-105">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="9d413-106">Operations</span><span class="sxs-lookup"><span data-stu-id="9d413-106">Operations</span></span>](operations.md)
  
```XML
<DeleteRuleOperation>
    <RuleId/>
</DeleteRuleOperation>
```

 <span data-ttu-id="9d413-107">**DeleteRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="9d413-107">**DeleteRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d413-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9d413-108">Attributes and elements</span></span>

<span data-ttu-id="9d413-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9d413-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d413-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="9d413-110">Attributes</span></span>

<span data-ttu-id="9d413-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9d413-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d413-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9d413-112">Child elements</span></span>

|<span data-ttu-id="9d413-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9d413-113">**Element**</span></span>|<span data-ttu-id="9d413-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d413-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d413-115">RuleId</span><span class="sxs-lookup"><span data-stu-id="9d413-115">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="9d413-116">Especifica o identificador da regra a excluir.</span><span class="sxs-lookup"><span data-stu-id="9d413-116">Specifies the identifier of the rule to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d413-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9d413-117">Parent elements</span></span>

|<span data-ttu-id="9d413-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9d413-118">**Element**</span></span>|<span data-ttu-id="9d413-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d413-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d413-120">Operations</span><span class="sxs-lookup"><span data-stu-id="9d413-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="9d413-121">Contém uma matriz das operações de regra que podem ser executadas em uma caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="9d413-121">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9d413-122">Text value</span><span class="sxs-lookup"><span data-stu-id="9d413-122">Text value</span></span>

<span data-ttu-id="9d413-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9d413-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9d413-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="9d413-124">Remarks</span></span>

<span data-ttu-id="9d413-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d413-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d413-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9d413-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d413-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="9d413-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9d413-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9d413-128">Schema Name</span></span>  <br/> |<span data-ttu-id="9d413-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9d413-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="9d413-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9d413-130">Validation File</span></span>  <br/> |<span data-ttu-id="9d413-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9d413-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9d413-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9d413-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d413-133">False</span><span class="sxs-lookup"><span data-stu-id="9d413-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d413-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="9d413-134">See also</span></span>

- [<span data-ttu-id="9d413-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="9d413-135">UpdateInboxRules</span></span>](updateinboxrules.md) 
- [<span data-ttu-id="9d413-136">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="9d413-136">SetRuleOperation</span></span>](setruleoperation.md) 
- [<span data-ttu-id="9d413-137">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="9d413-137">CreateRuleOperation</span></span>](createruleoperation.md)
- [<span data-ttu-id="9d413-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9d413-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

