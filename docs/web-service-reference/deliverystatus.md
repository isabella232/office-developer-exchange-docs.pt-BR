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
description: O elemento DeliveryStatus especifica o status de uma mensagem.
ms.openlocfilehash: ae32202284d3dd272f693fbb7b76070cb6019d28
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461398"
---
# <a name="deliverystatus"></a><span data-ttu-id="4c0a7-103">DeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="4c0a7-103">DeliveryStatus</span></span>

<span data-ttu-id="4c0a7-104">O elemento **DeliveryStatus** especifica o status de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="4c0a7-104">The **DeliveryStatus** element specifies the status for a message.</span></span> 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 <span data-ttu-id="4c0a7-105">**MessageTrackingDeliveryStatusType**</span><span class="sxs-lookup"><span data-stu-id="4c0a7-105">**MessageTrackingDeliveryStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4c0a7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4c0a7-106">Attributes and elements</span></span>

<span data-ttu-id="4c0a7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4c0a7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c0a7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4c0a7-108">Attributes</span></span>

<span data-ttu-id="4c0a7-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4c0a7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4c0a7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4c0a7-110">Child elements</span></span>

<span data-ttu-id="4c0a7-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4c0a7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4c0a7-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4c0a7-112">Parent elements</span></span>

|<span data-ttu-id="4c0a7-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4c0a7-113">**Element**</span></span>|<span data-ttu-id="4c0a7-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4c0a7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c0a7-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="4c0a7-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="4c0a7-116">Contém informações de um único evento para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="4c0a7-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4c0a7-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="4c0a7-117">Text value</span></span>

<span data-ttu-id="4c0a7-118">A tabela a seguir lista os valores de texto possíveis para o elemento **DeliveryStatus** .</span><span class="sxs-lookup"><span data-stu-id="4c0a7-118">The following table lists the possible text values for the **DeliveryStatus** element.</span></span> 
  
<span data-ttu-id="4c0a7-119">**Valores do elemento DeliveryStatus**</span><span class="sxs-lookup"><span data-stu-id="4c0a7-119">**DeliveryStatus element values**</span></span>

|<span data-ttu-id="4c0a7-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="4c0a7-120">**Value**</span></span>|<span data-ttu-id="4c0a7-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4c0a7-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4c0a7-122">Sucedida</span><span class="sxs-lookup"><span data-stu-id="4c0a7-122">Unsuccessful</span></span>  <br/> |<span data-ttu-id="4c0a7-123">Especifica que uma mensagem não foi entregue.</span><span class="sxs-lookup"><span data-stu-id="4c0a7-123">Specifies that a message was not delivered.</span></span>  <br/> |
|<span data-ttu-id="4c0a7-124">Pending</span><span class="sxs-lookup"><span data-stu-id="4c0a7-124">Pending</span></span>  <br/> |<span data-ttu-id="4c0a7-125">Especifica que a mensagem está aguardando aprovação de um moderador.</span><span class="sxs-lookup"><span data-stu-id="4c0a7-125">Specifies that the message is waiting for approval from a moderator.</span></span>  <br/> |
|<span data-ttu-id="4c0a7-126">Gerados</span><span class="sxs-lookup"><span data-stu-id="4c0a7-126">Delivered</span></span>  <br/> |<span data-ttu-id="4c0a7-127">Especifica que a mensagem foi entregue a todos os destinatários especificados.</span><span class="sxs-lookup"><span data-stu-id="4c0a7-127">Specifies that the message was delivered to all of the specified recipients.</span></span>  <br/> |
|<span data-ttu-id="4c0a7-128">Enviados</span><span class="sxs-lookup"><span data-stu-id="4c0a7-128">Transferred</span></span>  <br/> |<span data-ttu-id="4c0a7-129">Especifica que a mensagem foi transferida para um servidor fora do escopo de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4c0a7-129">Specifies that the message was transferred to a server outside the search scope.</span></span>  <br/> |
|<span data-ttu-id="4c0a7-130">Ler</span><span class="sxs-lookup"><span data-stu-id="4c0a7-130">Read</span></span>  <br/> |<span data-ttu-id="4c0a7-131">Especifica que a mensagem foi entregue e lida pelos destinatários.</span><span class="sxs-lookup"><span data-stu-id="4c0a7-131">Specifies that the message was delivered and read by the recipients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4c0a7-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="4c0a7-132">Remarks</span></span>

<span data-ttu-id="4c0a7-133">O elemento **DeliveryStatus** era do tipo **MessageTrackingDeliveryStatusType** no Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="4c0a7-133">The **DeliveryStatus** element was of type **MessageTrackingDeliveryStatusType** in Exchange Server 2010.</span></span> 
  
<span data-ttu-id="4c0a7-134">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4c0a7-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4c0a7-135">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4c0a7-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4c0a7-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="4c0a7-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4c0a7-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4c0a7-137">Schema Name</span></span>  <br/> |<span data-ttu-id="4c0a7-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4c0a7-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="4c0a7-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4c0a7-139">Validation File</span></span>  <br/> |<span data-ttu-id="4c0a7-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4c0a7-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4c0a7-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4c0a7-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="4c0a7-142">False</span><span class="sxs-lookup"><span data-stu-id="4c0a7-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4c0a7-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="4c0a7-143">See also</span></span>

- [<span data-ttu-id="4c0a7-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4c0a7-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

