---
title: IsAllDayEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAllDayEvent
api_type:
- schema
ms.assetid: 29140a64-9d7a-4a14-a10d-c98197c9831b
description: O elemento IsAllDayEvent indica se um item de calendário ou uma solicitação de reunião representa um evento de dia inteiro.
ms.openlocfilehash: f0c975deecf96e94599a47ef2c33e54a7d1a80b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526533"
---
# <a name="isalldayevent"></a><span data-ttu-id="2f507-103">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="2f507-103">IsAllDayEvent</span></span>

<span data-ttu-id="2f507-104">O elemento **IsAllDayEvent** indica se um item de calendário ou uma solicitação de reunião representa um evento de dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="2f507-104">The **IsAllDayEvent** element indicates whether a calendar item or meeting request represents an all-day event.</span></span> 
  
```xml
<IsAllDayEvent/>
```

 <span data-ttu-id="2f507-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2f507-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2f507-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2f507-106">Attributes and elements</span></span>

<span data-ttu-id="2f507-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2f507-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f507-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2f507-108">Attributes</span></span>

<span data-ttu-id="2f507-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2f507-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2f507-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2f507-110">Child elements</span></span>

<span data-ttu-id="2f507-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2f507-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2f507-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2f507-112">Parent elements</span></span>

|<span data-ttu-id="2f507-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2f507-113">**Element**</span></span>|<span data-ttu-id="2f507-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2f507-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f507-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="2f507-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2f507-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f507-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2f507-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="2f507-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2f507-118">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f507-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2f507-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="2f507-119">Text value</span></span>

<span data-ttu-id="2f507-120">Um valor de texto que representa um valor booliano é necessário se esse elemento for incluído.</span><span class="sxs-lookup"><span data-stu-id="2f507-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="2f507-121">Um valor **true** indica que o item representa um evento de dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="2f507-121">A value of **true** indicates that the item represents an all-day event.</span></span> <span data-ttu-id="2f507-122">Um valor **false** indica que o item abrange menos do que o horário de trabalho de um usuário.</span><span class="sxs-lookup"><span data-stu-id="2f507-122">A value of **false** indicates that the item spans less than a user's working hours.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2f507-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="2f507-123">Remarks</span></span>

<span data-ttu-id="2f507-124">Um evento de dia inteiro abrange a duração de horas de trabalho que são definidas para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2f507-124">An all-day event spans the duration of working hours that is defined for a mailbox.</span></span>
  
<span data-ttu-id="2f507-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="2f507-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f507-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2f507-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f507-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="2f507-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2f507-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2f507-128">Schema name</span></span>  <br/> |<span data-ttu-id="2f507-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2f507-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="2f507-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2f507-130">Validation file</span></span>  <br/> |<span data-ttu-id="2f507-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2f507-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2f507-132">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2f507-132">Can be empty</span></span>  <br/> |<span data-ttu-id="2f507-133">False</span><span class="sxs-lookup"><span data-stu-id="2f507-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2f507-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="2f507-134">See also</span></span>



- [<span data-ttu-id="2f507-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2f507-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

