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
ms.openlocfilehash: 8867b7da7c75cfd9d41f708c0481627d5186cc14
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825622"
---
# <a name="subscriptionid-getevents"></a><span data-ttu-id="223ea-103">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="223ea-103">SubscriptionId (GetEvents)</span></span>

<span data-ttu-id="223ea-104">O elemento **SubscriptionId** representa o identificador de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="223ea-104">The **SubscriptionId** element represents the identifier for a subscription.</span></span> 
  
```xml
<SubscriptionId/>
```

 <span data-ttu-id="223ea-105">**SubscriptionIdType**</span><span class="sxs-lookup"><span data-stu-id="223ea-105">**SubscriptionIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="223ea-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="223ea-106">Attributes and elements</span></span>

<span data-ttu-id="223ea-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="223ea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="223ea-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="223ea-108">Attributes</span></span>

<span data-ttu-id="223ea-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="223ea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="223ea-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="223ea-110">Child elements</span></span>

<span data-ttu-id="223ea-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="223ea-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="223ea-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="223ea-112">Parent elements</span></span>

|<span data-ttu-id="223ea-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="223ea-113">**Element**</span></span>|<span data-ttu-id="223ea-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="223ea-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="223ea-115">GetEvents</span><span class="sxs-lookup"><span data-stu-id="223ea-115">GetEvents</span></span>](getevents.md) <br/> |<span data-ttu-id="223ea-116">Representa a operação usada pelos clientes de recepção para notificações de solicitação do servidor.</span><span class="sxs-lookup"><span data-stu-id="223ea-116">Represents the operation used by pull clients to request notifications from the server.</span></span>  <br/> |
|[<span data-ttu-id="223ea-117">Notificação</span><span class="sxs-lookup"><span data-stu-id="223ea-117">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="223ea-118">Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="223ea-118">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
|[<span data-ttu-id="223ea-119">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="223ea-119">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md) <br/> |<span data-ttu-id="223ea-120">Contém o status e o resultado de uma solicitação Subscribe.</span><span class="sxs-lookup"><span data-stu-id="223ea-120">Contains the status and result of a Subscribe request.</span></span>  <br/> |
|[<span data-ttu-id="223ea-121">Cancelar assinatura</span><span class="sxs-lookup"><span data-stu-id="223ea-121">Unsubscribe</span></span>](unsubscribe.md) <br/> |<span data-ttu-id="223ea-122">Contém as propriedades usadas para cancelar a assinatura de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="223ea-122">Contains the properties used to unsubscribe from a subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="223ea-123">Text value</span><span class="sxs-lookup"><span data-stu-id="223ea-123">Text value</span></span>

<span data-ttu-id="223ea-124">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="223ea-124">A text value is required.</span></span> <span data-ttu-id="223ea-125">O valor de texto é um GUID.</span><span class="sxs-lookup"><span data-stu-id="223ea-125">The text value is a GUID.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="223ea-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="223ea-126">Remarks</span></span>

<span data-ttu-id="223ea-127">O GUID que representa o identificador de inscrição é gerado pelo servidor de acesso para cliente quando a assinatura é criada.</span><span class="sxs-lookup"><span data-stu-id="223ea-127">The GUID that represents the subscription identifier is generated by the Client Access server when the subscription is created.</span></span>
  
<span data-ttu-id="223ea-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="223ea-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="223ea-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="223ea-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="223ea-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="223ea-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="223ea-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="223ea-131">Schema name</span></span>  <br/> |<span data-ttu-id="223ea-132">esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="223ea-132">messages schema</span></span>  <br/> |
|<span data-ttu-id="223ea-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="223ea-133">Validation file</span></span>  <br/> |<span data-ttu-id="223ea-134">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="223ea-134">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="223ea-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="223ea-135">Can be empty</span></span>  <br/> |<span data-ttu-id="223ea-136">False</span><span class="sxs-lookup"><span data-stu-id="223ea-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="223ea-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="223ea-137">See also</span></span>



[<span data-ttu-id="223ea-138">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="223ea-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="223ea-139">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="223ea-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="223ea-140">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="223ea-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

