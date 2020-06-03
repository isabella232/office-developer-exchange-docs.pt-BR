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
description: O elemento Argument especifica argumentos para a ação.
ms.openlocfilehash: 41e3b1d891610669b0cc93f3daf6e8ee98c48396
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464753"
---
# <a name="argument"></a><span data-ttu-id="a2ef2-103">Argumento</span><span class="sxs-lookup"><span data-stu-id="a2ef2-103">Argument</span></span>

<span data-ttu-id="a2ef2-104">O elemento **Argument** especifica argumentos para a ação.</span><span class="sxs-lookup"><span data-stu-id="a2ef2-104">The **Argument** element specifies arguments to the action.</span></span> 
  
```xml
<Argument Value=""/>
```

 <span data-ttu-id="a2ef2-105">**ProtectionRuleArgumentType**</span><span class="sxs-lookup"><span data-stu-id="a2ef2-105">**ProtectionRuleArgumentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2ef2-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a2ef2-106">Attributes and elements</span></span>

<span data-ttu-id="a2ef2-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a2ef2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2ef2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a2ef2-108">Attributes</span></span>

|<span data-ttu-id="a2ef2-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="a2ef2-109">**Attribute**</span></span>|<span data-ttu-id="a2ef2-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a2ef2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a2ef2-111">**Valor**</span><span class="sxs-lookup"><span data-stu-id="a2ef2-111">**Value**</span></span> <br/> |<span data-ttu-id="a2ef2-112">Um valor de cadeia de caracteres não vazio que representa o valor de um argumento para a parte de ação de uma regra de proteção.</span><span class="sxs-lookup"><span data-stu-id="a2ef2-112">A non-empty string value that represents the value of an argument to the action part of a protection rule.</span></span> <span data-ttu-id="a2ef2-113">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="a2ef2-113">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a2ef2-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a2ef2-114">Child elements</span></span>

<span data-ttu-id="a2ef2-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a2ef2-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a2ef2-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a2ef2-116">Parent elements</span></span>

|<span data-ttu-id="a2ef2-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a2ef2-117">**Element**</span></span>|<span data-ttu-id="a2ef2-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a2ef2-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2ef2-119">Ação (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="a2ef2-119">Action (ProtectionRuleActionType)</span></span>](action-protectionruleactiontype.md) <br/> |<span data-ttu-id="a2ef2-120">Identifica qual ação deve ser executada se a condição da condição da regra corresponder.</span><span class="sxs-lookup"><span data-stu-id="a2ef2-120">Identifies what action must be executed if the condition part of the rule matches.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a2ef2-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a2ef2-121">Text value</span></span>

<span data-ttu-id="a2ef2-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a2ef2-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a2ef2-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="a2ef2-123">Remarks</span></span>

<span data-ttu-id="a2ef2-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a2ef2-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2ef2-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a2ef2-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2ef2-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="a2ef2-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a2ef2-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a2ef2-127">Schema Name</span></span>  <br/> |<span data-ttu-id="a2ef2-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a2ef2-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="a2ef2-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a2ef2-129">Validation File</span></span>  <br/> |<span data-ttu-id="a2ef2-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a2ef2-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a2ef2-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a2ef2-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2ef2-132">False</span><span class="sxs-lookup"><span data-stu-id="a2ef2-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2ef2-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="a2ef2-133">See also</span></span>

- [<span data-ttu-id="a2ef2-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a2ef2-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

