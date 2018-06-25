---
title: DeliveryStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliveryStatus
api_type:
- schema
ms.assetid: eab55db3-affb-42be-a586-5caa04052433
description: O elemento DeliveryStatus Especifica o status de uma mensagem.
ms.openlocfilehash: 4e6f31e8ef4f98d8e838ba91167c7dd5d6ab2590
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751774"
---
# <a name="deliverystatus"></a><span data-ttu-id="9652d-103">DeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="9652d-103">DeliveryStatus</span></span>

<span data-ttu-id="9652d-104">O elemento **DeliveryStatus** Especifica o status de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="9652d-104">The **DeliveryStatus** element specifies the status for a message.</span></span> 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 <span data-ttu-id="9652d-105">**MessageTrackingDeliveryStatusType**</span><span class="sxs-lookup"><span data-stu-id="9652d-105">**MessageTrackingDeliveryStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9652d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9652d-106">Attributes and elements</span></span>

<span data-ttu-id="9652d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9652d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9652d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9652d-108">Attributes</span></span>

<span data-ttu-id="9652d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9652d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9652d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9652d-110">Child elements</span></span>

<span data-ttu-id="9652d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9652d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9652d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9652d-112">Parent elements</span></span>

|<span data-ttu-id="9652d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9652d-113">**Element**</span></span>|<span data-ttu-id="9652d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9652d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9652d-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="9652d-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="9652d-116">Contém informações para um único evento de um destinatário.</span><span class="sxs-lookup"><span data-stu-id="9652d-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9652d-117">Text value</span><span class="sxs-lookup"><span data-stu-id="9652d-117">Text value</span></span>

<span data-ttu-id="9652d-118">A tabela a seguir lista os valores de texto possíveis para o elemento **DeliveryStatus** .</span><span class="sxs-lookup"><span data-stu-id="9652d-118">The following table lists the possible text values for the **DeliveryStatus** element.</span></span> 
  
<span data-ttu-id="9652d-119">**Valores de elemento DeliveryStatus**</span><span class="sxs-lookup"><span data-stu-id="9652d-119">**DeliveryStatus element values**</span></span>

|<span data-ttu-id="9652d-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="9652d-120">**Value**</span></span>|<span data-ttu-id="9652d-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9652d-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9652d-122">Sem êxito</span><span class="sxs-lookup"><span data-stu-id="9652d-122">Unsuccessful</span></span>  <br/> |<span data-ttu-id="9652d-123">Especifica que uma mensagem não foi entregue.</span><span class="sxs-lookup"><span data-stu-id="9652d-123">Specifies that a message was not delivered.</span></span>  <br/> |
|<span data-ttu-id="9652d-124">Pendente</span><span class="sxs-lookup"><span data-stu-id="9652d-124">Pending</span></span>  <br/> |<span data-ttu-id="9652d-125">Especifica que a mensagem está aguardando aprovação do moderador.</span><span class="sxs-lookup"><span data-stu-id="9652d-125">Specifies that the message is waiting for approval from a moderator.</span></span>  <br/> |
|<span data-ttu-id="9652d-126">Entregue</span><span class="sxs-lookup"><span data-stu-id="9652d-126">Delivered</span></span>  <br/> |<span data-ttu-id="9652d-127">Especifica que a mensagem foi entregue a todos os destinatários especificados.</span><span class="sxs-lookup"><span data-stu-id="9652d-127">Specifies that the message was delivered to all of the specified recipients.</span></span>  <br/> |
|<span data-ttu-id="9652d-128">Transferido</span><span class="sxs-lookup"><span data-stu-id="9652d-128">Transferred</span></span>  <br/> |<span data-ttu-id="9652d-129">Especifica que a mensagem foi transferida para um servidor fora do escopo de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="9652d-129">Specifies that the message was transferred to a server outside the search scope.</span></span>  <br/> |
|<span data-ttu-id="9652d-130">Ler</span><span class="sxs-lookup"><span data-stu-id="9652d-130">Read</span></span>  <br/> |<span data-ttu-id="9652d-131">Especifica que a mensagem foi entregue e leia pelos destinatários.</span><span class="sxs-lookup"><span data-stu-id="9652d-131">Specifies that the message was delivered and read by the recipients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9652d-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="9652d-132">Remarks</span></span>

<span data-ttu-id="9652d-133">O elemento **DeliveryStatus** era do tipo **MessageTrackingDeliveryStatusType** no Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="9652d-133">The **DeliveryStatus** element was of type **MessageTrackingDeliveryStatusType** in Exchange Server 2010.</span></span> 
  
<span data-ttu-id="9652d-134">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9652d-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9652d-135">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9652d-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9652d-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="9652d-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9652d-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9652d-137">Schema Name</span></span>  <br/> |<span data-ttu-id="9652d-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9652d-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="9652d-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9652d-139">Validation File</span></span>  <br/> |<span data-ttu-id="9652d-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9652d-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9652d-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9652d-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="9652d-142">False</span><span class="sxs-lookup"><span data-stu-id="9652d-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9652d-143">Ver também</span><span class="sxs-lookup"><span data-stu-id="9652d-143">See also</span></span>

- [<span data-ttu-id="9652d-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9652d-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

