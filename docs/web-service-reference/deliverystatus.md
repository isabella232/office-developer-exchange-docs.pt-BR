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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751774"
---
# <a name="deliverystatus"></a><span data-ttu-id="a7db1-103">DeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="a7db1-103">DeliveryStatus</span></span>

<span data-ttu-id="a7db1-104">O elemento **DeliveryStatus** Especifica o status de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="a7db1-104">The **DeliveryStatus** element specifies the status for a message.</span></span> 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 <span data-ttu-id="a7db1-105">**MessageTrackingDeliveryStatusType**</span><span class="sxs-lookup"><span data-stu-id="a7db1-105">**MessageTrackingDeliveryStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7db1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a7db1-106">Attributes and elements</span></span>

<span data-ttu-id="a7db1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a7db1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7db1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a7db1-108">Attributes</span></span>

<span data-ttu-id="a7db1-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a7db1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a7db1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a7db1-110">Child elements</span></span>

<span data-ttu-id="a7db1-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a7db1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a7db1-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a7db1-112">Parent elements</span></span>

|<span data-ttu-id="a7db1-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a7db1-113">**Element**</span></span>|<span data-ttu-id="a7db1-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a7db1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7db1-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="a7db1-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="a7db1-116">Contém informações para um único evento de um destinatário.</span><span class="sxs-lookup"><span data-stu-id="a7db1-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a7db1-117">Text value</span><span class="sxs-lookup"><span data-stu-id="a7db1-117">Text value</span></span>

<span data-ttu-id="a7db1-118">A tabela a seguir lista os valores de texto possíveis para o elemento **DeliveryStatus** .</span><span class="sxs-lookup"><span data-stu-id="a7db1-118">The following table lists the possible text values for the **DeliveryStatus** element.</span></span> 
  
<span data-ttu-id="a7db1-119">**Valores de elemento DeliveryStatus**</span><span class="sxs-lookup"><span data-stu-id="a7db1-119">**DeliveryStatus element values**</span></span>

|<span data-ttu-id="a7db1-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="a7db1-120">**Value**</span></span>|<span data-ttu-id="a7db1-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a7db1-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a7db1-122">Sem êxito</span><span class="sxs-lookup"><span data-stu-id="a7db1-122">Unsuccessful</span></span>  <br/> |<span data-ttu-id="a7db1-123">Especifica que uma mensagem não foi entregue.</span><span class="sxs-lookup"><span data-stu-id="a7db1-123">Specifies that a message was not delivered.</span></span>  <br/> |
|<span data-ttu-id="a7db1-124">Pendente</span><span class="sxs-lookup"><span data-stu-id="a7db1-124">Pending</span></span>  <br/> |<span data-ttu-id="a7db1-125">Especifica que a mensagem está aguardando aprovação do moderador.</span><span class="sxs-lookup"><span data-stu-id="a7db1-125">Specifies that the message is waiting for approval from a moderator.</span></span>  <br/> |
|<span data-ttu-id="a7db1-126">Entregue</span><span class="sxs-lookup"><span data-stu-id="a7db1-126">Delivered</span></span>  <br/> |<span data-ttu-id="a7db1-127">Especifica que a mensagem foi entregue a todos os destinatários especificados.</span><span class="sxs-lookup"><span data-stu-id="a7db1-127">Specifies that the message was delivered to all of the specified recipients.</span></span>  <br/> |
|<span data-ttu-id="a7db1-128">Transferido</span><span class="sxs-lookup"><span data-stu-id="a7db1-128">Transferred</span></span>  <br/> |<span data-ttu-id="a7db1-129">Especifica que a mensagem foi transferida para um servidor fora do escopo de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a7db1-129">Specifies that the message was transferred to a server outside the search scope.</span></span>  <br/> |
|<span data-ttu-id="a7db1-130">Ler</span><span class="sxs-lookup"><span data-stu-id="a7db1-130">Read</span></span>  <br/> |<span data-ttu-id="a7db1-131">Especifica que a mensagem foi entregue e leia pelos destinatários.</span><span class="sxs-lookup"><span data-stu-id="a7db1-131">Specifies that the message was delivered and read by the recipients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a7db1-132">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="a7db1-132">Remarks</span></span>

<span data-ttu-id="a7db1-133">O elemento **DeliveryStatus** era do tipo **MessageTrackingDeliveryStatusType** no Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="a7db1-133">The **DeliveryStatus** element was of type **MessageTrackingDeliveryStatusType** in Exchange Server 2010.</span></span> 
  
<span data-ttu-id="a7db1-134">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7db1-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7db1-135">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a7db1-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7db1-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="a7db1-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a7db1-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a7db1-137">Schema Name</span></span>  <br/> |<span data-ttu-id="a7db1-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a7db1-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="a7db1-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a7db1-139">Validation File</span></span>  <br/> |<span data-ttu-id="a7db1-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a7db1-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a7db1-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a7db1-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="a7db1-142">False</span><span class="sxs-lookup"><span data-stu-id="a7db1-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7db1-143">Ver também</span><span class="sxs-lookup"><span data-stu-id="a7db1-143">See also</span></span>

- [<span data-ttu-id="a7db1-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a7db1-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

