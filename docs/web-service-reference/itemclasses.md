---
title: ItemClasses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemClasses
api_type:
- schema
ms.assetid: f95430cc-2860-47c1-af2d-8c4156c9b281
description: O elemento ItemClasses representa as classes de item que devem ser marcadas em mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 70a4823f9017ba8c6f894394d5907f1adeb80167
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824148"
---
# <a name="itemclasses"></a><span data-ttu-id="bdef6-103">ItemClasses</span><span class="sxs-lookup"><span data-stu-id="bdef6-103">ItemClasses</span></span>

<span data-ttu-id="bdef6-104">O elemento **ItemClasses** representa as classes de item que devem ser marcadas em mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="bdef6-104">The **ItemClasses** element represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ItemClasses>
    <String/>
</ItemClasses>
```

 <span data-ttu-id="bdef6-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="bdef6-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bdef6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="bdef6-106">Attributes and elements</span></span>

<span data-ttu-id="bdef6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bdef6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bdef6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="bdef6-108">Attributes</span></span>

<span data-ttu-id="bdef6-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bdef6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bdef6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bdef6-110">Child elements</span></span>

|<span data-ttu-id="bdef6-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bdef6-111">**Element**</span></span>|<span data-ttu-id="bdef6-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bdef6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bdef6-113">String</span><span class="sxs-lookup"><span data-stu-id="bdef6-113">String</span></span>](string.md) <br/> |<span data-ttu-id="bdef6-114">Representa uma classe de item único.</span><span class="sxs-lookup"><span data-stu-id="bdef6-114">Represents a single item class.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bdef6-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bdef6-115">Parent elements</span></span>

|<span data-ttu-id="bdef6-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bdef6-116">**Element**</span></span>|<span data-ttu-id="bdef6-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bdef6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bdef6-118">Condições</span><span class="sxs-lookup"><span data-stu-id="bdef6-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="bdef6-119">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="bdef6-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="bdef6-120">Exceções</span><span class="sxs-lookup"><span data-stu-id="bdef6-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="bdef6-121">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="bdef6-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bdef6-122">Text value</span><span class="sxs-lookup"><span data-stu-id="bdef6-122">Text value</span></span>

<span data-ttu-id="bdef6-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bdef6-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bdef6-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="bdef6-124">Remarks</span></span>

<span data-ttu-id="bdef6-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="bdef6-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bdef6-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="bdef6-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bdef6-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="bdef6-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bdef6-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bdef6-128">Schema name</span></span>  <br/> |<span data-ttu-id="bdef6-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="bdef6-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="bdef6-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bdef6-130">Validation file</span></span>  <br/> |<span data-ttu-id="bdef6-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bdef6-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bdef6-132">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="bdef6-132">Can be empty</span></span>  <br/> |<span data-ttu-id="bdef6-133">False</span><span class="sxs-lookup"><span data-stu-id="bdef6-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bdef6-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="bdef6-134">See also</span></span>



- [<span data-ttu-id="bdef6-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bdef6-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

