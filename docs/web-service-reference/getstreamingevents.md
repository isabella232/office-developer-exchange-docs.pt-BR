---
title: GetStreamingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEvents
api_type:
- schema
ms.assetid: dbe83857-c4f8-4d98-813f-e03c289697a1
description: O elemento GetStreamingEvents representa a operação que é usada pelos clientes para solicitar notificações de streaming do servidor.
ms.openlocfilehash: b07015541cf9c2fbbbc11ebc9f10421bdb9ee84f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823679"
---
# <a name="getstreamingevents"></a><span data-ttu-id="26fa8-103">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="26fa8-103">GetStreamingEvents</span></span>

<span data-ttu-id="26fa8-104">O elemento **GetStreamingEvents** representa a operação que é usada pelos clientes para solicitar notificações de streaming do servidor.</span><span class="sxs-lookup"><span data-stu-id="26fa8-104">The **GetStreamingEvents** element represents the operation that is used by clients to request streaming notifications from the server.</span></span> 
  
[<span data-ttu-id="26fa8-105">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="26fa8-105">GetStreamingEvents</span></span>](getstreamingevents.md)
  
```XML
<GetStreamingEvents>
   <SubscriptionId/>
   <ConnectionTimeout/>
</GetStreamingEvents>
```

 <span data-ttu-id="26fa8-106">**GetStreamingEventsType**</span><span class="sxs-lookup"><span data-stu-id="26fa8-106">**GetStreamingEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26fa8-107">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="26fa8-107">Attributes and elements</span></span>

<span data-ttu-id="26fa8-108">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="26fa8-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26fa8-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="26fa8-109">Attributes</span></span>

<span data-ttu-id="26fa8-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="26fa8-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26fa8-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="26fa8-111">Child elements</span></span>

|<span data-ttu-id="26fa8-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="26fa8-112">**Element**</span></span>|<span data-ttu-id="26fa8-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="26fa8-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26fa8-114">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="26fa8-114">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md) <br/> |<span data-ttu-id="26fa8-115">Representa o identificador de uma assinatura que é consultado para eventos.</span><span class="sxs-lookup"><span data-stu-id="26fa8-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="26fa8-116">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="26fa8-116">ConnectionTimeout</span></span>](connectiontimeout.md) <br/> |<span data-ttu-id="26fa8-117">Representa o número de minutos para manter uma conexão aberta.</span><span class="sxs-lookup"><span data-stu-id="26fa8-117">Represents the number of minutes to keep a connection open.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="26fa8-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="26fa8-118">Parent elements</span></span>

<span data-ttu-id="26fa8-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="26fa8-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="26fa8-120">Text value</span><span class="sxs-lookup"><span data-stu-id="26fa8-120">Text value</span></span>

<span data-ttu-id="26fa8-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="26fa8-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="26fa8-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="26fa8-122">Remarks</span></span>

<span data-ttu-id="26fa8-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="26fa8-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26fa8-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="26fa8-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26fa8-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="26fa8-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="26fa8-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="26fa8-126">Schema name</span></span>  <br/> |<span data-ttu-id="26fa8-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="26fa8-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="26fa8-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="26fa8-128">Validation file</span></span>  <br/> |<span data-ttu-id="26fa8-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="26fa8-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="26fa8-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="26fa8-130">Can be empty</span></span>  <br/> |<span data-ttu-id="26fa8-131">False</span><span class="sxs-lookup"><span data-stu-id="26fa8-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26fa8-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="26fa8-132">See also</span></span>



[<span data-ttu-id="26fa8-133">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="26fa8-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="26fa8-134">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="26fa8-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="26fa8-135">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="26fa8-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="26fa8-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="26fa8-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

