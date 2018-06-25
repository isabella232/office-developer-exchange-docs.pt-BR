---
title: Ação (ProtectionRuleActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Action
api_type:
- schema
ms.assetid: ca090dec-e2c5-49c8-a057-8d1f2409147f
description: O elemento Action identifica a ação que deve ser executada se corresponder a parte de condição da regra.
ms.openlocfilehash: 8f699e698d3159c5ff2636da506542da3b218251
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752214"
---
# <a name="action-protectionruleactiontype"></a><span data-ttu-id="f6ce1-103">Ação (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="f6ce1-103">Action (ProtectionRuleActionType)</span></span>

<span data-ttu-id="f6ce1-104">O elemento **Action** identifica a ação que deve ser executada se corresponder a parte de condição da regra.</span><span class="sxs-lookup"><span data-stu-id="f6ce1-104">The **Action** element identifies what action must be executed if the condition part of the rule matches.</span></span> 
  
```xml
<Action Name="">
   <Argument/>
</Action>

```

 <span data-ttu-id="f6ce1-105">**ProtectionRuleActionType**</span><span class="sxs-lookup"><span data-stu-id="f6ce1-105">**ProtectionRuleActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6ce1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f6ce1-106">Attributes and elements</span></span>

<span data-ttu-id="f6ce1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f6ce1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6ce1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f6ce1-108">Attributes</span></span>

|<span data-ttu-id="f6ce1-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="f6ce1-109">**Attribute**</span></span>|<span data-ttu-id="f6ce1-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f6ce1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f6ce1-111">**Name**</span><span class="sxs-lookup"><span data-stu-id="f6ce1-111">**Name**</span></span> <br/> |<span data-ttu-id="f6ce1-112">Identifica o nome da ação.</span><span class="sxs-lookup"><span data-stu-id="f6ce1-112">Identifies the name of the action.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f6ce1-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f6ce1-113">Child elements</span></span>

|<span data-ttu-id="f6ce1-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f6ce1-114">**Element**</span></span>|<span data-ttu-id="f6ce1-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f6ce1-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6ce1-116">Argumento</span><span class="sxs-lookup"><span data-stu-id="f6ce1-116">Argument</span></span>](argument.md) <br/> |<span data-ttu-id="f6ce1-117">Especifica os argumentos para a ação.</span><span class="sxs-lookup"><span data-stu-id="f6ce1-117">Specifies arguments to the action.</span></span> <span data-ttu-id="f6ce1-118">Este elemento não ocorrerá se a ação especificada não requer argumentos deve ser especificado.</span><span class="sxs-lookup"><span data-stu-id="f6ce1-118">This element will not occur if the specified action does not require arguments to be specified.</span></span> <span data-ttu-id="f6ce1-119">Esse elemento pode ocorrer uma ou mais vezes, se uma ação exige um ou mais argumentos.</span><span class="sxs-lookup"><span data-stu-id="f6ce1-119">This element can occur one or more times if an action requires one or more arguments.</span></span> <span data-ttu-id="f6ce1-120">A ação **RightsProtectMessage** irá conter um único argumento.</span><span class="sxs-lookup"><span data-stu-id="f6ce1-120">The **RightsProtectMessage** action will contain a single argument.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f6ce1-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f6ce1-121">Parent elements</span></span>

|<span data-ttu-id="f6ce1-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f6ce1-122">**Element**</span></span>|<span data-ttu-id="f6ce1-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f6ce1-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6ce1-124">Rule</span><span class="sxs-lookup"><span data-stu-id="f6ce1-124">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="f6ce1-125">Contém uma regra de proteção do único.</span><span class="sxs-lookup"><span data-stu-id="f6ce1-125">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f6ce1-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="f6ce1-126">Remarks</span></span>

<span data-ttu-id="f6ce1-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6ce1-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6ce1-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f6ce1-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6ce1-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="f6ce1-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f6ce1-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f6ce1-130">Schema Name</span></span>  <br/> |<span data-ttu-id="f6ce1-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f6ce1-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="f6ce1-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f6ce1-132">Validation File</span></span>  <br/> |<span data-ttu-id="f6ce1-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f6ce1-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f6ce1-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f6ce1-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6ce1-135">False</span><span class="sxs-lookup"><span data-stu-id="f6ce1-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6ce1-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="f6ce1-136">See also</span></span>

- [<span data-ttu-id="f6ce1-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f6ce1-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

