---
title: Isorganizer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a31ac268-5061-4272-a433-ffaea2fbcfa9
description: O elemento isorganizer especifica um valor Boolean que indica se essa pessoa é o organizador da reunião.
ms.openlocfilehash: 45b7a66068dc00f6e60b7380240bea6836282fd4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466560"
---
# <a name="isorganizer"></a><span data-ttu-id="961e9-103">Isorganizer</span><span class="sxs-lookup"><span data-stu-id="961e9-103">IsOrganizer</span></span>

<span data-ttu-id="961e9-104">O elemento **Isorganizer** especifica um valor Boolean que indica se essa pessoa é o organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="961e9-104">The **IsOrganizer** element specifies a Boolean value that indicates whether this person is the organizer of the meeting.</span></span> 
  
```XML
<IsOrganizer>true | false</IsOrganizer>
```

 <span data-ttu-id="961e9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="961e9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="961e9-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="961e9-106">Attributes and elements</span></span>

<span data-ttu-id="961e9-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="961e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="961e9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="961e9-108">Attributes</span></span>

<span data-ttu-id="961e9-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="961e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="961e9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="961e9-110">Child elements</span></span>

<span data-ttu-id="961e9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="961e9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="961e9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="961e9-112">Parent elements</span></span>

|<span data-ttu-id="961e9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="961e9-113">**Element**</span></span>|<span data-ttu-id="961e9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="961e9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="961e9-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="961e9-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="961e9-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="961e9-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="961e9-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="961e9-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="961e9-118">Representa uma mensagem de reunião.</span><span class="sxs-lookup"><span data-stu-id="961e9-118">Represents a meeting message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="961e9-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="961e9-119">Text value</span></span>

<span data-ttu-id="961e9-120">Um valor de texto **true** para o elemento **isorganizer** indica que o item de calendário ou a mensagem de reunião foi criado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="961e9-120">A text value of **true** for the **IsOrganizer** element indicates that the calendar item or meeting message was created by the user.</span></span> <span data-ttu-id="961e9-121">Um valor **false** indica que o item de calendário ou a mensagem de reunião não foi criado BV o usuário.</span><span class="sxs-lookup"><span data-stu-id="961e9-121">A value of **false** indicates that the calendar item or meeting message was not created bv the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="961e9-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="961e9-122">Remarks</span></span>

<span data-ttu-id="961e9-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="961e9-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="961e9-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="961e9-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="961e9-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="961e9-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="961e9-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="961e9-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="961e9-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="961e9-127">Schema Name</span></span>  <br/> |<span data-ttu-id="961e9-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="961e9-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="961e9-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="961e9-129">Validation File</span></span>  <br/> |<span data-ttu-id="961e9-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="961e9-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="961e9-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="961e9-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="961e9-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="961e9-132">See also</span></span>



- [<span data-ttu-id="961e9-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="961e9-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

