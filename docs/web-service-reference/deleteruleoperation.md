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
ms.openlocfilehash: 6b17f7f99f1fd9b9889db00fdf55fba5eef5aba8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526918"
---
# <a name="deleteruleoperation"></a><span data-ttu-id="af996-103">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="af996-103">DeleteRuleOperation</span></span>

<span data-ttu-id="af996-104">O elemento **DeleteRuleOperation** contém uma operação para excluir uma regra de caixa de entrada existente.</span><span class="sxs-lookup"><span data-stu-id="af996-104">The **DeleteRuleOperation** element contains an operation to delete an existing Inbox rule.</span></span> 
  
- [<span data-ttu-id="af996-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="af996-105">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="af996-106">Operations</span><span class="sxs-lookup"><span data-stu-id="af996-106">Operations</span></span>](operations.md)
  
```XML
<DeleteRuleOperation>
    <RuleId/>
</DeleteRuleOperation>
```

 <span data-ttu-id="af996-107">**DeleteRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="af996-107">**DeleteRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af996-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="af996-108">Attributes and elements</span></span>

<span data-ttu-id="af996-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="af996-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af996-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="af996-110">Attributes</span></span>

<span data-ttu-id="af996-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af996-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af996-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="af996-112">Child elements</span></span>

|<span data-ttu-id="af996-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="af996-113">**Element**</span></span>|<span data-ttu-id="af996-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="af996-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af996-115">RuleId</span><span class="sxs-lookup"><span data-stu-id="af996-115">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="af996-116">Especifica o identificador da regra a ser excluída.</span><span class="sxs-lookup"><span data-stu-id="af996-116">Specifies the identifier of the rule to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="af996-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="af996-117">Parent elements</span></span>

|<span data-ttu-id="af996-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="af996-118">**Element**</span></span>|<span data-ttu-id="af996-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="af996-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af996-120">Operations</span><span class="sxs-lookup"><span data-stu-id="af996-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="af996-121">Contém uma matriz de operações de regra que podem ser executadas em uma caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="af996-121">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="af996-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="af996-122">Text value</span></span>

<span data-ttu-id="af996-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="af996-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="af996-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="af996-124">Remarks</span></span>

<span data-ttu-id="af996-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="af996-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af996-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="af996-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af996-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="af996-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="af996-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="af996-128">Schema Name</span></span>  <br/> |<span data-ttu-id="af996-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="af996-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="af996-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="af996-130">Validation File</span></span>  <br/> |<span data-ttu-id="af996-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="af996-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="af996-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="af996-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="af996-133">False</span><span class="sxs-lookup"><span data-stu-id="af996-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af996-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="af996-134">See also</span></span>

- [<span data-ttu-id="af996-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="af996-135">UpdateInboxRules</span></span>](updateinboxrules.md) 
- [<span data-ttu-id="af996-136">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="af996-136">SetRuleOperation</span></span>](setruleoperation.md) 
- [<span data-ttu-id="af996-137">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="af996-137">CreateRuleOperation</span></span>](createruleoperation.md)
- [<span data-ttu-id="af996-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="af996-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

