---
title: WithinDateRange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WithinDateRange
api_type:
- schema
ms.assetid: 226aeb15-016f-45ca-992a-c137ba09ca08
description: O elemento WithinDateRange Especifica o intervalo de datas dentro do qual as mensagens recebidas precisará foram recebidos em ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: d85ef91c581008c2aafb06b1900c4514aebacd65
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838073"
---
# <a name="withindaterange"></a><span data-ttu-id="c2302-103">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="c2302-103">WithinDateRange</span></span>

<span data-ttu-id="c2302-104">O elemento **WithinDateRange** Especifica o intervalo de datas dentro do qual as mensagens recebidas precisará foram recebidos em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="c2302-104">The **WithinDateRange** element specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinDateRange>
     <StartDateTime/>
     <EndDateTime/>
</WithinDateRange>
```

 <span data-ttu-id="c2302-105">**RulePredicateDateRangeType**</span><span class="sxs-lookup"><span data-stu-id="c2302-105">**RulePredicateDateRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2302-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c2302-106">Attributes and elements</span></span>

<span data-ttu-id="c2302-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c2302-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2302-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c2302-108">Attributes</span></span>

<span data-ttu-id="c2302-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c2302-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2302-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c2302-110">Child elements</span></span>

|<span data-ttu-id="c2302-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c2302-111">**Element**</span></span>|<span data-ttu-id="c2302-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c2302-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2302-113">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="c2302-113">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="c2302-114">Especifica a regra de período de tempo e indica que a condição de regra for atendida após esse valor.</span><span class="sxs-lookup"><span data-stu-id="c2302-114">Specifies the rule time period and indicates that the rule condition is met after this value.</span></span>  <br/> |
|[<span data-ttu-id="c2302-115">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="c2302-115">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="c2302-116">Especifica a regra de período de tempo e indica que a condição de regra é atendida antes que esse valor.</span><span class="sxs-lookup"><span data-stu-id="c2302-116">Specifies the rule time period and indicates that the rule condition is met before this value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c2302-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c2302-117">Parent elements</span></span>

|<span data-ttu-id="c2302-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c2302-118">**Element**</span></span>|<span data-ttu-id="c2302-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c2302-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2302-120">Condições</span><span class="sxs-lookup"><span data-stu-id="c2302-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="c2302-121">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="c2302-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="c2302-122">Exceções</span><span class="sxs-lookup"><span data-stu-id="c2302-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="c2302-123">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="c2302-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c2302-124">Text value</span><span class="sxs-lookup"><span data-stu-id="c2302-124">Text value</span></span>

<span data-ttu-id="c2302-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c2302-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c2302-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="c2302-126">Remarks</span></span>

<span data-ttu-id="c2302-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c2302-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2302-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c2302-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2302-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="c2302-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c2302-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c2302-130">Schema Name</span></span>  <br/> |<span data-ttu-id="c2302-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c2302-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c2302-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c2302-132">Validation File</span></span>  <br/> |<span data-ttu-id="c2302-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c2302-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c2302-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c2302-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2302-135">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="c2302-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2302-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="c2302-136">See also</span></span>



- [<span data-ttu-id="c2302-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c2302-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

