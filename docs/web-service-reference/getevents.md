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
description: O elemento GetEvents representa a operação usada por clientes de recebimento para solicitar notificações do servidor.
ms.openlocfilehash: 004f782ccd32b3c5e501080bfc59419a6e7d9ce4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462497"
---
# <a name="getevents"></a><span data-ttu-id="3f326-103">GetEvents</span><span class="sxs-lookup"><span data-stu-id="3f326-103">GetEvents</span></span>

<span data-ttu-id="3f326-104">O elemento **GetEvents** representa a operação usada por clientes de recebimento para solicitar notificações do servidor.</span><span class="sxs-lookup"><span data-stu-id="3f326-104">The **GetEvents** element represents the operation used by pull clients to request notifications from the server.</span></span> 
  
[<span data-ttu-id="3f326-105">GetEvents</span><span class="sxs-lookup"><span data-stu-id="3f326-105">GetEvents</span></span>](getevents.md)
  
```xml
<GetEvents>
   <SubscriptionId/>
   <Watermark/>
</GetEvents>
```

 <span data-ttu-id="3f326-106">**Geteventtype**</span><span class="sxs-lookup"><span data-stu-id="3f326-106">**GetEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f326-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3f326-107">Attributes and elements</span></span>

<span data-ttu-id="3f326-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3f326-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f326-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="3f326-109">Attributes</span></span>

<span data-ttu-id="3f326-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f326-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3f326-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3f326-111">Child elements</span></span>

|<span data-ttu-id="3f326-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3f326-112">**Element**</span></span>|<span data-ttu-id="3f326-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3f326-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f326-114">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="3f326-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="3f326-115">Representa o identificador de uma assinatura que é consultada para eventos.</span><span class="sxs-lookup"><span data-stu-id="3f326-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="3f326-116">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="3f326-116">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="3f326-117">Representa a última marca d' água retornada ao cliente.</span><span class="sxs-lookup"><span data-stu-id="3f326-117">Represents the last watermark returned to the client.</span></span> <span data-ttu-id="3f326-118">Se GetEvents não tiver sido chamado para esta assinatura, o cliente usará a marca d' água retornada da solicitação de assinatura.</span><span class="sxs-lookup"><span data-stu-id="3f326-118">If GetEvents has not been called for this subscription, the client uses the watermark returned from the Subscribe request.</span></span> <span data-ttu-id="3f326-119">Caso contrário, a marca d' água do último evento na resposta GetEvents será usada.</span><span class="sxs-lookup"><span data-stu-id="3f326-119">Otherwise, the watermark from the last event in the last GetEvents response is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3f326-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3f326-120">Parent elements</span></span>

<span data-ttu-id="3f326-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f326-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3f326-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="3f326-122">Remarks</span></span>

<span data-ttu-id="3f326-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="3f326-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f326-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3f326-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f326-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="3f326-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3f326-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3f326-126">Schema name</span></span>  <br/> |<span data-ttu-id="3f326-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3f326-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3f326-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3f326-128">Validation file</span></span>  <br/> |<span data-ttu-id="3f326-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3f326-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3f326-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3f326-130">Can be empty</span></span>  <br/> |<span data-ttu-id="3f326-131">falso</span><span class="sxs-lookup"><span data-stu-id="3f326-131">false</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3f326-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="3f326-132">See also</span></span>



[<span data-ttu-id="3f326-133">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="3f326-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="3f326-134">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="3f326-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="3f326-135">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="3f326-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

