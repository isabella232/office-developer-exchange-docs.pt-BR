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
description: O elemento AdjacentMeetings identifica todos os itens de calendário adjacentes a um horário de reunião.
ms.openlocfilehash: 7c89095e24af799df22a848be06a0fd65d53be7f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463577"
---
# <a name="adjacentmeetings"></a><span data-ttu-id="59060-103">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="59060-103">AdjacentMeetings</span></span>

<span data-ttu-id="59060-104">O elemento **AdjacentMeetings** identifica todos os itens de calendário adjacentes a um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="59060-104">The **AdjacentMeetings** element identifies all calendar items that are adjacent to a meeting time.</span></span> 
  
```xml
<AdjacentMeetings>
   <CalendarItem/>
</AdjacentMeetings>
```

 <span data-ttu-id="59060-105">**NonEmptyArrayOfAllItemsType**</span><span class="sxs-lookup"><span data-stu-id="59060-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59060-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="59060-106">Attributes and elements</span></span>

<span data-ttu-id="59060-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="59060-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59060-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="59060-108">Attributes</span></span>

<span data-ttu-id="59060-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="59060-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59060-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="59060-110">Child elements</span></span>

|<span data-ttu-id="59060-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="59060-111">**Element**</span></span>|<span data-ttu-id="59060-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="59060-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59060-113">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="59060-113">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="59060-114">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="59060-114">Represents an Exchange calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="59060-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="59060-115">Parent elements</span></span>

|<span data-ttu-id="59060-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="59060-116">**Element**</span></span>|<span data-ttu-id="59060-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="59060-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59060-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="59060-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="59060-119">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="59060-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="59060-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="59060-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="59060-121">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="59060-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="59060-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="59060-122">Remarks</span></span>

<span data-ttu-id="59060-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="59060-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="59060-124">Embora elementos filho adicionais sejam válidos por esquema, o elemento [CalendarItem](calendaritem.md) é o único elemento filho que os serviços Web do Exchange (EWS) retornarão dentro do elemento **AdjacentMeetings** .</span><span class="sxs-lookup"><span data-stu-id="59060-124">Although additional child elements are valid per the schema, the [CalendarItem](calendaritem.md) element is the only child element that Exchange Web Services (EWS) will return within the **AdjacentMeetings** element.</span></span> <span data-ttu-id="59060-125">Este tópico não lista os elementos filho que são válidos por esquema, mas não serão retornados pelo EWS.</span><span class="sxs-lookup"><span data-stu-id="59060-125">This topic does not list child elements that are valid per the schema but will not be returned by EWS.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="59060-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="59060-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59060-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="59060-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="59060-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="59060-128">Schema Name</span></span>  <br/> |<span data-ttu-id="59060-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="59060-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="59060-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="59060-130">Validation File</span></span>  <br/> |<span data-ttu-id="59060-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="59060-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="59060-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="59060-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="59060-133">False</span><span class="sxs-lookup"><span data-stu-id="59060-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59060-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="59060-134">See also</span></span>

- [<span data-ttu-id="59060-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="59060-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

