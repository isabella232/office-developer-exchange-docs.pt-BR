---
title: ModifiedOccurrences
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ModifiedOccurrences
api_type:
- schema
ms.assetid: 552932fc-b3b4-486e-8d73-32c0bb10bd68
description: O elemento ModifiedOccurrences contém uma matriz de recorrente ocorrências de item de calendário que foram modificados para que sejam diferentes do que o item de recorrência mestre.
ms.openlocfilehash: 53f60740bcaa2de6713e1b6a3d2874153285645a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824472"
---
# <a name="modifiedoccurrences"></a><span data-ttu-id="5a972-103">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="5a972-103">ModifiedOccurrences</span></span>

<span data-ttu-id="5a972-104">O elemento **ModifiedOccurrences** contém uma matriz de recorrente ocorrências de item de calendário que foram modificados para que sejam diferentes do que o item de recorrência mestre.</span><span class="sxs-lookup"><span data-stu-id="5a972-104">The **ModifiedOccurrences** element contains an array of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span> 
  
```xml
<ModifiedOccurrences>
   <Occurrence/>
</ModifiedOccurrences>
```

 <span data-ttu-id="5a972-105">**NonEmptyArrayOfOccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="5a972-105">**NonEmptyArrayOfOccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a972-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5a972-106">Attributes and elements</span></span>

<span data-ttu-id="5a972-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5a972-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a972-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5a972-108">Attributes</span></span>

<span data-ttu-id="5a972-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5a972-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a972-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5a972-110">Child elements</span></span>

|<span data-ttu-id="5a972-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5a972-111">**Element**</span></span>|<span data-ttu-id="5a972-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5a972-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a972-113">Ocorrência</span><span class="sxs-lookup"><span data-stu-id="5a972-113">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="5a972-114">Representa uma única ocorrência de modificação de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="5a972-114">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5a972-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5a972-115">Parent elements</span></span>

|<span data-ttu-id="5a972-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5a972-116">**Element**</span></span>|<span data-ttu-id="5a972-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5a972-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a972-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="5a972-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="5a972-119">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a972-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5a972-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5a972-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5a972-121">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a972-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5a972-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="5a972-122">Remarks</span></span>

<span data-ttu-id="5a972-123">Esse elemento é válido se [CalendarItemType](calendaritemtype.md) tem o valor de RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="5a972-123">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="5a972-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="5a972-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a972-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5a972-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a972-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="5a972-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5a972-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5a972-127">Schema name</span></span>  <br/> |<span data-ttu-id="5a972-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5a972-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="5a972-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5a972-129">Validation file</span></span>  <br/> |<span data-ttu-id="5a972-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5a972-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5a972-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5a972-131">Can be empty</span></span>  <br/> |<span data-ttu-id="5a972-132">False</span><span class="sxs-lookup"><span data-stu-id="5a972-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a972-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="5a972-133">See also</span></span>



- [<span data-ttu-id="5a972-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5a972-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

