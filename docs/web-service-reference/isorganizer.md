---
title: IsOrganizer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a31ac268-5061-4272-a433-ffaea2fbcfa9
description: O elemento IsOrganizer Especifica um valor Boolean que indica se essa pessoa é o organizador da reunião.
ms.openlocfilehash: 5fd775cfc0a296c08d19d0468d96aa36ba67ddd0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824063"
---
# <a name="isorganizer"></a><span data-ttu-id="f1d53-103">IsOrganizer</span><span class="sxs-lookup"><span data-stu-id="f1d53-103">IsOrganizer</span></span>

<span data-ttu-id="f1d53-104">O elemento **IsOrganizer** Especifica um valor Boolean que indica se essa pessoa é o organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="f1d53-104">The **IsOrganizer** element specifies a Boolean value that indicates whether this person is the organizer of the meeting.</span></span> 
  
```XML
<IsOrganizer>true | false</IsOrganizer>
```

 <span data-ttu-id="f1d53-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f1d53-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1d53-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f1d53-106">Attributes and elements</span></span>

<span data-ttu-id="f1d53-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f1d53-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1d53-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f1d53-108">Attributes</span></span>

<span data-ttu-id="f1d53-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f1d53-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1d53-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f1d53-110">Child elements</span></span>

<span data-ttu-id="f1d53-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f1d53-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f1d53-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f1d53-112">Parent elements</span></span>

|<span data-ttu-id="f1d53-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f1d53-113">**Element**</span></span>|<span data-ttu-id="f1d53-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f1d53-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1d53-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="f1d53-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="f1d53-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1d53-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f1d53-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="f1d53-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="f1d53-118">Representa uma mensagem de reunião.</span><span class="sxs-lookup"><span data-stu-id="f1d53-118">Represents a meeting message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f1d53-119">Text value</span><span class="sxs-lookup"><span data-stu-id="f1d53-119">Text value</span></span>

<span data-ttu-id="f1d53-120">Um valor de **true** para o elemento **IsOrganizer** text indica se a mensagem de reunião ou de item de calendário foi criada pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="f1d53-120">A text value of **true** for the **IsOrganizer** element indicates that the calendar item or meeting message was created by the user.</span></span> <span data-ttu-id="f1d53-121">Um valor **false** indica que a mensagem de reunião ou de item de calendário não foi criada bv o usuário.</span><span class="sxs-lookup"><span data-stu-id="f1d53-121">A value of **false** indicates that the calendar item or meeting message was not created bv the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f1d53-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="f1d53-122">Remarks</span></span>

<span data-ttu-id="f1d53-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f1d53-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f1d53-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1d53-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1d53-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f1d53-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1d53-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="f1d53-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f1d53-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f1d53-127">Schema Name</span></span>  <br/> |<span data-ttu-id="f1d53-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="f1d53-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="f1d53-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f1d53-129">Validation File</span></span>  <br/> |<span data-ttu-id="f1d53-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f1d53-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f1d53-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f1d53-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f1d53-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="f1d53-132">See also</span></span>



- [<span data-ttu-id="f1d53-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f1d53-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

