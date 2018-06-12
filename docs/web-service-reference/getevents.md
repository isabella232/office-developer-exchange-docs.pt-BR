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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752472"
---
# <a name="getevents"></a><span data-ttu-id="880a2-103">GetEvents</span><span class="sxs-lookup"><span data-stu-id="880a2-103">GetEvents</span></span>

<span data-ttu-id="880a2-104">O elemento **GetEvents** representa a operação usada pelos clientes de recepção para notificações de solicitação do servidor.</span><span class="sxs-lookup"><span data-stu-id="880a2-104">The **GetEvents** element represents the operation used by pull clients to request notifications from the server.</span></span> 
  
[<span data-ttu-id="880a2-105">GetEvents</span><span class="sxs-lookup"><span data-stu-id="880a2-105">GetEvents</span></span>](getevents.md)
  
```xml
<GetEvents>
   <SubscriptionId/>
   <Watermark/>
</GetEvents>
```

 <span data-ttu-id="880a2-106">**GetEventsType**</span><span class="sxs-lookup"><span data-stu-id="880a2-106">**GetEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="880a2-107">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="880a2-107">Attributes and elements</span></span>

<span data-ttu-id="880a2-108">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="880a2-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="880a2-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="880a2-109">Attributes</span></span>

<span data-ttu-id="880a2-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="880a2-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="880a2-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="880a2-111">Child elements</span></span>

|<span data-ttu-id="880a2-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="880a2-112">**Element**</span></span>|<span data-ttu-id="880a2-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="880a2-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="880a2-114">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="880a2-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="880a2-115">Representa o identificador de uma assinatura que é consultado para eventos.</span><span class="sxs-lookup"><span data-stu-id="880a2-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="880a2-116">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="880a2-116">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="880a2-117">Representa a última marca d'água retornada ao cliente.</span><span class="sxs-lookup"><span data-stu-id="880a2-117">Represents the last watermark returned to the client.</span></span> <span data-ttu-id="880a2-118">Se não tiver sido chamado GetEvents para esta inscrição, o cliente usa a marca d'água retornada da solicitação Subscribe.</span><span class="sxs-lookup"><span data-stu-id="880a2-118">If GetEvents has not been called for this subscription, the client uses the watermark returned from the Subscribe request.</span></span> <span data-ttu-id="880a2-119">Caso contrário, a marca d'água a partir do último evento na última resposta GetEvents é usada.</span><span class="sxs-lookup"><span data-stu-id="880a2-119">Otherwise, the watermark from the last event in the last GetEvents response is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="880a2-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="880a2-120">Parent elements</span></span>

<span data-ttu-id="880a2-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="880a2-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="880a2-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="880a2-122">Remarks</span></span>

<span data-ttu-id="880a2-123">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="880a2-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="880a2-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="880a2-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="880a2-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="880a2-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="880a2-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="880a2-126">Schema name</span></span>  <br/> |<span data-ttu-id="880a2-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="880a2-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="880a2-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="880a2-128">Validation file</span></span>  <br/> |<span data-ttu-id="880a2-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="880a2-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="880a2-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="880a2-130">Can be empty</span></span>  <br/> |<span data-ttu-id="880a2-131">false</span><span class="sxs-lookup"><span data-stu-id="880a2-131">false</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="880a2-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="880a2-132">See also</span></span>



[<span data-ttu-id="880a2-133">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="880a2-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="880a2-134">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="880a2-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="880a2-135">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="880a2-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

