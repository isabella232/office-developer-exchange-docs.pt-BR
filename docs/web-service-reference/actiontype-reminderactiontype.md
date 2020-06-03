---
title: ActionType (ReminderActionType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0ffcdcf4-8ea3-483c-bb7f-0cd84126120c
description: O elemento ActionType especifica a ação a ser tomada no lembrete.
ms.openlocfilehash: 5c62b2dd945b23a5ff2bb824385c45dbc617a5a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465055"
---
# <a name="actiontype-reminderactiontype"></a><span data-ttu-id="8072b-103">ActionType (ReminderActionType)</span><span class="sxs-lookup"><span data-stu-id="8072b-103">ActionType (ReminderActionType)</span></span>

<span data-ttu-id="8072b-104">O elemento **ActionType** especifica a ação a ser tomada no lembrete.</span><span class="sxs-lookup"><span data-stu-id="8072b-104">The **ActionType** element specifies the action to take on the reminder.</span></span> 
  
```XML
<ActionType> Dismiss | Snooze </ActionType>
```

 <span data-ttu-id="8072b-105">**ReminderActionType**</span><span class="sxs-lookup"><span data-stu-id="8072b-105">**ReminderActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8072b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8072b-106">Attributes and elements</span></span>

<span data-ttu-id="8072b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8072b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8072b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8072b-108">Attributes</span></span>

<span data-ttu-id="8072b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8072b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8072b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8072b-110">Child elements</span></span>

<span data-ttu-id="8072b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8072b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8072b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8072b-112">Parent elements</span></span>

[<span data-ttu-id="8072b-113">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="8072b-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="8072b-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8072b-114">Text value</span></span>

<span data-ttu-id="8072b-115">O valor de texto do elemento **ActionType** especifica a ação a ser tomada no lembrete.</span><span class="sxs-lookup"><span data-stu-id="8072b-115">The text value of the **ActionType** element specifies the action to take on the reminder.</span></span> <span data-ttu-id="8072b-116">O valor de texto de **ignorar** indica que o lembrete deve ser Descartado.</span><span class="sxs-lookup"><span data-stu-id="8072b-116">The text value of **Dismiss** indicates the reminder should be dismissed.</span></span> <span data-ttu-id="8072b-117">O valor de texto de **adiar** indica que o lembrete deve ser atrasado até o tempo especificado pelo elemento [NewReminderTime](newremindertime.md) .</span><span class="sxs-lookup"><span data-stu-id="8072b-117">The text value of **Snooze** indicates that the reminder should be delayed until the time specified by the [NewReminderTime](newremindertime.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8072b-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="8072b-118">Remarks</span></span>

<span data-ttu-id="8072b-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8072b-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8072b-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8072b-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8072b-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8072b-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8072b-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="8072b-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8072b-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8072b-123">Schema Name</span></span>  <br/> |<span data-ttu-id="8072b-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8072b-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="8072b-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8072b-125">Validation File</span></span>  <br/> |<span data-ttu-id="8072b-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8072b-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8072b-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8072b-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="8072b-128">False</span><span class="sxs-lookup"><span data-stu-id="8072b-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8072b-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="8072b-129">See also</span></span>

- [<span data-ttu-id="8072b-130">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="8072b-130">ReminderItemAction</span></span>](reminderitemaction.md)
- [<span data-ttu-id="8072b-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8072b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

