---
title: ConflictingMeetingCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictingMeetingCount
api_type:
- schema
ms.assetid: 11f4d93a-b514-4a27-8d19-f4f0a35a185e
description: O elemento ConflictingMeetingCount representa o número de reuniões que estão em conflito com o item de calendário.
ms.openlocfilehash: ace800982c284cf65ff22d92c711197ee5ee1d06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751420"
---
# <a name="conflictingmeetingcount"></a><span data-ttu-id="a0871-103">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="a0871-103">ConflictingMeetingCount</span></span>

<span data-ttu-id="a0871-104">O elemento **ConflictingMeetingCount** representa o número de reuniões que estão em conflito com o item de calendário.</span><span class="sxs-lookup"><span data-stu-id="a0871-104">The **ConflictingMeetingCount** element represents the number of meetings that conflict with the calendar item.</span></span> 
  
```xml
<ConflictingMeetingCount/>
```

 <span data-ttu-id="a0871-105">**int**</span><span class="sxs-lookup"><span data-stu-id="a0871-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0871-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a0871-106">Attributes and elements</span></span>

<span data-ttu-id="a0871-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a0871-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0871-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a0871-108">Attributes</span></span>

<span data-ttu-id="a0871-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a0871-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0871-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a0871-110">Child elements</span></span>

<span data-ttu-id="a0871-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a0871-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a0871-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a0871-112">Parent elements</span></span>

|<span data-ttu-id="a0871-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a0871-113">**Element**</span></span>|<span data-ttu-id="a0871-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a0871-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0871-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="a0871-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a0871-116">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0871-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a0871-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="a0871-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a0871-118">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0871-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a0871-119">Text value</span><span class="sxs-lookup"><span data-stu-id="a0871-119">Text value</span></span>

<span data-ttu-id="a0871-120">O valor de texto representa um número inteiro.</span><span class="sxs-lookup"><span data-stu-id="a0871-120">The text value represents an integer.</span></span> <span data-ttu-id="a0871-121">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a0871-121">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a0871-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="a0871-122">Remarks</span></span>

<span data-ttu-id="a0871-123">Um item de calendário é considerado conflitante se ele ocorrer, pelo menos em parte, ao mesmo tempo como outro item de calendário na mesma pasta Calendário.</span><span class="sxs-lookup"><span data-stu-id="a0871-123">A calendar item is considered conflicting if it occurs, at least in part, at the same time as another calendar item in the same calendar folder.</span></span> <span data-ttu-id="a0871-124">Se um item de calendário estiver em uma pasta noncalendar, ele é comparado com itens de calendário na pasta de calendário padrão.</span><span class="sxs-lookup"><span data-stu-id="a0871-124">If a calendar item is in a noncalendar folder, it is compared with calendar items in the default calendar folder.</span></span> <span data-ttu-id="a0871-125">Solicitações de reunião são comparadas com itens de calendário na pasta de calendário padrão.</span><span class="sxs-lookup"><span data-stu-id="a0871-125">Meeting requests are compared with calendar items in the default calendar folder.</span></span>
  
<span data-ttu-id="a0871-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="a0871-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0871-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a0871-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0871-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="a0871-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a0871-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a0871-129">Schema name</span></span>  <br/> |<span data-ttu-id="a0871-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a0871-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="a0871-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a0871-131">Validation file</span></span>  <br/> |<span data-ttu-id="a0871-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a0871-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a0871-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a0871-133">Can be empty</span></span>  <br/> |<span data-ttu-id="a0871-134">False</span><span class="sxs-lookup"><span data-stu-id="a0871-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0871-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="a0871-135">See also</span></span>



- [<span data-ttu-id="a0871-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a0871-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

