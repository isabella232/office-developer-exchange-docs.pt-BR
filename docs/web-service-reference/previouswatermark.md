---
title: PreviousWatermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PreviousWatermark
api_type:
- schema
ms.assetid: 474f4f7c-47da-47d4-8126-230012172fb5
description: O elemento PreviousWatermark representa a marca d'água do evento mais recente que foi comunicada com êxito para o cliente para a assinatura.
ms.openlocfilehash: 93c6f90d0866ae13618391b8544ab593fe33922b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824886"
---
# <a name="previouswatermark"></a><span data-ttu-id="558b3-103">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="558b3-103">PreviousWatermark</span></span>

<span data-ttu-id="558b3-104">O elemento **PreviousWatermark** representa a marca d'água do evento mais recente que foi comunicada com êxito para o cliente para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="558b3-104">The **PreviousWatermark** element represents the watermark of the latest event that was successfully communicated to the client for the subscription.</span></span> 
  
```xml
<PreviousWatermark/>
```

 <span data-ttu-id="558b3-105">**WatermarkType**</span><span class="sxs-lookup"><span data-stu-id="558b3-105">**WatermarkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="558b3-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="558b3-106">Attributes and elements</span></span>

<span data-ttu-id="558b3-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="558b3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="558b3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="558b3-108">Attributes</span></span>

<span data-ttu-id="558b3-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="558b3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="558b3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="558b3-110">Child elements</span></span>

<span data-ttu-id="558b3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="558b3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="558b3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="558b3-112">Parent elements</span></span>

|<span data-ttu-id="558b3-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="558b3-113">**Element**</span></span>|<span data-ttu-id="558b3-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="558b3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="558b3-115">Notificação</span><span class="sxs-lookup"><span data-stu-id="558b3-115">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="558b3-116">Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="558b3-116">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="558b3-117">Text value</span><span class="sxs-lookup"><span data-stu-id="558b3-117">Text value</span></span>

<span data-ttu-id="558b3-118">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="558b3-118">A text value is required.</span></span> <span data-ttu-id="558b3-119">O valor de texto representa a marca d'água mais recente.</span><span class="sxs-lookup"><span data-stu-id="558b3-119">The text value represents the latest watermark.</span></span> <span data-ttu-id="558b3-120">O valor de texto não pode ser uma sequência vazia.</span><span class="sxs-lookup"><span data-stu-id="558b3-120">The text value cannot be an empty string.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="558b3-121">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="558b3-121">Remarks</span></span>

<span data-ttu-id="558b3-122">A propriedade **PreviousWatermark** é útil para o cliente na determinação da última notificação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="558b3-122">The **PreviousWatermark** property is useful to the client in determining the last successful notification.</span></span> <span data-ttu-id="558b3-123">Por exemplo, se uma assinatura tem três eventos com marcas d'água 1, 2 e 3 e a próxima notificação é enviada com um valor **PreviousWatermark** 3, o cliente pode comparar este valor como o valor de marca d'água da última notificação recebida.</span><span class="sxs-lookup"><span data-stu-id="558b3-123">For example, if a subscription has three events with watermarks 1, 2, and 3, and the next notification is sent with a **PreviousWatermark** value of 3, the client can compare this value to the Watermark value of the last notification received.</span></span> <span data-ttu-id="558b3-124">Isso permite que o cliente garantir a continuidade de eventos.</span><span class="sxs-lookup"><span data-stu-id="558b3-124">This enables the client to ensure the continuity of events.</span></span> 
  
<span data-ttu-id="558b3-125">Para clientes de push, o **PreviousWatermark** é comparado com a local, no lado do cliente última conhecida marca d'água.</span><span class="sxs-lookup"><span data-stu-id="558b3-125">For push clients, the **PreviousWatermark** is compared to the local, client-side last known watermark.</span></span> <span data-ttu-id="558b3-126">Se os valores forem diferentes, o cliente perdeu uma notificação de evento e deverá restabelecer uma inscrição usando a marca d'água local mais recente.</span><span class="sxs-lookup"><span data-stu-id="558b3-126">If the values are different, the client has missed an event notification and should reestablish a subscription by using the latest local watermark.</span></span> <span data-ttu-id="558b3-127">Por exemplo, se um cliente de push recebe eventos de três para uma inscrição com marcas d'água 1, 2 e 3 e a próxima notificação vem com um valor **PreviousWatermark** 5, o cliente perdeu a notificação de pelo menos um e crie uma nova assinatura, passando um 3 como a marca d'água.</span><span class="sxs-lookup"><span data-stu-id="558b3-127">For example, if a push client receives three events for a subscription with watermarks 1, 2, and 3, and the next notification comes with a **PreviousWatermark** value of 5, the client has missed at least one notification and should create a new subscription, passing a 3 as the watermark.</span></span> 
  
<span data-ttu-id="558b3-128">No caso de um cliente de recepção, o valor de **PreviousWatermark** será o mesmo que a [marca d'água](watermark.md) incluídos pelo cliente na chamada GetEvents.</span><span class="sxs-lookup"><span data-stu-id="558b3-128">In the case of a pull client, the value of **PreviousWatermark** will be the same as the [Watermark](watermark.md) included by the client in the GetEvents call.</span></span> 
  
<span data-ttu-id="558b3-129">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="558b3-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="558b3-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="558b3-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="558b3-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="558b3-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="558b3-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="558b3-132">Schema Name</span></span>  <br/> |<span data-ttu-id="558b3-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="558b3-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="558b3-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="558b3-134">Validation File</span></span>  <br/> |<span data-ttu-id="558b3-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="558b3-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="558b3-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="558b3-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="558b3-137">False</span><span class="sxs-lookup"><span data-stu-id="558b3-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="558b3-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="558b3-138">See also</span></span>



[<span data-ttu-id="558b3-139">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="558b3-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="558b3-140">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="558b3-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="558b3-141">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="558b3-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)
