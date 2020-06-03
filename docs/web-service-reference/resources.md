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
description: O elemento resources representa um recurso agendado para uma reunião.
ms.openlocfilehash: 67b4ed93a67a48945845887aa2d08b5bfe0102d4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455587"
---
# <a name="resources"></a><span data-ttu-id="cb2ed-103">Recursos</span><span class="sxs-lookup"><span data-stu-id="cb2ed-103">Resources</span></span>

<span data-ttu-id="cb2ed-104">O elemento **Resources** representa um recurso agendado para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="cb2ed-104">The **Resources** element represents a scheduled resource for a meeting.</span></span> 
  
```xml
<Resources>
   <Attendee/>
</Resources>
```

 <span data-ttu-id="cb2ed-105">**NonEmptyArrayOfAttendeesType**</span><span class="sxs-lookup"><span data-stu-id="cb2ed-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cb2ed-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cb2ed-106">Attributes and elements</span></span>

<span data-ttu-id="cb2ed-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cb2ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb2ed-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cb2ed-108">Attributes</span></span>

<span data-ttu-id="cb2ed-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb2ed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cb2ed-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cb2ed-110">Child elements</span></span>

|<span data-ttu-id="cb2ed-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cb2ed-111">**Element**</span></span>|<span data-ttu-id="cb2ed-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cb2ed-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb2ed-113">Participante</span><span class="sxs-lookup"><span data-stu-id="cb2ed-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="cb2ed-114">Representa participantes e recursos de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="cb2ed-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cb2ed-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cb2ed-115">Parent elements</span></span>

|<span data-ttu-id="cb2ed-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cb2ed-116">**Element**</span></span>|<span data-ttu-id="cb2ed-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cb2ed-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb2ed-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="cb2ed-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="cb2ed-119">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb2ed-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="cb2ed-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="cb2ed-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="cb2ed-121">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb2ed-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cb2ed-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="cb2ed-122">Remarks</span></span>

<span data-ttu-id="cb2ed-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="cb2ed-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cb2ed-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cb2ed-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cb2ed-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="cb2ed-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cb2ed-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cb2ed-126">Schema name</span></span>  <br/> |<span data-ttu-id="cb2ed-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="cb2ed-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="cb2ed-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cb2ed-128">Validation file</span></span>  <br/> |<span data-ttu-id="cb2ed-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cb2ed-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cb2ed-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="cb2ed-130">Can be empty</span></span>  <br/> |<span data-ttu-id="cb2ed-131">False</span><span class="sxs-lookup"><span data-stu-id="cb2ed-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cb2ed-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="cb2ed-132">See also</span></span>



- [<span data-ttu-id="cb2ed-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cb2ed-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

