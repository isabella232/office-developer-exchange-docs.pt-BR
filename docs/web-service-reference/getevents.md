---
title: GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEvents
api_type:
- schema
ms.assetid: 22d4da6b-d8a8-484f-82c4-3e4b8f5431cd
description: O elemento GetEvents representa a operação usada pelos clientes de recepção para notificações de solicitação do servidor.
ms.openlocfilehash: e7b24207bff579a2f5230676d6520452f96fe0ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752472"
---
# <a name="getevents"></a><span data-ttu-id="d038f-103">GetEvents</span><span class="sxs-lookup"><span data-stu-id="d038f-103">GetEvents</span></span>

<span data-ttu-id="d038f-104">O elemento **GetEvents** representa a operação usada pelos clientes de recepção para notificações de solicitação do servidor.</span><span class="sxs-lookup"><span data-stu-id="d038f-104">The **GetEvents** element represents the operation used by pull clients to request notifications from the server.</span></span> 
  
[<span data-ttu-id="d038f-105">GetEvents</span><span class="sxs-lookup"><span data-stu-id="d038f-105">GetEvents</span></span>](getevents.md)
  
```xml
<GetEvents>
   <SubscriptionId/>
   <Watermark/>
</GetEvents>
```

 <span data-ttu-id="d038f-106">**GetEventsType**</span><span class="sxs-lookup"><span data-stu-id="d038f-106">**GetEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d038f-107">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d038f-107">Attributes and elements</span></span>

<span data-ttu-id="d038f-108">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d038f-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d038f-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="d038f-109">Attributes</span></span>

<span data-ttu-id="d038f-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d038f-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d038f-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d038f-111">Child elements</span></span>

|<span data-ttu-id="d038f-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d038f-112">**Element**</span></span>|<span data-ttu-id="d038f-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d038f-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d038f-114">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="d038f-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="d038f-115">Representa o identificador de uma assinatura que é consultado para eventos.</span><span class="sxs-lookup"><span data-stu-id="d038f-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="d038f-116">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="d038f-116">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="d038f-117">Representa a última marca d'água retornada ao cliente.</span><span class="sxs-lookup"><span data-stu-id="d038f-117">Represents the last watermark returned to the client.</span></span> <span data-ttu-id="d038f-118">Se não tiver sido chamado GetEvents para esta inscrição, o cliente usa a marca d'água retornada da solicitação Subscribe.</span><span class="sxs-lookup"><span data-stu-id="d038f-118">If GetEvents has not been called for this subscription, the client uses the watermark returned from the Subscribe request.</span></span> <span data-ttu-id="d038f-119">Caso contrário, a marca d'água a partir do último evento na última resposta GetEvents é usada.</span><span class="sxs-lookup"><span data-stu-id="d038f-119">Otherwise, the watermark from the last event in the last GetEvents response is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d038f-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d038f-120">Parent elements</span></span>

<span data-ttu-id="d038f-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d038f-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d038f-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="d038f-122">Remarks</span></span>

<span data-ttu-id="d038f-123">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d038f-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d038f-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d038f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d038f-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="d038f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d038f-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d038f-126">Schema name</span></span>  <br/> |<span data-ttu-id="d038f-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d038f-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d038f-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d038f-128">Validation file</span></span>  <br/> |<span data-ttu-id="d038f-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d038f-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d038f-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d038f-130">Can be empty</span></span>  <br/> |<span data-ttu-id="d038f-131">false</span><span class="sxs-lookup"><span data-stu-id="d038f-131">false</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d038f-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="d038f-132">See also</span></span>



[<span data-ttu-id="d038f-133">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="d038f-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d038f-134">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="d038f-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d038f-135">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="d038f-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

