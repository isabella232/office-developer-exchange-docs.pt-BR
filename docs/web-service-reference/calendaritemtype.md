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
ms.openlocfilehash: 05e93b6db3ae574c03f6e43c5ebec2288edec3e5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527191"
---
# <a name="calendaritemtype"></a><span data-ttu-id="34e27-103">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="34e27-103">CalendarItemType</span></span>

<span data-ttu-id="34e27-104">O elemento **CalendarItemType** representa o tipo de um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="34e27-104">The **CalendarItemType** element represents the type of a calendar item.</span></span> 
  
```xml
<CalendarItemType/>
```

 <span data-ttu-id="34e27-105">**CalendarItemTypeType**</span><span class="sxs-lookup"><span data-stu-id="34e27-105">**CalendarItemTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34e27-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="34e27-106">Attributes and elements</span></span>

<span data-ttu-id="34e27-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="34e27-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34e27-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="34e27-108">Attributes</span></span>

<span data-ttu-id="34e27-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34e27-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="34e27-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="34e27-110">Child elements</span></span>

<span data-ttu-id="34e27-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="34e27-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="34e27-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="34e27-112">Parent elements</span></span>

|<span data-ttu-id="34e27-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="34e27-113">**Element**</span></span>|<span data-ttu-id="34e27-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="34e27-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34e27-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="34e27-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="34e27-116">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="34e27-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="34e27-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="34e27-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="34e27-118">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="34e27-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="34e27-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="34e27-119">Text value</span></span>

<span data-ttu-id="34e27-120">Um valor de texto será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="34e27-120">A text value is required if this element is used.</span></span> <span data-ttu-id="34e27-121">Estes são os valores possíveis para este elemento:</span><span class="sxs-lookup"><span data-stu-id="34e27-121">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="34e27-122">**Único** O item não está associado a um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="34e27-122">**Single** The item is not associated with a recurring calendar item.</span></span> 
    
- <span data-ttu-id="34e27-123">**Ocorrência** O item é uma ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="34e27-123">**Occurrence** The item is an occurrence of a recurring calendar item.</span></span> 
    
- <span data-ttu-id="34e27-124">**Exceção** O item é uma exceção a um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="34e27-124">**Exception** The item is an exception to a recurring calendar item.</span></span> 
    
- <span data-ttu-id="34e27-125">**RecurringMaster** O item é mestre para um conjunto de itens de calendário recorrentes.</span><span class="sxs-lookup"><span data-stu-id="34e27-125">**RecurringMaster** The item is master for a set of recurring calendar items.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="34e27-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="34e27-126">Remarks</span></span>

<span data-ttu-id="34e27-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="34e27-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34e27-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="34e27-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34e27-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="34e27-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="34e27-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="34e27-130">Schema name</span></span>  <br/> |<span data-ttu-id="34e27-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="34e27-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="34e27-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="34e27-132">Validation file</span></span>  <br/> |<span data-ttu-id="34e27-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="34e27-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="34e27-134">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="34e27-134">Can be empty</span></span>  <br/> |<span data-ttu-id="34e27-135">False</span><span class="sxs-lookup"><span data-stu-id="34e27-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="34e27-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="34e27-136">See also</span></span>



- [<span data-ttu-id="34e27-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="34e27-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

