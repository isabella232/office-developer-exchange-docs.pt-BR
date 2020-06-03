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
description: O elemento WithinDateRange especifica o intervalo de datas no qual as mensagens de entrada precisam ser recebidas para que a condição ou exceção seja aplicada.
ms.openlocfilehash: ef5fb15b64ee4f7060f907818c4ebd4367ced5e7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461846"
---
# <a name="withindaterange"></a><span data-ttu-id="de7cb-103">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="de7cb-103">WithinDateRange</span></span>

<span data-ttu-id="de7cb-104">O elemento **WithinDateRange** especifica o intervalo de datas no qual as mensagens de entrada precisam ser recebidas para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="de7cb-104">The **WithinDateRange** element specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinDateRange>
     <StartDateTime/>
     <EndDateTime/>
</WithinDateRange>
```

 <span data-ttu-id="de7cb-105">**RulePredicateDateRangeType**</span><span class="sxs-lookup"><span data-stu-id="de7cb-105">**RulePredicateDateRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de7cb-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="de7cb-106">Attributes and elements</span></span>

<span data-ttu-id="de7cb-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="de7cb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de7cb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="de7cb-108">Attributes</span></span>

<span data-ttu-id="de7cb-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de7cb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de7cb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="de7cb-110">Child elements</span></span>

|<span data-ttu-id="de7cb-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="de7cb-111">**Element**</span></span>|<span data-ttu-id="de7cb-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="de7cb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de7cb-113">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="de7cb-113">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="de7cb-114">Especifica o período de tempo da regra e indica que a condição da regra é atendida após esse valor.</span><span class="sxs-lookup"><span data-stu-id="de7cb-114">Specifies the rule time period and indicates that the rule condition is met after this value.</span></span>  <br/> |
|[<span data-ttu-id="de7cb-115">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="de7cb-115">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="de7cb-116">Especifica o período de tempo da regra e indica que a condição da regra é atendida antes desse valor.</span><span class="sxs-lookup"><span data-stu-id="de7cb-116">Specifies the rule time period and indicates that the rule condition is met before this value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="de7cb-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="de7cb-117">Parent elements</span></span>

|<span data-ttu-id="de7cb-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="de7cb-118">**Element**</span></span>|<span data-ttu-id="de7cb-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="de7cb-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de7cb-120">Condições</span><span class="sxs-lookup"><span data-stu-id="de7cb-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="de7cb-121">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="de7cb-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="de7cb-122">Exceções</span><span class="sxs-lookup"><span data-stu-id="de7cb-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="de7cb-123">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="de7cb-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="de7cb-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="de7cb-124">Text value</span></span>

<span data-ttu-id="de7cb-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="de7cb-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="de7cb-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="de7cb-126">Remarks</span></span>

<span data-ttu-id="de7cb-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="de7cb-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de7cb-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="de7cb-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de7cb-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="de7cb-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="de7cb-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="de7cb-130">Schema Name</span></span>  <br/> |<span data-ttu-id="de7cb-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="de7cb-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="de7cb-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="de7cb-132">Validation File</span></span>  <br/> |<span data-ttu-id="de7cb-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="de7cb-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="de7cb-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="de7cb-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="de7cb-135">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="de7cb-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de7cb-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="de7cb-136">See also</span></span>



- [<span data-ttu-id="de7cb-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="de7cb-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

