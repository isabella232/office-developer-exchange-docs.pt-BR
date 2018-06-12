---
title: Recursos
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Resources
api_type:
- schema
ms.assetid: a2133cf2-7c62-4f1c-b3aa-75f14d30dd74
description: O elemento de recursos representa um recurso agendado para uma reunião.
ms.openlocfilehash: 31f358414e53f55b983f7633fc9c67b0ce3ab645
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825166"
---
# <a name="resources"></a><span data-ttu-id="22f36-103">Recursos</span><span class="sxs-lookup"><span data-stu-id="22f36-103">Resources</span></span>

<span data-ttu-id="22f36-104">O elemento de **recursos** representa um recurso agendado para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="22f36-104">The **Resources** element represents a scheduled resource for a meeting.</span></span> 
  
```xml
<Resources>
   <Attendee/>
</Resources>
```

 <span data-ttu-id="22f36-105">**NonEmptyArrayOfAttendeesType**</span><span class="sxs-lookup"><span data-stu-id="22f36-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22f36-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="22f36-106">Attributes and elements</span></span>

<span data-ttu-id="22f36-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="22f36-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22f36-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="22f36-108">Attributes</span></span>

<span data-ttu-id="22f36-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="22f36-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22f36-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="22f36-110">Child elements</span></span>

|<span data-ttu-id="22f36-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="22f36-111">**Element**</span></span>|<span data-ttu-id="22f36-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="22f36-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22f36-113">Attendee</span><span class="sxs-lookup"><span data-stu-id="22f36-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="22f36-114">Representa os participantes e recursos para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="22f36-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="22f36-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="22f36-115">Parent elements</span></span>

|<span data-ttu-id="22f36-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="22f36-116">**Element**</span></span>|<span data-ttu-id="22f36-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="22f36-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22f36-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="22f36-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="22f36-119">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="22f36-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="22f36-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="22f36-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="22f36-121">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="22f36-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="22f36-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="22f36-122">Remarks</span></span>

<span data-ttu-id="22f36-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="22f36-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22f36-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="22f36-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22f36-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="22f36-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="22f36-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="22f36-126">Schema name</span></span>  <br/> |<span data-ttu-id="22f36-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="22f36-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="22f36-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="22f36-128">Validation file</span></span>  <br/> |<span data-ttu-id="22f36-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="22f36-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="22f36-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="22f36-130">Can be empty</span></span>  <br/> |<span data-ttu-id="22f36-131">False</span><span class="sxs-lookup"><span data-stu-id="22f36-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22f36-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="22f36-132">See also</span></span>



- [<span data-ttu-id="22f36-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="22f36-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

