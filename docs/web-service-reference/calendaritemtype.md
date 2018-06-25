---
title: CalendarItemType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarItemType
api_type:
- schema
ms.assetid: 1feb0788-adf7-4a7c-830c-005214ad930f
description: O elemento CalendarItemType representa o tipo de um item de calendário.
ms.openlocfilehash: 3fe95c86ea24e6dfeb4740ead5e787bd63b5190d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751357"
---
# <a name="calendaritemtype"></a><span data-ttu-id="5e993-103">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="5e993-103">CalendarItemType</span></span>

<span data-ttu-id="5e993-104">O elemento **CalendarItemType** representa o tipo de um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="5e993-104">The **CalendarItemType** element represents the type of a calendar item.</span></span> 
  
```xml
<CalendarItemType/>
```

 <span data-ttu-id="5e993-105">**CalendarItemTypeType**</span><span class="sxs-lookup"><span data-stu-id="5e993-105">**CalendarItemTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5e993-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5e993-106">Attributes and elements</span></span>

<span data-ttu-id="5e993-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5e993-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5e993-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5e993-108">Attributes</span></span>

<span data-ttu-id="5e993-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5e993-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5e993-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5e993-110">Child elements</span></span>

<span data-ttu-id="5e993-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5e993-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5e993-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5e993-112">Parent elements</span></span>

|<span data-ttu-id="5e993-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5e993-113">**Element**</span></span>|<span data-ttu-id="5e993-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5e993-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e993-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5e993-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5e993-116">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5e993-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5e993-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="5e993-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="5e993-118">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5e993-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5e993-119">Text value</span><span class="sxs-lookup"><span data-stu-id="5e993-119">Text value</span></span>

<span data-ttu-id="5e993-120">Se este elemento for usado, será necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="5e993-120">A text value is required if this element is used.</span></span> <span data-ttu-id="5e993-121">Estes são os valores possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="5e993-121">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="5e993-122">**Único** O item não é associado um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="5e993-122">**Single** The item is not associated with a recurring calendar item.</span></span> 
    
- <span data-ttu-id="5e993-123">**Ocorrência** O item é uma ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="5e993-123">**Occurrence** The item is an occurrence of a recurring calendar item.</span></span> 
    
- <span data-ttu-id="5e993-124">**Exceção** O item é uma exceção a um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="5e993-124">**Exception** The item is an exception to a recurring calendar item.</span></span> 
    
- <span data-ttu-id="5e993-125">**RecurringMaster** O item é o mestre de um conjunto de itens de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="5e993-125">**RecurringMaster** The item is master for a set of recurring calendar items.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="5e993-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="5e993-126">Remarks</span></span>

<span data-ttu-id="5e993-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="5e993-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5e993-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5e993-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5e993-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="5e993-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5e993-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5e993-130">Schema name</span></span>  <br/> |<span data-ttu-id="5e993-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5e993-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="5e993-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5e993-132">Validation file</span></span>  <br/> |<span data-ttu-id="5e993-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5e993-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5e993-134">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5e993-134">Can be empty</span></span>  <br/> |<span data-ttu-id="5e993-135">False</span><span class="sxs-lookup"><span data-stu-id="5e993-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e993-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="5e993-136">See also</span></span>



- [<span data-ttu-id="5e993-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5e993-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

