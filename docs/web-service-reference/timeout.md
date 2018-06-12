---
title: Timeout
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Timeout
api_type:
- schema
ms.assetid: c2e1ca5a-6667-4f6f-aac4-89de33bddc54
description: O elemento de tempo limite representa a duração em minutos, que a assinatura pode permanecer inativa sem uma solicitação GetEvents do cliente.
ms.openlocfilehash: 0a26002689e131959f09318b01d97ffb73b605f9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837746"
---
# <a name="timeout"></a><span data-ttu-id="22ab6-103">Timeout</span><span class="sxs-lookup"><span data-stu-id="22ab6-103">Timeout</span></span>

<span data-ttu-id="22ab6-104">O elemento de **tempo limite** representa a duração em minutos, que a assinatura pode permanecer inativa sem uma solicitação GetEvents do cliente.</span><span class="sxs-lookup"><span data-stu-id="22ab6-104">The **Timeout** element represents the duration, in minutes, that the subscription can remain idle without a GetEvents request from the client.</span></span> 
  
```xml
<Timeout/>
```

 <span data-ttu-id="22ab6-105">**int**</span><span class="sxs-lookup"><span data-stu-id="22ab6-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22ab6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="22ab6-106">Attributes and elements</span></span>

<span data-ttu-id="22ab6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="22ab6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22ab6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="22ab6-108">Attributes</span></span>

<span data-ttu-id="22ab6-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="22ab6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22ab6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="22ab6-110">Child elements</span></span>

<span data-ttu-id="22ab6-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="22ab6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="22ab6-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="22ab6-112">Parent elements</span></span>

|<span data-ttu-id="22ab6-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="22ab6-113">**Element**</span></span>|<span data-ttu-id="22ab6-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="22ab6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22ab6-115">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="22ab6-115">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="22ab6-116">Representa uma assinatura para uma inscrição de notificação de evento baseado em extração.</span><span class="sxs-lookup"><span data-stu-id="22ab6-116">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="22ab6-117">Text value</span><span class="sxs-lookup"><span data-stu-id="22ab6-117">Text value</span></span>

<span data-ttu-id="22ab6-118">Se este elemento for usado, será necessário um valor de texto que representa um número inteiro.</span><span class="sxs-lookup"><span data-stu-id="22ab6-118">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="22ab6-119">Os valores possíveis para esse elemento são de 1 a 1440, inclusive.</span><span class="sxs-lookup"><span data-stu-id="22ab6-119">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="22ab6-120">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22ab6-120">This element is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="22ab6-121">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="22ab6-121">Remarks</span></span>

<span data-ttu-id="22ab6-122">O timer de tempo limite para a assinatura é redefinido por uma solicitação GetEvents bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="22ab6-122">The timeout timer for the subscription is reset by a successful GetEvents request.</span></span>
  
<span data-ttu-id="22ab6-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="22ab6-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="22ab6-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="22ab6-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22ab6-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="22ab6-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="22ab6-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="22ab6-126">Schema name</span></span>  <br/> |<span data-ttu-id="22ab6-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="22ab6-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="22ab6-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="22ab6-128">Validation file</span></span>  <br/> |<span data-ttu-id="22ab6-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="22ab6-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="22ab6-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="22ab6-130">Can be empty</span></span>  <br/> |<span data-ttu-id="22ab6-131">False</span><span class="sxs-lookup"><span data-stu-id="22ab6-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22ab6-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="22ab6-132">See also</span></span>



[<span data-ttu-id="22ab6-133">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="22ab6-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="22ab6-134">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="22ab6-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="22ab6-135">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="22ab6-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

