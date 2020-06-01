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
ms.openlocfilehash: 8771bbed166cfb6fdcf4d1dfe4fa0812013e2667
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459809"
---
# <a name="lastoccurrence"></a><span data-ttu-id="ae6a1-103">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="ae6a1-103">LastOccurrence</span></span>

<span data-ttu-id="ae6a1-104">O elemento **LastOccurrence** representa a última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-104">The **LastOccurrence** element represents the last occurrence of a recurring calendar item.</span></span> 
  
```xml
<LastOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</LastOccurrence>
```

 <span data-ttu-id="ae6a1-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="ae6a1-105">**OccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae6a1-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ae6a1-106">Attributes and elements</span></span>

<span data-ttu-id="ae6a1-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae6a1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ae6a1-108">Attributes</span></span>

<span data-ttu-id="ae6a1-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ae6a1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae6a1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ae6a1-110">Child elements</span></span>

|<span data-ttu-id="ae6a1-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ae6a1-111">**Element**</span></span>|<span data-ttu-id="ae6a1-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ae6a1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae6a1-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="ae6a1-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ae6a1-114">Contém o identificador exclusivo e a chave de alteração da última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-114">Contains the unique identifier and change key of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ae6a1-115">Start</span><span class="sxs-lookup"><span data-stu-id="ae6a1-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="ae6a1-116">Representa a hora de início da última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-116">Represents the start time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ae6a1-117">Ponto</span><span class="sxs-lookup"><span data-stu-id="ae6a1-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ae6a1-118">Representa a hora de término da última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-118">Represents the end time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ae6a1-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="ae6a1-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="ae6a1-120">Representa a hora de início original da última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-120">Represents the original start time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ae6a1-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ae6a1-121">Parent elements</span></span>

|<span data-ttu-id="ae6a1-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ae6a1-122">**Element**</span></span>|<span data-ttu-id="ae6a1-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ae6a1-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae6a1-124">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ae6a1-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ae6a1-125">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ae6a1-126">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ae6a1-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ae6a1-127">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ae6a1-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="ae6a1-128">Remarks</span></span>

<span data-ttu-id="ae6a1-129">Este elemento é válido se [CalendarItemType](calendaritemtype.md) tiver o valor RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-129">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="ae6a1-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae6a1-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ae6a1-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae6a1-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="ae6a1-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ae6a1-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ae6a1-133">Schema name</span></span>  <br/> |<span data-ttu-id="ae6a1-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ae6a1-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="ae6a1-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ae6a1-135">Validation file</span></span>  <br/> |<span data-ttu-id="ae6a1-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ae6a1-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ae6a1-137">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ae6a1-137">Can be empty</span></span>  <br/> |<span data-ttu-id="ae6a1-138">False</span><span class="sxs-lookup"><span data-stu-id="ae6a1-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae6a1-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="ae6a1-139">See also</span></span>



- [<span data-ttu-id="ae6a1-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ae6a1-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="ae6a1-141">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="ae6a1-141">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

