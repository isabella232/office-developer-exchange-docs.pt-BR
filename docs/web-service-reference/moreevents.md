---
title: MoreEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoreEvents
api_type:
- schema
ms.assetid: 76a7ea58-a44f-49b8-baba-d21302d742ad
description: O elemento MoreEvents indica se há mais eventos na fila a serem entregues ao cliente.
ms.openlocfilehash: fd12dd2e2e64ce1711e553ba5eb29bd0eb64c892
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462728"
---
# <a name="moreevents"></a><span data-ttu-id="7214d-103">MoreEvents</span><span class="sxs-lookup"><span data-stu-id="7214d-103">MoreEvents</span></span>

<span data-ttu-id="7214d-104">O elemento **MoreEvents** indica se há mais eventos na fila a serem entregues ao cliente.</span><span class="sxs-lookup"><span data-stu-id="7214d-104">The **MoreEvents** element indicates whether there are more events in the queue to be delivered to the client.</span></span> 
  
```xml
<MoreEvents/>
```

 <span data-ttu-id="7214d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="7214d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7214d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="7214d-106">Attributes and elements</span></span>

<span data-ttu-id="7214d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7214d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7214d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7214d-108">Attributes</span></span>

<span data-ttu-id="7214d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7214d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7214d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7214d-110">Child elements</span></span>

<span data-ttu-id="7214d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7214d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7214d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7214d-112">Parent elements</span></span>

|<span data-ttu-id="7214d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7214d-113">**Element**</span></span>|<span data-ttu-id="7214d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7214d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7214d-115">Notificação</span><span class="sxs-lookup"><span data-stu-id="7214d-115">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7214d-116">Contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="7214d-116">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7214d-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="7214d-117">Text value</span></span>

<span data-ttu-id="7214d-118">O valor de texto representa um valor booliano.</span><span class="sxs-lookup"><span data-stu-id="7214d-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="7214d-119">Um valor **true** indica que há mais eventos na fila.</span><span class="sxs-lookup"><span data-stu-id="7214d-119">A value of **true** indicates that more events are in the queue.</span></span> <span data-ttu-id="7214d-120">Um valor **false** indica que não há mais eventos na fila.</span><span class="sxs-lookup"><span data-stu-id="7214d-120">A value of **false** indicates that no more events are in the queue.</span></span> <span data-ttu-id="7214d-121">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7214d-121">This property is read-only.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7214d-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="7214d-122">Remarks</span></span>

<span data-ttu-id="7214d-123">No caso de notificações de recebimento, um valor **true** neste elemento indica ao cliente que outra solicitação GetEvents deve ser emitida para obter os eventos restantes.</span><span class="sxs-lookup"><span data-stu-id="7214d-123">In the case of Pull notifications, a **true** value in this element indicates to the client that another GetEvents request should be issued to get the remaining events.</span></span> <span data-ttu-id="7214d-124">Supondo que as especificações do cliente exijam latência mínima para notificações de evento, as solicitações GetEvents devem continuar em uma sucessão contínua até que um valor **false** **MoreEvents** seja retornado.</span><span class="sxs-lookup"><span data-stu-id="7214d-124">Assuming that the client specifications require minimum latency for event notifications, GetEvents requests should continue in a continuous succession until a **false** **MoreEvents** value is returned.</span></span> 
  
<span data-ttu-id="7214d-125">No caso de notificações por push, um valor **true** para **MoreEvents** indica ao cliente que outra solicitação de notificação será enviada ao cliente para entregar os eventos restantes.</span><span class="sxs-lookup"><span data-stu-id="7214d-125">In the case of Push notifications, a **true** value for **MoreEvents** indicates to the client that another notification request will be sent to the client to deliver the remaining events.</span></span> <span data-ttu-id="7214d-126">Semelhante às notificações pull, essas solicitações de acompanhamento continuarão em uma sucessão contínua até que a fila de eventos no servidor de acesso para cliente esteja vazia.</span><span class="sxs-lookup"><span data-stu-id="7214d-126">Similar to Pull notifications, these follow-up requests will continue in continuous succession until the event queue on the Client Access server is empty.</span></span> 
  
<span data-ttu-id="7214d-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7214d-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7214d-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="7214d-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7214d-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="7214d-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7214d-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7214d-130">Schema Name</span></span>  <br/> |<span data-ttu-id="7214d-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7214d-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="7214d-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7214d-132">Validation File</span></span>  <br/> |<span data-ttu-id="7214d-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7214d-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7214d-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7214d-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="7214d-135">False</span><span class="sxs-lookup"><span data-stu-id="7214d-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7214d-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="7214d-136">See also</span></span>



[<span data-ttu-id="7214d-137">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="7214d-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="7214d-138">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="7214d-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="7214d-139">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="7214d-139">Unsubscribe operation</span></span>](unsubscribe-operation.md)

