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
ms.openlocfilehash: aa562b60a7299543af8653bbc767edf329075644
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466812"
---
# <a name="newmailevent"></a><span data-ttu-id="097b9-103">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="097b9-103">NewMailEvent</span></span>

<span data-ttu-id="097b9-104">O elemento **NewMailEvent** representa um evento que é disparado por um novo item de email em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="097b9-104">The **NewMailEvent** element represents an event that is triggered by a new mail item in a mailbox.</span></span> 
  
```xml
<NewMailEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</NewMailEvent>
```

 <span data-ttu-id="097b9-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="097b9-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="097b9-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="097b9-106">Attributes and elements</span></span>

<span data-ttu-id="097b9-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="097b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="097b9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="097b9-108">Attributes</span></span>

<span data-ttu-id="097b9-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="097b9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="097b9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="097b9-110">Child elements</span></span>

|<span data-ttu-id="097b9-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="097b9-111">**Element**</span></span>|<span data-ttu-id="097b9-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="097b9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="097b9-113">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="097b9-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="097b9-114">Representa um indicador de evento na tabela de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="097b9-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="097b9-115">Registra</span><span class="sxs-lookup"><span data-stu-id="097b9-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="097b9-116">Representa o carimbo de data/hora da chegada de um novo item de email em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="097b9-116">Represents the timestamp of the arrival of a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="097b9-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="097b9-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="097b9-118">Representa o identificador de um novo item de email.</span><span class="sxs-lookup"><span data-stu-id="097b9-118">Represents the identifier of a new mail item.</span></span>  <br/> |
|[<span data-ttu-id="097b9-119">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="097b9-119">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="097b9-120">Representa o identificador da pasta pai do novo item de email.</span><span class="sxs-lookup"><span data-stu-id="097b9-120">Represents the identifier of the parent folder of the new mail item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="097b9-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="097b9-121">Parent elements</span></span>

|<span data-ttu-id="097b9-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="097b9-122">**Element**</span></span>|<span data-ttu-id="097b9-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="097b9-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="097b9-124">Notificação</span><span class="sxs-lookup"><span data-stu-id="097b9-124">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="097b9-125">Contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="097b9-125">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="097b9-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="097b9-126">Remarks</span></span>

<span data-ttu-id="097b9-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="097b9-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="097b9-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="097b9-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="097b9-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="097b9-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="097b9-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="097b9-130">Schema name</span></span>  <br/> |<span data-ttu-id="097b9-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="097b9-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="097b9-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="097b9-132">Validation file</span></span>  <br/> |<span data-ttu-id="097b9-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="097b9-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="097b9-134">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="097b9-134">Can be empty</span></span>  <br/> |<span data-ttu-id="097b9-135">False</span><span class="sxs-lookup"><span data-stu-id="097b9-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="097b9-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="097b9-136">See also</span></span>



[<span data-ttu-id="097b9-137">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="097b9-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="097b9-138">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="097b9-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="097b9-139">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="097b9-139">Unsubscribe operation</span></span>](unsubscribe-operation.md)

