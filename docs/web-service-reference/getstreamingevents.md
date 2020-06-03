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
description: O elemento GetStreamingEvents representa a operação que é usada por clientes para solicitar notificações de streaming do servidor.
ms.openlocfilehash: ec133ecd69c05a2208e95f925133570af0233cf2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457316"
---
# <a name="getstreamingevents"></a><span data-ttu-id="ee2d9-103">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="ee2d9-103">GetStreamingEvents</span></span>

<span data-ttu-id="ee2d9-104">O elemento **GetStreamingEvents** representa a operação que é usada por clientes para solicitar notificações de streaming do servidor.</span><span class="sxs-lookup"><span data-stu-id="ee2d9-104">The **GetStreamingEvents** element represents the operation that is used by clients to request streaming notifications from the server.</span></span> 
  
[<span data-ttu-id="ee2d9-105">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="ee2d9-105">GetStreamingEvents</span></span>](getstreamingevents.md)
  
```XML
<GetStreamingEvents>
   <SubscriptionId/>
   <ConnectionTimeout/>
</GetStreamingEvents>
```

 <span data-ttu-id="ee2d9-106">**GetStreamingEventsType**</span><span class="sxs-lookup"><span data-stu-id="ee2d9-106">**GetStreamingEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee2d9-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ee2d9-107">Attributes and elements</span></span>

<span data-ttu-id="ee2d9-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ee2d9-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee2d9-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="ee2d9-109">Attributes</span></span>

<span data-ttu-id="ee2d9-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee2d9-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ee2d9-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ee2d9-111">Child elements</span></span>

|<span data-ttu-id="ee2d9-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ee2d9-112">**Element**</span></span>|<span data-ttu-id="ee2d9-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ee2d9-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee2d9-114">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="ee2d9-114">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md) <br/> |<span data-ttu-id="ee2d9-115">Representa o identificador de uma assinatura que é consultada para eventos.</span><span class="sxs-lookup"><span data-stu-id="ee2d9-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="ee2d9-116">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="ee2d9-116">ConnectionTimeout</span></span>](connectiontimeout.md) <br/> |<span data-ttu-id="ee2d9-117">Representa o número de minutos para manter uma conexão aberta.</span><span class="sxs-lookup"><span data-stu-id="ee2d9-117">Represents the number of minutes to keep a connection open.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ee2d9-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ee2d9-118">Parent elements</span></span>

<span data-ttu-id="ee2d9-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee2d9-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ee2d9-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ee2d9-120">Text value</span></span>

<span data-ttu-id="ee2d9-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ee2d9-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ee2d9-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="ee2d9-122">Remarks</span></span>

<span data-ttu-id="ee2d9-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ee2d9-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ee2d9-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ee2d9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee2d9-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="ee2d9-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ee2d9-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ee2d9-126">Schema name</span></span>  <br/> |<span data-ttu-id="ee2d9-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ee2d9-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ee2d9-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ee2d9-128">Validation file</span></span>  <br/> |<span data-ttu-id="ee2d9-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ee2d9-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ee2d9-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ee2d9-130">Can be empty</span></span>  <br/> |<span data-ttu-id="ee2d9-131">False</span><span class="sxs-lookup"><span data-stu-id="ee2d9-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ee2d9-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="ee2d9-132">See also</span></span>



[<span data-ttu-id="ee2d9-133">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="ee2d9-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="ee2d9-134">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="ee2d9-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="ee2d9-135">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="ee2d9-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="ee2d9-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ee2d9-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

