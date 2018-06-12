---
title: IsMeeting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeeting
api_type:
- schema
ms.assetid: 6ce22f17-7a31-46c4-b643-0894d087e852
description: O elemento IsMeeting indica se o item do calendário é uma reunião ou um compromisso.
ms.openlocfilehash: bb1349a8690450882e6beac0ccd84a8d03272a7d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824051"
---
# <a name="ismeeting"></a><span data-ttu-id="f10b4-103">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="f10b4-103">IsMeeting</span></span>

<span data-ttu-id="f10b4-104">O elemento **IsMeeting** indica se o item do calendário é uma reunião ou um compromisso.</span><span class="sxs-lookup"><span data-stu-id="f10b4-104">The **IsMeeting** element indicates whether the calendar item is a meeting or an appointment.</span></span> 
  
```xml
<IsMeeting/>
```

 <span data-ttu-id="f10b4-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f10b4-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f10b4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f10b4-106">Attributes and elements</span></span>

<span data-ttu-id="f10b4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f10b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f10b4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f10b4-108">Attributes</span></span>

<span data-ttu-id="f10b4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f10b4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f10b4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f10b4-110">Child elements</span></span>

<span data-ttu-id="f10b4-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f10b4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f10b4-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f10b4-112">Parent elements</span></span>

|<span data-ttu-id="f10b4-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f10b4-113">**Element**</span></span>|<span data-ttu-id="f10b4-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f10b4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f10b4-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="f10b4-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="f10b4-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f10b4-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f10b4-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="f10b4-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f10b4-118">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f10b4-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f10b4-119">Text value</span><span class="sxs-lookup"><span data-stu-id="f10b4-119">Text value</span></span>

<span data-ttu-id="f10b4-120">Um valor de texto que representa um valor booleano é necessário se este elemento é incluído.</span><span class="sxs-lookup"><span data-stu-id="f10b4-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="f10b4-121">Um valor **true** indica que o item de calendário é uma reunião.</span><span class="sxs-lookup"><span data-stu-id="f10b4-121">A value of **true** indicates that the calendar item is a meeting.</span></span> <span data-ttu-id="f10b4-122">Um valor **false** indica que o item de calendário é um compromisso.</span><span class="sxs-lookup"><span data-stu-id="f10b4-122">A value of **false** indicates that the calendar item is an appointment.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f10b4-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="f10b4-123">Remarks</span></span>

<span data-ttu-id="f10b4-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="f10b4-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f10b4-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f10b4-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f10b4-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="f10b4-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f10b4-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f10b4-127">Schema name</span></span>  <br/> |<span data-ttu-id="f10b4-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f10b4-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="f10b4-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f10b4-129">Validation file</span></span>  <br/> |<span data-ttu-id="f10b4-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f10b4-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f10b4-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f10b4-131">Can be empty</span></span>  <br/> |<span data-ttu-id="f10b4-132">False</span><span class="sxs-lookup"><span data-stu-id="f10b4-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f10b4-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="f10b4-133">See also</span></span>



- [<span data-ttu-id="f10b4-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f10b4-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

