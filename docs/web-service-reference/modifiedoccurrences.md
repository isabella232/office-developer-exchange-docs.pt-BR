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
description: O elemento ModifiedOccurrences contém uma matriz de ocorrências de itens de calendário recorrentes que foram modificadas para que sejam diferentes do item mestre de recorrência.
ms.openlocfilehash: d599e3d232bfffc5bedd37f3dae4d8b10a82ffde
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530419"
---
# <a name="modifiedoccurrences"></a><span data-ttu-id="c7858-103">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="c7858-103">ModifiedOccurrences</span></span>

<span data-ttu-id="c7858-104">O elemento **ModifiedOccurrences** contém uma matriz de ocorrências de itens de calendário recorrentes que foram modificadas para que sejam diferentes do item mestre de recorrência.</span><span class="sxs-lookup"><span data-stu-id="c7858-104">The **ModifiedOccurrences** element contains an array of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span> 
  
```xml
<ModifiedOccurrences>
   <Occurrence/>
</ModifiedOccurrences>
```

 <span data-ttu-id="c7858-105">**NonEmptyArrayOfOccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="c7858-105">**NonEmptyArrayOfOccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c7858-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c7858-106">Attributes and elements</span></span>

<span data-ttu-id="c7858-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c7858-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7858-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c7858-108">Attributes</span></span>

<span data-ttu-id="c7858-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7858-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c7858-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c7858-110">Child elements</span></span>

|<span data-ttu-id="c7858-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c7858-111">**Element**</span></span>|<span data-ttu-id="c7858-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c7858-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7858-113">Ocorrência</span><span class="sxs-lookup"><span data-stu-id="c7858-113">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="c7858-114">Representa uma única ocorrência modificada de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="c7858-114">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c7858-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c7858-115">Parent elements</span></span>

|<span data-ttu-id="c7858-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c7858-116">**Element**</span></span>|<span data-ttu-id="c7858-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c7858-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7858-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="c7858-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c7858-119">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7858-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c7858-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c7858-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c7858-121">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7858-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c7858-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="c7858-122">Remarks</span></span>

<span data-ttu-id="c7858-123">Este elemento é válido se [CalendarItemType](calendaritemtype.md) tiver o valor RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="c7858-123">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="c7858-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c7858-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c7858-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c7858-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7858-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="c7858-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c7858-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c7858-127">Schema name</span></span>  <br/> |<span data-ttu-id="c7858-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c7858-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="c7858-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c7858-129">Validation file</span></span>  <br/> |<span data-ttu-id="c7858-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c7858-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c7858-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c7858-131">Can be empty</span></span>  <br/> |<span data-ttu-id="c7858-132">False</span><span class="sxs-lookup"><span data-stu-id="c7858-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c7858-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="c7858-133">See also</span></span>



- [<span data-ttu-id="c7858-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c7858-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

