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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838081"
---
# <a name="withinsizerange"></a><span data-ttu-id="fc65b-103">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="fc65b-103">WithinSizeRange</span></span>

<span data-ttu-id="fc65b-104">O elemento **WithinSizeRange** Especifica os tamanhos mínimos e máximo que as mensagens recebidas devem estar na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="fc65b-104">The **WithinSizeRange** element specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinSizeRange>
     <MinimumSize/>
     <MaximumSize/>
</WithinSizeRange>
```

 <span data-ttu-id="fc65b-105">**RulePredicateSizeRangeType**</span><span class="sxs-lookup"><span data-stu-id="fc65b-105">**RulePredicateSizeRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc65b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="fc65b-106">Attributes and elements</span></span>

<span data-ttu-id="fc65b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fc65b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc65b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fc65b-108">Attributes</span></span>

<span data-ttu-id="fc65b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fc65b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc65b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fc65b-110">Child elements</span></span>

|<span data-ttu-id="fc65b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fc65b-111">**Element**</span></span>|<span data-ttu-id="fc65b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc65b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc65b-113">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="fc65b-113">MinimumSize</span></span>](minimumsize.md) <br/> |<span data-ttu-id="fc65b-114">Especifica o tamanho mínimo que uma mensagem deve ser em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="fc65b-114">Specifies the minimum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="fc65b-115">MaximumSize</span><span class="sxs-lookup"><span data-stu-id="fc65b-115">MaximumSize</span></span>](maximumsize.md) <br/> |<span data-ttu-id="fc65b-116">Especifica o tamanho máximo que uma mensagem deve ser em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="fc65b-116">Specifies the maximum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fc65b-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fc65b-117">Parent elements</span></span>

|<span data-ttu-id="fc65b-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fc65b-118">**Element**</span></span>|<span data-ttu-id="fc65b-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc65b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc65b-120">Condições</span><span class="sxs-lookup"><span data-stu-id="fc65b-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="fc65b-121">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="fc65b-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="fc65b-122">Exceções</span><span class="sxs-lookup"><span data-stu-id="fc65b-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="fc65b-123">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="fc65b-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fc65b-124">Text value</span><span class="sxs-lookup"><span data-stu-id="fc65b-124">Text value</span></span>

<span data-ttu-id="fc65b-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fc65b-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fc65b-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="fc65b-126">Remarks</span></span>

<span data-ttu-id="fc65b-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc65b-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc65b-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="fc65b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc65b-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="fc65b-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fc65b-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fc65b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="fc65b-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="fc65b-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fc65b-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fc65b-132">Validation File</span></span>  <br/> |<span data-ttu-id="fc65b-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fc65b-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fc65b-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fc65b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc65b-135">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="fc65b-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc65b-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="fc65b-136">See also</span></span>



- [<span data-ttu-id="fc65b-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fc65b-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

