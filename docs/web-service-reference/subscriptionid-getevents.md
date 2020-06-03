---
title: SubscriptionId (GetEvents)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionId
api_type:
- schema
ms.assetid: 77c0abab-69e8-428e-8c20-22258e4ef71b
description: O elemento SubscriptionId representa o identificador de uma assinatura.
ms.openlocfilehash: e103386f466d65717878b4a6c811f3c3ad6e7c7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465349"
---
# <a name="subscriptionid-getevents"></a><span data-ttu-id="f8b88-103">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="f8b88-103">SubscriptionId (GetEvents)</span></span>

<span data-ttu-id="f8b88-104">O elemento **SubscriptionId** representa o identificador de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="f8b88-104">The **SubscriptionId** element represents the identifier for a subscription.</span></span> 
  
```xml
<SubscriptionId/>
```

 <span data-ttu-id="f8b88-105">**SubscriptionIdType**</span><span class="sxs-lookup"><span data-stu-id="f8b88-105">**SubscriptionIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f8b88-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f8b88-106">Attributes and elements</span></span>

<span data-ttu-id="f8b88-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f8b88-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8b88-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f8b88-108">Attributes</span></span>

<span data-ttu-id="f8b88-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f8b88-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f8b88-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f8b88-110">Child elements</span></span>

<span data-ttu-id="f8b88-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f8b88-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f8b88-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f8b88-112">Parent elements</span></span>

|<span data-ttu-id="f8b88-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f8b88-113">**Element**</span></span>|<span data-ttu-id="f8b88-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f8b88-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8b88-115">GetEvents</span><span class="sxs-lookup"><span data-stu-id="f8b88-115">GetEvents</span></span>](getevents.md) <br/> |<span data-ttu-id="f8b88-116">Representa a operação usada por clientes de recebimento para solicitar notificações do servidor.</span><span class="sxs-lookup"><span data-stu-id="f8b88-116">Represents the operation used by pull clients to request notifications from the server.</span></span>  <br/> |
|[<span data-ttu-id="f8b88-117">Notificação</span><span class="sxs-lookup"><span data-stu-id="f8b88-117">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f8b88-118">Contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="f8b88-118">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
|[<span data-ttu-id="f8b88-119">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f8b88-119">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md) <br/> |<span data-ttu-id="f8b88-120">Contém o status e o resultado de uma solicitação de assinatura.</span><span class="sxs-lookup"><span data-stu-id="f8b88-120">Contains the status and result of a Subscribe request.</span></span>  <br/> |
|[<span data-ttu-id="f8b88-121">Cancelar assinatura</span><span class="sxs-lookup"><span data-stu-id="f8b88-121">Unsubscribe</span></span>](unsubscribe.md) <br/> |<span data-ttu-id="f8b88-122">Contém as propriedades usadas para cancelar a inscrição de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="f8b88-122">Contains the properties used to unsubscribe from a subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f8b88-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f8b88-123">Text value</span></span>

<span data-ttu-id="f8b88-124">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8b88-124">A text value is required.</span></span> <span data-ttu-id="f8b88-125">O valor de texto é um GUID.</span><span class="sxs-lookup"><span data-stu-id="f8b88-125">The text value is a GUID.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f8b88-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="f8b88-126">Remarks</span></span>

<span data-ttu-id="f8b88-127">O GUID que representa o identificador de assinatura é gerado pelo servidor de acesso para cliente quando a assinatura é criada.</span><span class="sxs-lookup"><span data-stu-id="f8b88-127">The GUID that represents the subscription identifier is generated by the Client Access server when the subscription is created.</span></span>
  
<span data-ttu-id="f8b88-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="f8b88-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8b88-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f8b88-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8b88-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="f8b88-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f8b88-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f8b88-131">Schema name</span></span>  <br/> |<span data-ttu-id="f8b88-132">esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f8b88-132">messages schema</span></span>  <br/> |
|<span data-ttu-id="f8b88-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f8b88-133">Validation file</span></span>  <br/> |<span data-ttu-id="f8b88-134">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f8b88-134">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f8b88-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f8b88-135">Can be empty</span></span>  <br/> |<span data-ttu-id="f8b88-136">False</span><span class="sxs-lookup"><span data-stu-id="f8b88-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f8b88-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="f8b88-137">See also</span></span>



[<span data-ttu-id="f8b88-138">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="f8b88-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="f8b88-139">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="f8b88-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="f8b88-140">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="f8b88-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

