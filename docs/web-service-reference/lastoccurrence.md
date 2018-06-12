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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824209"
---
# <a name="lastoccurrence"></a><span data-ttu-id="9f989-103">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="9f989-103">LastOccurrence</span></span>

<span data-ttu-id="9f989-104">O elemento **LastOccurrence** representa a última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="9f989-104">The **LastOccurrence** element represents the last occurrence of a recurring calendar item.</span></span> 
  
```xml
<LastOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</LastOccurrence>
```

 <span data-ttu-id="9f989-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="9f989-105">**OccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f989-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9f989-106">Attributes and elements</span></span>

<span data-ttu-id="9f989-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9f989-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f989-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9f989-108">Attributes</span></span>

<span data-ttu-id="9f989-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9f989-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f989-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9f989-110">Child elements</span></span>

|<span data-ttu-id="9f989-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9f989-111">**Element**</span></span>|<span data-ttu-id="9f989-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9f989-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f989-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="9f989-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="9f989-114">Contém o identificador e alterar a chave exclusiva da última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="9f989-114">Contains the unique identifier and change key of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9f989-115">Start</span><span class="sxs-lookup"><span data-stu-id="9f989-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="9f989-116">Representa a hora de início da última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="9f989-116">Represents the start time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9f989-117">End</span><span class="sxs-lookup"><span data-stu-id="9f989-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9f989-118">Representa a hora de término da última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="9f989-118">Represents the end time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9f989-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="9f989-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="9f989-120">Representa a hora de início original da última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="9f989-120">Represents the original start time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f989-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9f989-121">Parent elements</span></span>

|<span data-ttu-id="9f989-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9f989-122">**Element**</span></span>|<span data-ttu-id="9f989-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9f989-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f989-124">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="9f989-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="9f989-125">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f989-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9f989-126">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="9f989-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="9f989-127">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f989-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9f989-128">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="9f989-128">Remarks</span></span>

<span data-ttu-id="9f989-129">Esse elemento é válido se [CalendarItemType](calendaritemtype.md) tem o valor de RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="9f989-129">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="9f989-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="9f989-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f989-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9f989-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f989-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="9f989-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9f989-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9f989-133">Schema name</span></span>  <br/> |<span data-ttu-id="9f989-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9f989-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="9f989-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9f989-135">Validation file</span></span>  <br/> |<span data-ttu-id="9f989-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9f989-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9f989-137">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9f989-137">Can be empty</span></span>  <br/> |<span data-ttu-id="9f989-138">False</span><span class="sxs-lookup"><span data-stu-id="9f989-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f989-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="9f989-139">See also</span></span>



- [<span data-ttu-id="9f989-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9f989-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="9f989-141">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="9f989-141">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

