---
title: AdjacentMeetings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdjacentMeetings
api_type:
- schema
ms.assetid: 50a9c381-9166-476e-8421-29e51b94499b
description: O elemento AdjacentMeetings identifica todos os itens de calendário que são adjacentes para um horário de reunião.
ms.openlocfilehash: 9ab818f4f67c32c01101cc595ccb92424a872ef0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751070"
---
# <a name="adjacentmeetings"></a><span data-ttu-id="cfb46-103">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="cfb46-103">AdjacentMeetings</span></span>

<span data-ttu-id="cfb46-104">O elemento **AdjacentMeetings** identifica todos os itens de calendário que são adjacentes para um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="cfb46-104">The **AdjacentMeetings** element identifies all calendar items that are adjacent to a meeting time.</span></span> 
  
```xml
<AdjacentMeetings>
   <CalendarItem/>
</AdjacentMeetings>
```

 <span data-ttu-id="cfb46-105">**NonEmptyArrayOfAllItemsType**</span><span class="sxs-lookup"><span data-stu-id="cfb46-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cfb46-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="cfb46-106">Attributes and elements</span></span>

<span data-ttu-id="cfb46-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cfb46-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cfb46-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cfb46-108">Attributes</span></span>

<span data-ttu-id="cfb46-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cfb46-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cfb46-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cfb46-110">Child elements</span></span>

|<span data-ttu-id="cfb46-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cfb46-111">**Element**</span></span>|<span data-ttu-id="cfb46-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cfb46-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cfb46-113">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="cfb46-113">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="cfb46-114">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cfb46-114">Represents an Exchange calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cfb46-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cfb46-115">Parent elements</span></span>

|<span data-ttu-id="cfb46-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cfb46-116">**Element**</span></span>|<span data-ttu-id="cfb46-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cfb46-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cfb46-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="cfb46-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="cfb46-119">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cfb46-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="cfb46-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="cfb46-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="cfb46-121">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cfb46-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cfb46-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="cfb46-122">Remarks</span></span>

<span data-ttu-id="cfb46-123">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="cfb46-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="cfb46-124">Embora os elementos filho adicionais são válidos pelo esquema, o [CalendarItem](calendaritem.md) é o elemento filho somente que retornará os serviços Web do Exchange (EWS) dentro do elemento **AdjacentMeetings** .</span><span class="sxs-lookup"><span data-stu-id="cfb46-124">Although additional child elements are valid per the schema, the [CalendarItem](calendaritem.md) element is the only child element that Exchange Web Services (EWS) will return within the **AdjacentMeetings** element.</span></span> <span data-ttu-id="cfb46-125">Este tópico não lista os elementos filhos que são válidas pelo esquema, mas não serão retornados por EWS.</span><span class="sxs-lookup"><span data-stu-id="cfb46-125">This topic does not list child elements that are valid per the schema but will not be returned by EWS.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="cfb46-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="cfb46-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cfb46-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="cfb46-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cfb46-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cfb46-128">Schema Name</span></span>  <br/> |<span data-ttu-id="cfb46-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="cfb46-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="cfb46-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cfb46-130">Validation File</span></span>  <br/> |<span data-ttu-id="cfb46-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cfb46-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cfb46-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cfb46-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="cfb46-133">False</span><span class="sxs-lookup"><span data-stu-id="cfb46-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cfb46-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="cfb46-134">See also</span></span>

- [<span data-ttu-id="cfb46-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cfb46-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

