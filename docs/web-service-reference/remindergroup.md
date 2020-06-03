---
title: Um dos lembretes
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3e23c2a1-05d8-4fec-897c-f684a5b97e4c
description: O elemento de enlembrete especifica se o lembrete é para um item de calendário ou uma tarefa.
ms.openlocfilehash: be6f4a7d7e9d495ed7b42ed40c60f016468e8c2c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529865"
---
# <a name="remindergroup"></a><span data-ttu-id="23669-103">Um dos lembretes</span><span class="sxs-lookup"><span data-stu-id="23669-103">ReminderGroup</span></span>

<span data-ttu-id="23669-104">O elemento de **Enlembrete** especifica se o lembrete é para um item de calendário ou uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="23669-104">The **ReminderGroup** element specifies whether the reminder is for a calendar item or a task.</span></span> 
  
```XML
<ReminderGroup> Calendar | Task </ReminderGroup>
```

 <span data-ttu-id="23669-105">**ReminderGroupType**</span><span class="sxs-lookup"><span data-stu-id="23669-105">**ReminderGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="23669-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="23669-106">Attributes and elements</span></span>

<span data-ttu-id="23669-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="23669-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23669-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="23669-108">Attributes</span></span>

<span data-ttu-id="23669-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23669-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23669-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="23669-110">Child elements</span></span>

<span data-ttu-id="23669-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="23669-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="23669-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="23669-112">Parent elements</span></span>

[<span data-ttu-id="23669-113">Lembrete</span><span class="sxs-lookup"><span data-stu-id="23669-113">Reminder</span></span>](reminder.md)
  
## <a name="text-value"></a><span data-ttu-id="23669-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="23669-114">Text value</span></span>

<span data-ttu-id="23669-115">O valor de texto do elemento de grupo de **lembretes** é o tipo do lembrete.</span><span class="sxs-lookup"><span data-stu-id="23669-115">The text value of the **ReminderGroup** element is the group type of the reminder.</span></span> <span data-ttu-id="23669-116">O valor de texto do **calendário** especifica que o lembrete é para um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="23669-116">The text value of **Calendar** specifies that the reminder is for a calendar item.</span></span> <span data-ttu-id="23669-117">O valor de texto da **tarefa** especifica que o lembrete é para um item de tarefa.</span><span class="sxs-lookup"><span data-stu-id="23669-117">The text value of **Task** specifies that the reminder is for a task item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="23669-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="23669-118">Remarks</span></span>

<span data-ttu-id="23669-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="23669-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="23669-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="23669-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23669-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="23669-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23669-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="23669-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="23669-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="23669-123">Schema Name</span></span>  <br/> |<span data-ttu-id="23669-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="23669-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="23669-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="23669-125">Validation File</span></span>  <br/> |<span data-ttu-id="23669-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="23669-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="23669-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="23669-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="23669-128">False</span><span class="sxs-lookup"><span data-stu-id="23669-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="23669-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="23669-129">See also</span></span>



[<span data-ttu-id="23669-130">Lembrete</span><span class="sxs-lookup"><span data-stu-id="23669-130">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="23669-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="23669-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

