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
description: O elemento Timeout representa a duração, em minutos, que a assinatura pode permanecer ociosa sem uma solicitação de GetEvents do cliente.
ms.openlocfilehash: 6f3228cd480bf0eaf259c4f321bc74d0845b9bba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459893"
---
# <a name="timeout"></a><span data-ttu-id="a60cf-103">Timeout</span><span class="sxs-lookup"><span data-stu-id="a60cf-103">Timeout</span></span>

<span data-ttu-id="a60cf-104">O elemento **Timeout** representa a duração, em minutos, que a assinatura pode permanecer ociosa sem uma solicitação de GetEvents do cliente.</span><span class="sxs-lookup"><span data-stu-id="a60cf-104">The **Timeout** element represents the duration, in minutes, that the subscription can remain idle without a GetEvents request from the client.</span></span> 
  
```xml
<Timeout/>
```

 <span data-ttu-id="a60cf-105">**int**</span><span class="sxs-lookup"><span data-stu-id="a60cf-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a60cf-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a60cf-106">Attributes and elements</span></span>

<span data-ttu-id="a60cf-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a60cf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a60cf-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a60cf-108">Attributes</span></span>

<span data-ttu-id="a60cf-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a60cf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a60cf-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a60cf-110">Child elements</span></span>

<span data-ttu-id="a60cf-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a60cf-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a60cf-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a60cf-112">Parent elements</span></span>

|<span data-ttu-id="a60cf-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a60cf-113">**Element**</span></span>|<span data-ttu-id="a60cf-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a60cf-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a60cf-115">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="a60cf-115">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="a60cf-116">Representa uma assinatura para uma assinatura de notificação de eventos baseada em pull.</span><span class="sxs-lookup"><span data-stu-id="a60cf-116">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a60cf-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a60cf-117">Text value</span></span>

<span data-ttu-id="a60cf-118">Um valor de texto que representa um inteiro será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="a60cf-118">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="a60cf-119">Os valores possíveis para esse elemento são 1 a 1440, inclusive.</span><span class="sxs-lookup"><span data-stu-id="a60cf-119">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="a60cf-120">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a60cf-120">This element is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a60cf-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="a60cf-121">Remarks</span></span>

<span data-ttu-id="a60cf-122">O temporizador de tempo limite para a assinatura é redefinido por uma solicitação GetEvents bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="a60cf-122">The timeout timer for the subscription is reset by a successful GetEvents request.</span></span>
  
<span data-ttu-id="a60cf-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="a60cf-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="a60cf-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a60cf-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a60cf-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="a60cf-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a60cf-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a60cf-126">Schema name</span></span>  <br/> |<span data-ttu-id="a60cf-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a60cf-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="a60cf-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a60cf-128">Validation file</span></span>  <br/> |<span data-ttu-id="a60cf-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a60cf-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a60cf-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a60cf-130">Can be empty</span></span>  <br/> |<span data-ttu-id="a60cf-131">False</span><span class="sxs-lookup"><span data-stu-id="a60cf-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a60cf-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="a60cf-132">See also</span></span>



[<span data-ttu-id="a60cf-133">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="a60cf-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="a60cf-134">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="a60cf-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="a60cf-135">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="a60cf-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

