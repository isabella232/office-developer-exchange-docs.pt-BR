---
title: Compromissostate
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
description: O elemento Compromissostate especifica o status do compromisso.
ms.openlocfilehash: 8b0e827d02e9051f31d43199503dc286c50e2125
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463472"
---
# <a name="appointmentstate"></a><span data-ttu-id="25125-103">Compromissostate</span><span class="sxs-lookup"><span data-stu-id="25125-103">AppointmentState</span></span>

<span data-ttu-id="25125-104">O elemento **compromissostate** especifica o status do compromisso.</span><span class="sxs-lookup"><span data-stu-id="25125-104">The **AppointmentState** element specifies the status of the appointment.</span></span> 
  
```XML
<AppointmentState/>
```

 <span data-ttu-id="25125-105">**int**</span><span class="sxs-lookup"><span data-stu-id="25125-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25125-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="25125-106">Attributes and elements</span></span>

<span data-ttu-id="25125-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="25125-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25125-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="25125-108">Attributes</span></span>

<span data-ttu-id="25125-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25125-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25125-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="25125-110">Child elements</span></span>

<span data-ttu-id="25125-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="25125-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="25125-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="25125-112">Parent elements</span></span>

|<span data-ttu-id="25125-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="25125-113">**Element**</span></span>|<span data-ttu-id="25125-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="25125-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25125-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="25125-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="25125-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="25125-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="25125-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="25125-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="25125-118">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="25125-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="25125-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="25125-119">Text value</span></span>

<span data-ttu-id="25125-120">Este elemento contém um valor de texto que representa os bits de conjunto.</span><span class="sxs-lookup"><span data-stu-id="25125-120">This element contains a text value that represents set bits.</span></span> <span data-ttu-id="25125-121">Isso está no formato de inteiro.</span><span class="sxs-lookup"><span data-stu-id="25125-121">This is in integer form.</span></span> <span data-ttu-id="25125-122">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25125-122">This element is read-only.</span></span> <span data-ttu-id="25125-123">Ele só será retornado em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="25125-123">It will only be returned in a response.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="25125-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="25125-124">Remarks</span></span>

<span data-ttu-id="25125-125">O valor inteiro retornado representa a bitmask do estado do compromisso.</span><span class="sxs-lookup"><span data-stu-id="25125-125">The integer value that is returned represents the appointment state bitmask.</span></span> <span data-ttu-id="25125-126">A tabela a seguir descreve cada bit.</span><span class="sxs-lookup"><span data-stu-id="25125-126">The following table describes each bit.</span></span>
  
|<span data-ttu-id="25125-127">**Nome**</span><span class="sxs-lookup"><span data-stu-id="25125-127">**Name**</span></span>|<span data-ttu-id="25125-128">**Bits**</span><span class="sxs-lookup"><span data-stu-id="25125-128">**Bit**</span></span>|<span data-ttu-id="25125-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="25125-129">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="25125-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25125-130">None</span></span>  <br/> |<span data-ttu-id="25125-131">0x0000</span><span class="sxs-lookup"><span data-stu-id="25125-131">0x0000</span></span>  <br/> |<span data-ttu-id="25125-132">Nenhum sinalizador foi definido.</span><span class="sxs-lookup"><span data-stu-id="25125-132">No flags have been set.</span></span> <span data-ttu-id="25125-133">Isso é usado apenas para um compromisso que não inclua participantes.</span><span class="sxs-lookup"><span data-stu-id="25125-133">This is only used for an appointment that does not include attendees.</span></span>  <br/> |
|<span data-ttu-id="25125-134">Atenda</span><span class="sxs-lookup"><span data-stu-id="25125-134">Meeting</span></span>  <br/> |<span data-ttu-id="25125-135">0x0001</span><span class="sxs-lookup"><span data-stu-id="25125-135">0x0001</span></span>  <br/> |<span data-ttu-id="25125-136">Este compromisso é uma reunião.</span><span class="sxs-lookup"><span data-stu-id="25125-136">This appointment is a meeting.</span></span>  <br/> |
|<span data-ttu-id="25125-137">Received</span><span class="sxs-lookup"><span data-stu-id="25125-137">Received</span></span>  <br/> |<span data-ttu-id="25125-138">0x0002</span><span class="sxs-lookup"><span data-stu-id="25125-138">0x0002</span></span>  <br/> |<span data-ttu-id="25125-139">Este compromisso foi recebido.</span><span class="sxs-lookup"><span data-stu-id="25125-139">This appointment has been received.</span></span>  <br/> |
|<span data-ttu-id="25125-140">Foi</span><span class="sxs-lookup"><span data-stu-id="25125-140">Canceled</span></span>  <br/> |<span data-ttu-id="25125-141">0x0004</span><span class="sxs-lookup"><span data-stu-id="25125-141">0x0004</span></span>  <br/> |<span data-ttu-id="25125-142">Este compromisso foi cancelado.</span><span class="sxs-lookup"><span data-stu-id="25125-142">This appointment has been canceled.</span></span>  <br/> |
   
<span data-ttu-id="25125-143">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="25125-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25125-144">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="25125-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25125-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="25125-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25125-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="25125-146">Schema name</span></span>  <br/> |<span data-ttu-id="25125-147">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="25125-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="25125-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="25125-148">Validation file</span></span>  <br/> |<span data-ttu-id="25125-149">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="25125-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="25125-150">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="25125-150">Can be empty</span></span>  <br/> |<span data-ttu-id="25125-151">False</span><span class="sxs-lookup"><span data-stu-id="25125-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="25125-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="25125-152">See also</span></span>

- [<span data-ttu-id="25125-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="25125-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

