---
title: AppointmentState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppointmentState
api_type:
- schema
ms.assetid: ab3f5d04-ace1-4a15-9107-cefa6c41abc7
description: O elemento AppointmentState Especifica o status do compromisso.
ms.openlocfilehash: 05e92a3fea10a84518b0680c425011a91bc43d93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751190"
---
# <a name="appointmentstate"></a><span data-ttu-id="70704-103">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="70704-103">AppointmentState</span></span>

<span data-ttu-id="70704-104">O elemento **AppointmentState** Especifica o status do compromisso.</span><span class="sxs-lookup"><span data-stu-id="70704-104">The **AppointmentState** element specifies the status of the appointment.</span></span> 
  
```XML
<AppointmentState/>
```

 <span data-ttu-id="70704-105">**int**</span><span class="sxs-lookup"><span data-stu-id="70704-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70704-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="70704-106">Attributes and elements</span></span>

<span data-ttu-id="70704-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="70704-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70704-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="70704-108">Attributes</span></span>

<span data-ttu-id="70704-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="70704-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70704-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="70704-110">Child elements</span></span>

<span data-ttu-id="70704-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="70704-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="70704-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="70704-112">Parent elements</span></span>

|<span data-ttu-id="70704-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="70704-113">**Element**</span></span>|<span data-ttu-id="70704-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="70704-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70704-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="70704-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="70704-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="70704-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="70704-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="70704-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="70704-118">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="70704-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="70704-119">Text value</span><span class="sxs-lookup"><span data-stu-id="70704-119">Text value</span></span>

<span data-ttu-id="70704-120">Esse elemento contém um valor de texto que representa o conjunto de bits.</span><span class="sxs-lookup"><span data-stu-id="70704-120">This element contains a text value that represents set bits.</span></span> <span data-ttu-id="70704-121">Isso é no formulário inteiro.</span><span class="sxs-lookup"><span data-stu-id="70704-121">This is in integer form.</span></span> <span data-ttu-id="70704-122">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70704-122">This element is read-only.</span></span> <span data-ttu-id="70704-123">Ele só será retornado em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="70704-123">It will only be returned in a response.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="70704-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="70704-124">Remarks</span></span>

<span data-ttu-id="70704-125">O valor de inteiro retornado representa a máscara de bits de estado do compromisso.</span><span class="sxs-lookup"><span data-stu-id="70704-125">The integer value that is returned represents the appointment state bitmask.</span></span> <span data-ttu-id="70704-126">A tabela a seguir descreve cada bit.</span><span class="sxs-lookup"><span data-stu-id="70704-126">The following table describes each bit.</span></span>
  
|<span data-ttu-id="70704-127">**Name**</span><span class="sxs-lookup"><span data-stu-id="70704-127">**Name**</span></span>|<span data-ttu-id="70704-128">**Bit**</span><span class="sxs-lookup"><span data-stu-id="70704-128">**Bit**</span></span>|<span data-ttu-id="70704-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="70704-129">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="70704-130">None</span><span class="sxs-lookup"><span data-stu-id="70704-130">None</span></span>  <br/> |<span data-ttu-id="70704-131">0x0000</span><span class="sxs-lookup"><span data-stu-id="70704-131">0x0000</span></span>  <br/> |<span data-ttu-id="70704-132">Nenhum sinalizador foram definidos.</span><span class="sxs-lookup"><span data-stu-id="70704-132">No flags have been set.</span></span> <span data-ttu-id="70704-133">Isso é usado apenas para um compromisso que não inclui os participantes.</span><span class="sxs-lookup"><span data-stu-id="70704-133">This is only used for an appointment that does not include attendees.</span></span>  <br/> |
|<span data-ttu-id="70704-134">Reunião</span><span class="sxs-lookup"><span data-stu-id="70704-134">Meeting</span></span>  <br/> |<span data-ttu-id="70704-135">0x0001</span><span class="sxs-lookup"><span data-stu-id="70704-135">0x0001</span></span>  <br/> |<span data-ttu-id="70704-136">Este compromisso é uma reunião.</span><span class="sxs-lookup"><span data-stu-id="70704-136">This appointment is a meeting.</span></span>  <br/> |
|<span data-ttu-id="70704-137">Received</span><span class="sxs-lookup"><span data-stu-id="70704-137">Received</span></span>  <br/> |<span data-ttu-id="70704-138">0x0002</span><span class="sxs-lookup"><span data-stu-id="70704-138">0x0002</span></span>  <br/> |<span data-ttu-id="70704-139">Este compromisso foi recebido.</span><span class="sxs-lookup"><span data-stu-id="70704-139">This appointment has been received.</span></span>  <br/> |
|<span data-ttu-id="70704-140">Cancelado</span><span class="sxs-lookup"><span data-stu-id="70704-140">Canceled</span></span>  <br/> |<span data-ttu-id="70704-141">0x0004</span><span class="sxs-lookup"><span data-stu-id="70704-141">0x0004</span></span>  <br/> |<span data-ttu-id="70704-142">Este compromisso foi cancelado.</span><span class="sxs-lookup"><span data-stu-id="70704-142">This appointment has been canceled.</span></span>  <br/> |
   
<span data-ttu-id="70704-143">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="70704-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70704-144">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="70704-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70704-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="70704-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="70704-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="70704-146">Schema name</span></span>  <br/> |<span data-ttu-id="70704-147">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="70704-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="70704-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="70704-148">Validation file</span></span>  <br/> |<span data-ttu-id="70704-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="70704-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="70704-150">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="70704-150">Can be empty</span></span>  <br/> |<span data-ttu-id="70704-151">False</span><span class="sxs-lookup"><span data-stu-id="70704-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70704-152">Ver também</span><span class="sxs-lookup"><span data-stu-id="70704-152">See also</span></span>

- [<span data-ttu-id="70704-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="70704-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

