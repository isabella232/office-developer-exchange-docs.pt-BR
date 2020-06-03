---
title: Doclasss
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
description: O elemento doclasss representa as classes de item que devem ser carimbadas nas mensagens de entrada para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 56b99cad2abef0a9953e1793e5b633acca83a9eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460110"
---
# <a name="itemclasses"></a><span data-ttu-id="6458d-103">Doclasss</span><span class="sxs-lookup"><span data-stu-id="6458d-103">ItemClasses</span></span>

<span data-ttu-id="6458d-104">O elemento **Doclasss** representa as classes de item que devem ser carimbadas nas mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="6458d-104">The **ItemClasses** element represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ItemClasses>
    <String/>
</ItemClasses>
```

 <span data-ttu-id="6458d-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="6458d-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6458d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6458d-106">Attributes and elements</span></span>

<span data-ttu-id="6458d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6458d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6458d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6458d-108">Attributes</span></span>

<span data-ttu-id="6458d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6458d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6458d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6458d-110">Child elements</span></span>

|<span data-ttu-id="6458d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6458d-111">**Element**</span></span>|<span data-ttu-id="6458d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6458d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6458d-113">String</span><span class="sxs-lookup"><span data-stu-id="6458d-113">String</span></span>](string.md) <br/> |<span data-ttu-id="6458d-114">Representa uma única classe de item.</span><span class="sxs-lookup"><span data-stu-id="6458d-114">Represents a single item class.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6458d-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6458d-115">Parent elements</span></span>

|<span data-ttu-id="6458d-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6458d-116">**Element**</span></span>|<span data-ttu-id="6458d-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6458d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6458d-118">Condições</span><span class="sxs-lookup"><span data-stu-id="6458d-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="6458d-119">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="6458d-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="6458d-120">Exceções</span><span class="sxs-lookup"><span data-stu-id="6458d-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="6458d-121">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="6458d-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6458d-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="6458d-122">Text value</span></span>

<span data-ttu-id="6458d-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6458d-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6458d-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="6458d-124">Remarks</span></span>

<span data-ttu-id="6458d-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6458d-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6458d-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6458d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6458d-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="6458d-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6458d-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6458d-128">Schema name</span></span>  <br/> |<span data-ttu-id="6458d-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6458d-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="6458d-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6458d-130">Validation file</span></span>  <br/> |<span data-ttu-id="6458d-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6458d-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6458d-132">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="6458d-132">Can be empty</span></span>  <br/> |<span data-ttu-id="6458d-133">False</span><span class="sxs-lookup"><span data-stu-id="6458d-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6458d-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="6458d-134">See also</span></span>



- [<span data-ttu-id="6458d-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6458d-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

