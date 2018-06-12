---
title: NewMailEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NewMailEvent
api_type:
- schema
ms.assetid: 45057945-a3ec-4dac-92db-f0dc5fcfc34d
description: O elemento NewMailEvent representa um evento que é disparado por um novo item de email em uma caixa de correio.
ms.openlocfilehash: 8df3e4a218a8eaa9d129854e4816a3a43beddafa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824527"
---
# <a name="newmailevent"></a><span data-ttu-id="7ae27-103">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="7ae27-103">NewMailEvent</span></span>

<span data-ttu-id="7ae27-104">O elemento **NewMailEvent** representa um evento que é disparado por um novo item de email em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ae27-104">The **NewMailEvent** element represents an event that is triggered by a new mail item in a mailbox.</span></span> 
  
```xml
<NewMailEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</NewMailEvent>
```

 <span data-ttu-id="7ae27-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="7ae27-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ae27-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7ae27-106">Attributes and elements</span></span>

<span data-ttu-id="7ae27-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7ae27-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ae27-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7ae27-108">Attributes</span></span>

<span data-ttu-id="7ae27-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7ae27-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ae27-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7ae27-110">Child elements</span></span>

|<span data-ttu-id="7ae27-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7ae27-111">**Element**</span></span>|<span data-ttu-id="7ae27-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7ae27-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ae27-113">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="7ae27-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="7ae27-114">Representa um indicador de evento na tabela de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ae27-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="7ae27-115">Carimbo de hora</span><span class="sxs-lookup"><span data-stu-id="7ae27-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="7ae27-116">Representa o carimbo de hora de chegada de um novo item de email em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ae27-116">Represents the timestamp of the arrival of a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="7ae27-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="7ae27-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="7ae27-118">Representa o identificador de um novo item de email.</span><span class="sxs-lookup"><span data-stu-id="7ae27-118">Represents the identifier of a new mail item.</span></span>  <br/> |
|[<span data-ttu-id="7ae27-119">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="7ae27-119">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="7ae27-120">Representa o identificador da pasta pai de um novo item de email.</span><span class="sxs-lookup"><span data-stu-id="7ae27-120">Represents the identifier of the parent folder of the new mail item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7ae27-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7ae27-121">Parent elements</span></span>

|<span data-ttu-id="7ae27-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7ae27-122">**Element**</span></span>|<span data-ttu-id="7ae27-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7ae27-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ae27-124">Notificação</span><span class="sxs-lookup"><span data-stu-id="7ae27-124">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7ae27-125">Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="7ae27-125">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7ae27-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="7ae27-126">Remarks</span></span>

<span data-ttu-id="7ae27-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7ae27-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ae27-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7ae27-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ae27-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="7ae27-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7ae27-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7ae27-130">Schema name</span></span>  <br/> |<span data-ttu-id="7ae27-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7ae27-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="7ae27-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7ae27-132">Validation file</span></span>  <br/> |<span data-ttu-id="7ae27-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7ae27-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7ae27-134">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="7ae27-134">Can be empty</span></span>  <br/> |<span data-ttu-id="7ae27-135">False</span><span class="sxs-lookup"><span data-stu-id="7ae27-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ae27-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="7ae27-136">See also</span></span>



[<span data-ttu-id="7ae27-137">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="7ae27-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="7ae27-138">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="7ae27-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="7ae27-139">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="7ae27-139">Unsubscribe operation</span></span>](unsubscribe-operation.md)

