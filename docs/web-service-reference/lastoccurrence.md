---
title: LastOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LastOccurrence
api_type:
- schema
ms.assetid: c9ef0fcb-4265-4e60-9986-fff0f211d00b
description: O elemento LastOccurrence representa a última ocorrência de um item de calendário recorrente.
ms.openlocfilehash: 2c8fdfc0005e86c9dda84a48ae1d3692b5134ca8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824209"
---
# <a name="lastoccurrence"></a><span data-ttu-id="7c377-103">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="7c377-103">LastOccurrence</span></span>

<span data-ttu-id="7c377-104">O elemento **LastOccurrence** representa a última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="7c377-104">The **LastOccurrence** element represents the last occurrence of a recurring calendar item.</span></span> 
  
```xml
<LastOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</LastOccurrence>
```

 <span data-ttu-id="7c377-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="7c377-105">**OccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c377-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7c377-106">Attributes and elements</span></span>

<span data-ttu-id="7c377-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7c377-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c377-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7c377-108">Attributes</span></span>

<span data-ttu-id="7c377-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7c377-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c377-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7c377-110">Child elements</span></span>

|<span data-ttu-id="7c377-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7c377-111">**Element**</span></span>|<span data-ttu-id="7c377-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7c377-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c377-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="7c377-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="7c377-114">Contém o identificador e alterar a chave exclusiva da última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="7c377-114">Contains the unique identifier and change key of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7c377-115">Start</span><span class="sxs-lookup"><span data-stu-id="7c377-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="7c377-116">Representa a hora de início da última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="7c377-116">Represents the start time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7c377-117">End</span><span class="sxs-lookup"><span data-stu-id="7c377-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7c377-118">Representa a hora de término da última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="7c377-118">Represents the end time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7c377-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="7c377-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="7c377-120">Representa a hora de início original da última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="7c377-120">Represents the original start time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c377-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7c377-121">Parent elements</span></span>

|<span data-ttu-id="7c377-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7c377-122">**Element**</span></span>|<span data-ttu-id="7c377-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7c377-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c377-124">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="7c377-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="7c377-125">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c377-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7c377-126">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="7c377-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="7c377-127">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c377-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c377-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="7c377-128">Remarks</span></span>

<span data-ttu-id="7c377-129">Esse elemento é válido se [CalendarItemType](calendaritemtype.md) tem o valor de RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="7c377-129">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="7c377-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7c377-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c377-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7c377-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c377-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="7c377-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c377-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7c377-133">Schema name</span></span>  <br/> |<span data-ttu-id="7c377-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7c377-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c377-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7c377-135">Validation file</span></span>  <br/> |<span data-ttu-id="7c377-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7c377-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c377-137">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="7c377-137">Can be empty</span></span>  <br/> |<span data-ttu-id="7c377-138">False</span><span class="sxs-lookup"><span data-stu-id="7c377-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c377-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="7c377-139">See also</span></span>



- [<span data-ttu-id="7c377-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7c377-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="7c377-141">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="7c377-141">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

