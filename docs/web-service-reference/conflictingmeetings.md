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
description: O elemento ConflictingMeetings identifica todos os itens de calendário que estão em conflito com um tempo de reunião.
ms.openlocfilehash: 1d2558dba41ec3e7ae2711bb2dc26f54cada827a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751422"
---
# <a name="conflictingmeetings"></a><span data-ttu-id="88643-103">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="88643-103">ConflictingMeetings</span></span>

<span data-ttu-id="88643-104">O elemento **ConflictingMeetings** identifica todos os itens de calendário que estão em conflito com um tempo de reunião.</span><span class="sxs-lookup"><span data-stu-id="88643-104">The **ConflictingMeetings** element identifies all calendar items that conflict with a meeting time.</span></span> 
  
```xml
<ConflictingMeetings>
   <CalendarItem/>
</ConflictingMeetings>
```

 <span data-ttu-id="88643-105">**NonEmptyArrayOfAllItemsType**</span><span class="sxs-lookup"><span data-stu-id="88643-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88643-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="88643-106">Attributes and elements</span></span>

<span data-ttu-id="88643-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="88643-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88643-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="88643-108">Attributes</span></span>

<span data-ttu-id="88643-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="88643-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88643-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="88643-110">Child elements</span></span>

|<span data-ttu-id="88643-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="88643-111">**Element**</span></span>|<span data-ttu-id="88643-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="88643-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88643-113">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="88643-113">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="88643-114">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="88643-114">Represents an Exchange calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88643-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="88643-115">Parent elements</span></span>

|<span data-ttu-id="88643-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="88643-116">**Element**</span></span>|<span data-ttu-id="88643-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="88643-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88643-118">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="88643-118">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="88643-119">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="88643-119">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="88643-120">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="88643-120">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="88643-121">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="88643-121">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="88643-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="88643-122">Remarks</span></span>

<span data-ttu-id="88643-123">Se este elemento for usado, ele deve conter um ou mais elementos filho.</span><span class="sxs-lookup"><span data-stu-id="88643-123">If this element is used, it must contain one or more child elements.</span></span>
  
<span data-ttu-id="88643-124">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="88643-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="88643-125">Embora os elementos filho adicionais são válidos pelo esquema, o [CalendarItem](calendaritem.md) é o elemento filho somente que retornará os serviços Web do Exchange (EWS) dentro do elemento **ConflictingMeetings** .</span><span class="sxs-lookup"><span data-stu-id="88643-125">Although additional child elements are valid per the schema, the [CalendarItem](calendaritem.md) element is the only child element that Exchange Web Services (EWS) will return within the **ConflictingMeetings** element.</span></span> <span data-ttu-id="88643-126">Este tópico não lista os elementos filhos que são válidas pelo esquema, mas não serão retornados por EWS.</span><span class="sxs-lookup"><span data-stu-id="88643-126">This topic does not list child elements that are valid per the schema but will not be returned by EWS.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="88643-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="88643-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88643-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="88643-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="88643-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="88643-129">Schema Name</span></span>  <br/> |<span data-ttu-id="88643-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="88643-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="88643-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="88643-131">Validation File</span></span>  <br/> |<span data-ttu-id="88643-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="88643-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="88643-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="88643-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="88643-134">False</span><span class="sxs-lookup"><span data-stu-id="88643-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88643-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="88643-135">See also</span></span>



- [<span data-ttu-id="88643-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="88643-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

