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
description: O elemento Action identifica qual ação deve ser executada se a condição da condição da regra corresponder.
ms.openlocfilehash: 220a6fea16abb9ea823ae6239537b8c121702589
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527506"
---
# <a name="action-protectionruleactiontype"></a><span data-ttu-id="dd7e5-103">Ação (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="dd7e5-103">Action (ProtectionRuleActionType)</span></span>

<span data-ttu-id="dd7e5-104">O elemento **Action** identifica qual ação deve ser executada se a condição da condição da regra corresponder.</span><span class="sxs-lookup"><span data-stu-id="dd7e5-104">The **Action** element identifies what action must be executed if the condition part of the rule matches.</span></span> 
  
```xml
<Action Name="">
   <Argument/>
</Action>

```

 <span data-ttu-id="dd7e5-105">**ProtectionRuleActionType**</span><span class="sxs-lookup"><span data-stu-id="dd7e5-105">**ProtectionRuleActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd7e5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="dd7e5-106">Attributes and elements</span></span>

<span data-ttu-id="dd7e5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dd7e5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd7e5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="dd7e5-108">Attributes</span></span>

|<span data-ttu-id="dd7e5-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="dd7e5-109">**Attribute**</span></span>|<span data-ttu-id="dd7e5-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dd7e5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dd7e5-111">**Nome**</span><span class="sxs-lookup"><span data-stu-id="dd7e5-111">**Name**</span></span> <br/> |<span data-ttu-id="dd7e5-112">Identifica o nome da ação.</span><span class="sxs-lookup"><span data-stu-id="dd7e5-112">Identifies the name of the action.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="dd7e5-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dd7e5-113">Child elements</span></span>

|<span data-ttu-id="dd7e5-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dd7e5-114">**Element**</span></span>|<span data-ttu-id="dd7e5-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dd7e5-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd7e5-116">Argumento</span><span class="sxs-lookup"><span data-stu-id="dd7e5-116">Argument</span></span>](argument.md) <br/> |<span data-ttu-id="dd7e5-117">Especifica argumentos para a ação.</span><span class="sxs-lookup"><span data-stu-id="dd7e5-117">Specifies arguments to the action.</span></span> <span data-ttu-id="dd7e5-118">Esse elemento não ocorrerá se a ação especificada não exigir que os argumentos sejam especificados.</span><span class="sxs-lookup"><span data-stu-id="dd7e5-118">This element will not occur if the specified action does not require arguments to be specified.</span></span> <span data-ttu-id="dd7e5-119">Esse elemento pode ocorrer uma ou mais vezes se uma ação requer um ou mais argumentos.</span><span class="sxs-lookup"><span data-stu-id="dd7e5-119">This element can occur one or more times if an action requires one or more arguments.</span></span> <span data-ttu-id="dd7e5-120">A ação **RightsProtectMessage** conterá um único argumento.</span><span class="sxs-lookup"><span data-stu-id="dd7e5-120">The **RightsProtectMessage** action will contain a single argument.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dd7e5-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dd7e5-121">Parent elements</span></span>

|<span data-ttu-id="dd7e5-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dd7e5-122">**Element**</span></span>|<span data-ttu-id="dd7e5-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dd7e5-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd7e5-124">Rule</span><span class="sxs-lookup"><span data-stu-id="dd7e5-124">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="dd7e5-125">Contém uma única regra de proteção.</span><span class="sxs-lookup"><span data-stu-id="dd7e5-125">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dd7e5-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="dd7e5-126">Remarks</span></span>

<span data-ttu-id="dd7e5-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="dd7e5-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd7e5-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="dd7e5-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd7e5-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="dd7e5-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dd7e5-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dd7e5-130">Schema Name</span></span>  <br/> |<span data-ttu-id="dd7e5-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="dd7e5-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="dd7e5-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dd7e5-132">Validation File</span></span>  <br/> |<span data-ttu-id="dd7e5-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="dd7e5-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dd7e5-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="dd7e5-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd7e5-135">False</span><span class="sxs-lookup"><span data-stu-id="dd7e5-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd7e5-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="dd7e5-136">See also</span></span>

- [<span data-ttu-id="dd7e5-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="dd7e5-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

