---
title: ConflictingMeetings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictingMeetings
api_type:
- schema
ms.assetid: cfff7a11-7b3a-4995-9815-afedd45ebb0f
description: O elemento ConflictingMeetings identifica todos os itens de calendário que entram em conflito com um horário de reunião.
ms.openlocfilehash: dc897c9dc33117d379d89bb9bb41104ca02def1f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460173"
---
# <a name="conflictingmeetings"></a><span data-ttu-id="692be-103">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="692be-103">ConflictingMeetings</span></span>

<span data-ttu-id="692be-104">O elemento **ConflictingMeetings** identifica todos os itens de calendário que entram em conflito com um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="692be-104">The **ConflictingMeetings** element identifies all calendar items that conflict with a meeting time.</span></span> 
  
```xml
<ConflictingMeetings>
   <CalendarItem/>
</ConflictingMeetings>
```

 <span data-ttu-id="692be-105">**NonEmptyArrayOfAllItemsType**</span><span class="sxs-lookup"><span data-stu-id="692be-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="692be-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="692be-106">Attributes and elements</span></span>

<span data-ttu-id="692be-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="692be-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="692be-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="692be-108">Attributes</span></span>

<span data-ttu-id="692be-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="692be-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="692be-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="692be-110">Child elements</span></span>

|<span data-ttu-id="692be-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="692be-111">**Element**</span></span>|<span data-ttu-id="692be-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="692be-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="692be-113">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="692be-113">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="692be-114">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="692be-114">Represents an Exchange calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="692be-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="692be-115">Parent elements</span></span>

|<span data-ttu-id="692be-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="692be-116">**Element**</span></span>|<span data-ttu-id="692be-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="692be-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="692be-118">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="692be-118">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="692be-119">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="692be-119">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="692be-120">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="692be-120">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="692be-121">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="692be-121">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="692be-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="692be-122">Remarks</span></span>

<span data-ttu-id="692be-123">Se esse elemento for usado, ele deve conter um ou mais elementos filhos.</span><span class="sxs-lookup"><span data-stu-id="692be-123">If this element is used, it must contain one or more child elements.</span></span>
  
<span data-ttu-id="692be-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="692be-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="692be-125">Embora elementos filho adicionais sejam válidos por esquema, o elemento [CalendarItem](calendaritem.md) é o único elemento filho que os serviços Web do Exchange (EWS) retornarão dentro do elemento **ConflictingMeetings** .</span><span class="sxs-lookup"><span data-stu-id="692be-125">Although additional child elements are valid per the schema, the [CalendarItem](calendaritem.md) element is the only child element that Exchange Web Services (EWS) will return within the **ConflictingMeetings** element.</span></span> <span data-ttu-id="692be-126">Este tópico não lista os elementos filho que são válidos por esquema, mas não serão retornados pelo EWS.</span><span class="sxs-lookup"><span data-stu-id="692be-126">This topic does not list child elements that are valid per the schema but will not be returned by EWS.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="692be-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="692be-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="692be-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="692be-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="692be-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="692be-129">Schema Name</span></span>  <br/> |<span data-ttu-id="692be-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="692be-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="692be-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="692be-131">Validation File</span></span>  <br/> |<span data-ttu-id="692be-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="692be-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="692be-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="692be-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="692be-134">False</span><span class="sxs-lookup"><span data-stu-id="692be-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="692be-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="692be-135">See also</span></span>



- [<span data-ttu-id="692be-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="692be-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

