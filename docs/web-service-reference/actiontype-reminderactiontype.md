---
title: ActionType (ReminderActionType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0ffcdcf4-8ea3-483c-bb7f-0cd84126120c
description: O elemento ActionType Especifica a ação a ser executada no lembrete.
ms.openlocfilehash: 361259f733756995fae2c2c2390013a728e475a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751037"
---
# <a name="actiontype-reminderactiontype"></a><span data-ttu-id="c9f91-103">ActionType (ReminderActionType)</span><span class="sxs-lookup"><span data-stu-id="c9f91-103">ActionType (ReminderActionType)</span></span>

<span data-ttu-id="c9f91-104">O elemento **ActionType** Especifica a ação a ser executada no lembrete.</span><span class="sxs-lookup"><span data-stu-id="c9f91-104">The **ActionType** element specifies the action to take on the reminder.</span></span> 
  
```XML
<ActionType> Dismiss | Snooze </ActionType>
```

 <span data-ttu-id="c9f91-105">**ReminderActionType**</span><span class="sxs-lookup"><span data-stu-id="c9f91-105">**ReminderActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9f91-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c9f91-106">Attributes and elements</span></span>

<span data-ttu-id="c9f91-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c9f91-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9f91-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c9f91-108">Attributes</span></span>

<span data-ttu-id="c9f91-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c9f91-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9f91-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c9f91-110">Child elements</span></span>

<span data-ttu-id="c9f91-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c9f91-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c9f91-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c9f91-112">Parent elements</span></span>

[<span data-ttu-id="c9f91-113">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="c9f91-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="c9f91-114">Text value</span><span class="sxs-lookup"><span data-stu-id="c9f91-114">Text value</span></span>

<span data-ttu-id="c9f91-115">O valor de texto do elemento **ActionType** Especifica a ação a ser executada no lembrete.</span><span class="sxs-lookup"><span data-stu-id="c9f91-115">The text value of the **ActionType** element specifies the action to take on the reminder.</span></span> <span data-ttu-id="c9f91-116">O valor de texto da **Dismiss** indica que o lembrete deve ser descartado.</span><span class="sxs-lookup"><span data-stu-id="c9f91-116">The text value of **Dismiss** indicates the reminder should be dismissed.</span></span> <span data-ttu-id="c9f91-117">O valor de texto da **Snooze** indica que o lembrete deve ser atrasado até o tempo especificado pelo elemento [NewReminderTime](newremindertime.md) .</span><span class="sxs-lookup"><span data-stu-id="c9f91-117">The text value of **Snooze** indicates that the reminder should be delayed until the time specified by the [NewReminderTime](newremindertime.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c9f91-118">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="c9f91-118">Remarks</span></span>

<span data-ttu-id="c9f91-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c9f91-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c9f91-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9f91-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9f91-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c9f91-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9f91-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="c9f91-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c9f91-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c9f91-123">Schema Name</span></span>  <br/> |<span data-ttu-id="c9f91-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c9f91-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="c9f91-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c9f91-125">Validation File</span></span>  <br/> |<span data-ttu-id="c9f91-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c9f91-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c9f91-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c9f91-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9f91-128">False</span><span class="sxs-lookup"><span data-stu-id="c9f91-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9f91-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="c9f91-129">See also</span></span>

- [<span data-ttu-id="c9f91-130">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="c9f91-130">ReminderItemAction</span></span>](reminderitemaction.md)
- [<span data-ttu-id="c9f91-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c9f91-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

