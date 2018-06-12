---
title: Notificações
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Notifications
api_type:
- schema
ms.assetid: 153cc420-d2fe-42f1-afb2-9a31ee09a750
description: O elemento de notificações contém uma matriz de informações sobre a assinatura e os eventos que ocorreram desde a última notificação.
ms.openlocfilehash: f576bf579c91b77dcde8646a6af7fdc47145aef7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824550"
---
# <a name="notifications"></a><span data-ttu-id="ae31d-103">Notificações</span><span class="sxs-lookup"><span data-stu-id="ae31d-103">Notifications</span></span>

<span data-ttu-id="ae31d-104">O elemento de **notificações** contém uma matriz de informações sobre a assinatura e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="ae31d-104">The **Notifications** element contains an array of information about the subscription and the events that have occurred since the last notification.</span></span> 
  
```xml
<Notifications>
   <Notification/>
</Notifications>
```

 <span data-ttu-id="ae31d-105">**NonEmptyArrayOfNotificationsType**</span><span class="sxs-lookup"><span data-stu-id="ae31d-105">**NonEmptyArrayOfNotificationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae31d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ae31d-106">Attributes and elements</span></span>

<span data-ttu-id="ae31d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ae31d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae31d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ae31d-108">Attributes</span></span>

<span data-ttu-id="ae31d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ae31d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae31d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ae31d-110">Child elements</span></span>

|<span data-ttu-id="ae31d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ae31d-111">**Element**</span></span>|<span data-ttu-id="ae31d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ae31d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae31d-113">Notificação</span><span class="sxs-lookup"><span data-stu-id="ae31d-113">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ae31d-114">Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="ae31d-114">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ae31d-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ae31d-115">Parent elements</span></span>

|<span data-ttu-id="ae31d-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ae31d-116">**Element**</span></span>|<span data-ttu-id="ae31d-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ae31d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae31d-118">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ae31d-118">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="ae31d-119">Contém o status e o resultado de uma única solicitação de [operação GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ae31d-119">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ae31d-120">Text value</span><span class="sxs-lookup"><span data-stu-id="ae31d-120">Text value</span></span>

<span data-ttu-id="ae31d-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ae31d-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ae31d-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="ae31d-122">Remarks</span></span>

<span data-ttu-id="ae31d-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ae31d-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae31d-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ae31d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae31d-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="ae31d-125">Namespace</span></span>  <br/> |<span data-ttu-id="ae31d-126">http://schemas.microsoft.com/exchange/services/2006/messages e http://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="ae31d-126">http://schemas.microsoft.com/exchange/services/2006/messages and http://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="ae31d-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ae31d-127">Schema Name</span></span>  <br/> |<span data-ttu-id="ae31d-128">Esquema de mensagens; Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ae31d-128">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="ae31d-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ae31d-129">Validation File</span></span>  <br/> |<span data-ttu-id="ae31d-130">Messages.xsd; Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ae31d-130">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ae31d-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ae31d-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="ae31d-132">False</span><span class="sxs-lookup"><span data-stu-id="ae31d-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae31d-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="ae31d-133">See also</span></span>



[<span data-ttu-id="ae31d-134">Operação GetFolder</span><span class="sxs-lookup"><span data-stu-id="ae31d-134">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="ae31d-135">Operação DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="ae31d-135">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="ae31d-136">Operação MoveFolder</span><span class="sxs-lookup"><span data-stu-id="ae31d-136">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="ae31d-137">Operação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="ae31d-137">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="ae31d-138">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="ae31d-138">Subscribe operation</span></span>](subscribe-operation.md)

