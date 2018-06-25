---
title: ReminderGroup
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3e23c2a1-05d8-4fec-897c-f684a5b97e4c
description: O elemento ReminderGroup Especifica se o lembrete for para um item de calendário ou uma tarefa.
ms.openlocfilehash: d9d31cdab482d04149428021ad44cc742108053a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825060"
---
# <a name="remindergroup"></a><span data-ttu-id="91643-103">ReminderGroup</span><span class="sxs-lookup"><span data-stu-id="91643-103">ReminderGroup</span></span>

<span data-ttu-id="91643-104">O elemento **ReminderGroup** Especifica se o lembrete for para um item de calendário ou uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="91643-104">The **ReminderGroup** element specifies whether the reminder is for a calendar item or a task.</span></span> 
  
```XML
<ReminderGroup> Calendar | Task </ReminderGroup>
```

 <span data-ttu-id="91643-105">**ReminderGroupType**</span><span class="sxs-lookup"><span data-stu-id="91643-105">**ReminderGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91643-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="91643-106">Attributes and elements</span></span>

<span data-ttu-id="91643-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="91643-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91643-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="91643-108">Attributes</span></span>

<span data-ttu-id="91643-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="91643-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91643-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="91643-110">Child elements</span></span>

<span data-ttu-id="91643-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="91643-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91643-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="91643-112">Parent elements</span></span>

[<span data-ttu-id="91643-113">Lembrete</span><span class="sxs-lookup"><span data-stu-id="91643-113">Reminder</span></span>](reminder.md)
  
## <a name="text-value"></a><span data-ttu-id="91643-114">Text value</span><span class="sxs-lookup"><span data-stu-id="91643-114">Text value</span></span>

<span data-ttu-id="91643-115">O valor de texto do elemento **ReminderGroup** é o tipo de grupo do lembrete.</span><span class="sxs-lookup"><span data-stu-id="91643-115">The text value of the **ReminderGroup** element is the group type of the reminder.</span></span> <span data-ttu-id="91643-116">O valor do **calendário** texto Especifica que o lembrete for para um item do calendário.</span><span class="sxs-lookup"><span data-stu-id="91643-116">The text value of **Calendar** specifies that the reminder is for a calendar item.</span></span> <span data-ttu-id="91643-117">O valor de texto da **tarefa** Especifica que o lembrete for para um item de tarefa.</span><span class="sxs-lookup"><span data-stu-id="91643-117">The text value of **Task** specifies that the reminder is for a task item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="91643-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="91643-118">Remarks</span></span>

<span data-ttu-id="91643-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="91643-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="91643-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="91643-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91643-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="91643-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91643-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="91643-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91643-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="91643-123">Schema Name</span></span>  <br/> |<span data-ttu-id="91643-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="91643-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="91643-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="91643-125">Validation File</span></span>  <br/> |<span data-ttu-id="91643-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="91643-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="91643-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="91643-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="91643-128">False</span><span class="sxs-lookup"><span data-stu-id="91643-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="91643-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="91643-129">See also</span></span>



[<span data-ttu-id="91643-130">Lembrete</span><span class="sxs-lookup"><span data-stu-id="91643-130">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="91643-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="91643-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

