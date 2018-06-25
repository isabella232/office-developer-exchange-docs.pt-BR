---
title: AdjacentMeetingCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdjacentMeetingCount
api_type:
- schema
ms.assetid: 35045024-f6e1-47d1-89be-f100b7b4f3c7
description: O elemento AdjacentMeetingCount representa o número total de itens de calendário que sejam adjacentes um horário de reunião.
ms.openlocfilehash: a00468bec392498745fe778b627259a79d6027bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751068"
---
# <a name="adjacentmeetingcount"></a><span data-ttu-id="11350-103">AdjacentMeetingCount</span><span class="sxs-lookup"><span data-stu-id="11350-103">AdjacentMeetingCount</span></span>

<span data-ttu-id="11350-104">O elemento **AdjacentMeetingCount** representa o número total de itens de calendário que sejam adjacentes um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="11350-104">The **AdjacentMeetingCount** element represents the total number of calendar items that are adjacent to a meeting time.</span></span> 
  
```xml
<AdjacentMeetingCount/>
```

 <span data-ttu-id="11350-105">**Int**</span><span class="sxs-lookup"><span data-stu-id="11350-105">**Int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11350-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="11350-106">Attributes and elements</span></span>

<span data-ttu-id="11350-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="11350-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11350-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="11350-108">Attributes</span></span>

<span data-ttu-id="11350-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="11350-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="11350-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="11350-110">Child elements</span></span>

<span data-ttu-id="11350-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="11350-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="11350-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="11350-112">Parent elements</span></span>

|<span data-ttu-id="11350-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="11350-113">**Element**</span></span>|<span data-ttu-id="11350-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="11350-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11350-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="11350-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="11350-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11350-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="11350-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="11350-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="11350-118">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11350-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="11350-119">Text value</span><span class="sxs-lookup"><span data-stu-id="11350-119">Text value</span></span>

<span data-ttu-id="11350-120">É necessário um valor de texto que representa um número inteiro.</span><span class="sxs-lookup"><span data-stu-id="11350-120">A text value that represents an integer is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="11350-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="11350-121">Remarks</span></span>

<span data-ttu-id="11350-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="11350-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11350-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="11350-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11350-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="11350-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="11350-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="11350-125">Schema name</span></span>  <br/> |<span data-ttu-id="11350-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="11350-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="11350-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="11350-127">Validation file</span></span>  <br/> |<span data-ttu-id="11350-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="11350-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="11350-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="11350-129">Can be empty</span></span>  <br/> |<span data-ttu-id="11350-130">False</span><span class="sxs-lookup"><span data-stu-id="11350-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="11350-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="11350-131">See also</span></span>

- [<span data-ttu-id="11350-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="11350-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

