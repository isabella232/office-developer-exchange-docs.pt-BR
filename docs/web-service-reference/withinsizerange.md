---
title: WithinSizeRange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WithinSizeRange
api_type:
- schema
ms.assetid: 6f98650e-3399-4f87-9b7f-40bf20cdb821
description: O elemento WithinSizeRange Especifica os tamanhos mínimos e máximo que as mensagens recebidas devem estar na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 7711db9ca68f972f080c98197e30c7710620119a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838081"
---
# <a name="withinsizerange"></a><span data-ttu-id="e367d-103">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="e367d-103">WithinSizeRange</span></span>

<span data-ttu-id="e367d-104">O elemento **WithinSizeRange** Especifica os tamanhos mínimos e máximo que as mensagens recebidas devem estar na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="e367d-104">The **WithinSizeRange** element specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinSizeRange>
     <MinimumSize/>
     <MaximumSize/>
</WithinSizeRange>
```

 <span data-ttu-id="e367d-105">**RulePredicateSizeRangeType**</span><span class="sxs-lookup"><span data-stu-id="e367d-105">**RulePredicateSizeRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e367d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e367d-106">Attributes and elements</span></span>

<span data-ttu-id="e367d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e367d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e367d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e367d-108">Attributes</span></span>

<span data-ttu-id="e367d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e367d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e367d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e367d-110">Child elements</span></span>

|<span data-ttu-id="e367d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e367d-111">**Element**</span></span>|<span data-ttu-id="e367d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e367d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e367d-113">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="e367d-113">MinimumSize</span></span>](minimumsize.md) <br/> |<span data-ttu-id="e367d-114">Especifica o tamanho mínimo que uma mensagem deve ser em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="e367d-114">Specifies the minimum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="e367d-115">MaximumSize</span><span class="sxs-lookup"><span data-stu-id="e367d-115">MaximumSize</span></span>](maximumsize.md) <br/> |<span data-ttu-id="e367d-116">Especifica o tamanho máximo que uma mensagem deve ser em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="e367d-116">Specifies the maximum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e367d-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e367d-117">Parent elements</span></span>

|<span data-ttu-id="e367d-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e367d-118">**Element**</span></span>|<span data-ttu-id="e367d-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e367d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e367d-120">Condições</span><span class="sxs-lookup"><span data-stu-id="e367d-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="e367d-121">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="e367d-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="e367d-122">Exceções</span><span class="sxs-lookup"><span data-stu-id="e367d-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="e367d-123">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="e367d-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e367d-124">Text value</span><span class="sxs-lookup"><span data-stu-id="e367d-124">Text value</span></span>

<span data-ttu-id="e367d-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e367d-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e367d-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="e367d-126">Remarks</span></span>

<span data-ttu-id="e367d-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e367d-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e367d-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e367d-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e367d-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="e367d-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e367d-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e367d-130">Schema Name</span></span>  <br/> |<span data-ttu-id="e367d-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e367d-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e367d-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e367d-132">Validation File</span></span>  <br/> |<span data-ttu-id="e367d-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e367d-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e367d-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e367d-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="e367d-135">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="e367d-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e367d-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="e367d-136">See also</span></span>



- [<span data-ttu-id="e367d-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e367d-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

