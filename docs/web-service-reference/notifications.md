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
description: O elemento Notifications contém uma matriz de informações sobre a assinatura e os eventos que ocorreram desde a última notificação.
ms.openlocfilehash: 88fc56ba6e672e3dea7a1d31f7cc1fda018b9a15
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462616"
---
# <a name="notifications"></a><span data-ttu-id="694e3-103">Notificações</span><span class="sxs-lookup"><span data-stu-id="694e3-103">Notifications</span></span>

<span data-ttu-id="694e3-104">O elemento **Notifications** contém uma matriz de informações sobre a assinatura e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="694e3-104">The **Notifications** element contains an array of information about the subscription and the events that have occurred since the last notification.</span></span> 
  
```xml
<Notifications>
   <Notification/>
</Notifications>
```

 <span data-ttu-id="694e3-105">**NonEmptyArrayOfNotificationsType**</span><span class="sxs-lookup"><span data-stu-id="694e3-105">**NonEmptyArrayOfNotificationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="694e3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="694e3-106">Attributes and elements</span></span>

<span data-ttu-id="694e3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="694e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="694e3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="694e3-108">Attributes</span></span>

<span data-ttu-id="694e3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="694e3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="694e3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="694e3-110">Child elements</span></span>

|<span data-ttu-id="694e3-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="694e3-111">**Element**</span></span>|<span data-ttu-id="694e3-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="694e3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="694e3-113">Notificação</span><span class="sxs-lookup"><span data-stu-id="694e3-113">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="694e3-114">Contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="694e3-114">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="694e3-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="694e3-115">Parent elements</span></span>

|<span data-ttu-id="694e3-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="694e3-116">**Element**</span></span>|<span data-ttu-id="694e3-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="694e3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="694e3-118">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="694e3-118">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="694e3-119">Contém o status e o resultado de uma única solicitação de [operação GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="694e3-119">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="694e3-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="694e3-120">Text value</span></span>

<span data-ttu-id="694e3-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="694e3-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="694e3-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="694e3-122">Remarks</span></span>

<span data-ttu-id="694e3-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="694e3-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="694e3-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="694e3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="694e3-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="694e3-125">Namespace</span></span>  <br/> |<span data-ttu-id="694e3-126">https://schemas.microsoft.com/exchange/services/2006/messages e https://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="694e3-126">https://schemas.microsoft.com/exchange/services/2006/messages and https://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="694e3-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="694e3-127">Schema Name</span></span>  <br/> |<span data-ttu-id="694e3-128">Esquema de mensagens; Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="694e3-128">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="694e3-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="694e3-129">Validation File</span></span>  <br/> |<span data-ttu-id="694e3-130">Messages. xsd; Types. xsd</span><span class="sxs-lookup"><span data-stu-id="694e3-130">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="694e3-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="694e3-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="694e3-132">False</span><span class="sxs-lookup"><span data-stu-id="694e3-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="694e3-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="694e3-133">See also</span></span>



[<span data-ttu-id="694e3-134">Operação GetFolder</span><span class="sxs-lookup"><span data-stu-id="694e3-134">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="694e3-135">Operação DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="694e3-135">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="694e3-136">Operação MoveFolder</span><span class="sxs-lookup"><span data-stu-id="694e3-136">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="694e3-137">Operação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="694e3-137">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="694e3-138">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="694e3-138">Subscribe operation</span></span>](subscribe-operation.md)

