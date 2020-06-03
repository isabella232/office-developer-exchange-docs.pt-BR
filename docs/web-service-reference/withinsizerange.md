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
description: O elemento WithinSizeRange especifica os tamanhos mínimo e máximo que as mensagens de entrada devem ter para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 31da5815b70e20c47594da89b0b7ccab87eaf8f3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459739"
---
# <a name="withinsizerange"></a><span data-ttu-id="97470-103">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="97470-103">WithinSizeRange</span></span>

<span data-ttu-id="97470-104">O elemento **WithinSizeRange** especifica os tamanhos mínimo e máximo que as mensagens de entrada devem ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="97470-104">The **WithinSizeRange** element specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinSizeRange>
     <MinimumSize/>
     <MaximumSize/>
</WithinSizeRange>
```

 <span data-ttu-id="97470-105">**RulePredicateSizeRangeType**</span><span class="sxs-lookup"><span data-stu-id="97470-105">**RulePredicateSizeRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97470-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="97470-106">Attributes and elements</span></span>

<span data-ttu-id="97470-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="97470-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97470-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="97470-108">Attributes</span></span>

<span data-ttu-id="97470-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97470-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97470-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="97470-110">Child elements</span></span>

|<span data-ttu-id="97470-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="97470-111">**Element**</span></span>|<span data-ttu-id="97470-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97470-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97470-113">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="97470-113">MinimumSize</span></span>](minimumsize.md) <br/> |<span data-ttu-id="97470-114">Especifica o tamanho mínimo que uma mensagem deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="97470-114">Specifies the minimum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="97470-115">MaximumSize</span><span class="sxs-lookup"><span data-stu-id="97470-115">MaximumSize</span></span>](maximumsize.md) <br/> |<span data-ttu-id="97470-116">Especifica o tamanho máximo que uma mensagem deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="97470-116">Specifies the maximum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97470-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="97470-117">Parent elements</span></span>

|<span data-ttu-id="97470-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="97470-118">**Element**</span></span>|<span data-ttu-id="97470-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97470-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97470-120">Condições</span><span class="sxs-lookup"><span data-stu-id="97470-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="97470-121">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="97470-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="97470-122">Exceções</span><span class="sxs-lookup"><span data-stu-id="97470-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="97470-123">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="97470-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="97470-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="97470-124">Text value</span></span>

<span data-ttu-id="97470-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="97470-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="97470-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="97470-126">Remarks</span></span>

<span data-ttu-id="97470-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="97470-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97470-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="97470-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97470-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="97470-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="97470-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="97470-130">Schema Name</span></span>  <br/> |<span data-ttu-id="97470-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="97470-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="97470-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="97470-132">Validation File</span></span>  <br/> |<span data-ttu-id="97470-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="97470-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="97470-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="97470-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="97470-135">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="97470-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97470-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="97470-136">See also</span></span>



- [<span data-ttu-id="97470-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="97470-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

