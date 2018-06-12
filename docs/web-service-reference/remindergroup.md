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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825060"
---
# <a name="remindergroup"></a><span data-ttu-id="d8133-103">ReminderGroup</span><span class="sxs-lookup"><span data-stu-id="d8133-103">ReminderGroup</span></span>

<span data-ttu-id="d8133-104">O elemento **ReminderGroup** Especifica se o lembrete for para um item de calendário ou uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="d8133-104">The **ReminderGroup** element specifies whether the reminder is for a calendar item or a task.</span></span> 
  
```XML
<ReminderGroup> Calendar | Task </ReminderGroup>
```

 <span data-ttu-id="d8133-105">**ReminderGroupType**</span><span class="sxs-lookup"><span data-stu-id="d8133-105">**ReminderGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8133-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d8133-106">Attributes and elements</span></span>

<span data-ttu-id="d8133-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d8133-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8133-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d8133-108">Attributes</span></span>

<span data-ttu-id="d8133-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d8133-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8133-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d8133-110">Child elements</span></span>

<span data-ttu-id="d8133-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d8133-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d8133-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d8133-112">Parent elements</span></span>

[<span data-ttu-id="d8133-113">Lembrete</span><span class="sxs-lookup"><span data-stu-id="d8133-113">Reminder</span></span>](reminder.md)
  
## <a name="text-value"></a><span data-ttu-id="d8133-114">Text value</span><span class="sxs-lookup"><span data-stu-id="d8133-114">Text value</span></span>

<span data-ttu-id="d8133-115">O valor de texto do elemento **ReminderGroup** é o tipo de grupo do lembrete.</span><span class="sxs-lookup"><span data-stu-id="d8133-115">The text value of the **ReminderGroup** element is the group type of the reminder.</span></span> <span data-ttu-id="d8133-116">O valor do **calendário** texto Especifica que o lembrete for para um item do calendário.</span><span class="sxs-lookup"><span data-stu-id="d8133-116">The text value of **Calendar** specifies that the reminder is for a calendar item.</span></span> <span data-ttu-id="d8133-117">O valor de texto da **tarefa** Especifica que o lembrete for para um item de tarefa.</span><span class="sxs-lookup"><span data-stu-id="d8133-117">The text value of **Task** specifies that the reminder is for a task item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d8133-118">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="d8133-118">Remarks</span></span>

<span data-ttu-id="d8133-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d8133-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d8133-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8133-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8133-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d8133-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8133-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="d8133-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8133-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d8133-123">Schema Name</span></span>  <br/> |<span data-ttu-id="d8133-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d8133-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="d8133-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d8133-125">Validation File</span></span>  <br/> |<span data-ttu-id="d8133-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d8133-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8133-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d8133-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="d8133-128">False</span><span class="sxs-lookup"><span data-stu-id="d8133-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8133-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="d8133-129">See also</span></span>



[<span data-ttu-id="d8133-130">Lembrete</span><span class="sxs-lookup"><span data-stu-id="d8133-130">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="d8133-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d8133-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

