---
title: Argumento
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Argument
api_type:
- schema
ms.assetid: 15b0bfb8-2448-4ceb-aeac-965115e0fb72
description: O elemento de argumento especifica os argumentos para a ação.
ms.openlocfilehash: ed4e46a8d9897516e9c96bf3930f7d488bc06714
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751206"
---
# <a name="argument"></a><span data-ttu-id="709b7-103">Argumento</span><span class="sxs-lookup"><span data-stu-id="709b7-103">Argument</span></span>

<span data-ttu-id="709b7-104">O elemento de **argumento** Especifica os argumentos para a ação.</span><span class="sxs-lookup"><span data-stu-id="709b7-104">The **Argument** element specifies arguments to the action.</span></span> 
  
```xml
<Argument Value=""/>
```

 <span data-ttu-id="709b7-105">**ProtectionRuleArgumentType**</span><span class="sxs-lookup"><span data-stu-id="709b7-105">**ProtectionRuleArgumentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="709b7-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="709b7-106">Attributes and elements</span></span>

<span data-ttu-id="709b7-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="709b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="709b7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="709b7-108">Attributes</span></span>

|<span data-ttu-id="709b7-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="709b7-109">**Attribute**</span></span>|<span data-ttu-id="709b7-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="709b7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="709b7-111">**Valor**</span><span class="sxs-lookup"><span data-stu-id="709b7-111">**Value**</span></span> <br/> |<span data-ttu-id="709b7-112">Um valor de cadeia de caracteres não-vazias que representa o valor de um argumento para a parte de ação de uma regra de proteção.</span><span class="sxs-lookup"><span data-stu-id="709b7-112">A non-empty string value that represents the value of an argument to the action part of a protection rule.</span></span> <span data-ttu-id="709b7-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="709b7-113">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="709b7-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="709b7-114">Child elements</span></span>

<span data-ttu-id="709b7-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="709b7-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="709b7-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="709b7-116">Parent elements</span></span>

|<span data-ttu-id="709b7-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="709b7-117">**Element**</span></span>|<span data-ttu-id="709b7-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="709b7-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="709b7-119">Ação (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="709b7-119">Action (ProtectionRuleActionType)</span></span>](action-protectionruleactiontype.md) <br/> |<span data-ttu-id="709b7-120">Identifica a ação que deve ser executada se corresponder a parte de condição da regra.</span><span class="sxs-lookup"><span data-stu-id="709b7-120">Identifies what action must be executed if the condition part of the rule matches.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="709b7-121">Text value</span><span class="sxs-lookup"><span data-stu-id="709b7-121">Text value</span></span>

<span data-ttu-id="709b7-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="709b7-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="709b7-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="709b7-123">Remarks</span></span>

<span data-ttu-id="709b7-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="709b7-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="709b7-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="709b7-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="709b7-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="709b7-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="709b7-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="709b7-127">Schema Name</span></span>  <br/> |<span data-ttu-id="709b7-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="709b7-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="709b7-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="709b7-129">Validation File</span></span>  <br/> |<span data-ttu-id="709b7-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="709b7-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="709b7-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="709b7-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="709b7-132">False</span><span class="sxs-lookup"><span data-stu-id="709b7-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="709b7-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="709b7-133">See also</span></span>

- [<span data-ttu-id="709b7-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="709b7-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

