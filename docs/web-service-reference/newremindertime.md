---
title: NewReminderTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: O elemento NewReminderTime especifica um novo horário para um lembrete.
ms.openlocfilehash: a10f7e481b474501f33dba4c09060766568952b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465951"
---
# <a name="newremindertime"></a><span data-ttu-id="e5e31-103">NewReminderTime</span><span class="sxs-lookup"><span data-stu-id="e5e31-103">NewReminderTime</span></span>

<span data-ttu-id="e5e31-104">O elemento **NewReminderTime** especifica um novo horário para um lembrete.</span><span class="sxs-lookup"><span data-stu-id="e5e31-104">The **NewReminderTime** element specifies a new time for a reminder.</span></span> 
  
```XML
<NewReminderTime/>
```

 <span data-ttu-id="e5e31-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="e5e31-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e5e31-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e5e31-106">Attributes and elements</span></span>

<span data-ttu-id="e5e31-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e5e31-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5e31-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e5e31-108">Attributes</span></span>

<span data-ttu-id="e5e31-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5e31-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e5e31-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e5e31-110">Child elements</span></span>

<span data-ttu-id="e5e31-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e5e31-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e5e31-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e5e31-112">Parent elements</span></span>

[<span data-ttu-id="e5e31-113">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="e5e31-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="e5e31-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e5e31-114">Text value</span></span>

<span data-ttu-id="e5e31-115">O valor de texto do elemento **NewReminderTime** é uma nova hora para o lembrete.</span><span class="sxs-lookup"><span data-stu-id="e5e31-115">The text value of the **NewReminderTime** element is a new time for the reminder.</span></span> <span data-ttu-id="e5e31-116">O elemento **NewReminderTime** é usado quando o elemento [ActionType](actiontype-reminderactiontype.md) é definido como **adiar**, a fim de atrasar o lembrete.</span><span class="sxs-lookup"><span data-stu-id="e5e31-116">The **NewReminderTime** element is used when the [ActionType](actiontype-reminderactiontype.md) element is set to **Snooze**, in order to delay the reminder.</span></span> <span data-ttu-id="e5e31-117">O valor de **NewReminderTime** deve ser maior do que o [ReminderTime](remindertime.md) retornado pela [operação getlembrers](getreminders-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e5e31-117">The value of the **NewReminderTime** must be greater than the [ReminderTime](remindertime.md) returned by the [GetReminders operation](getreminders-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e5e31-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="e5e31-118">Remarks</span></span>

<span data-ttu-id="e5e31-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e5e31-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e5e31-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e5e31-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e5e31-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e5e31-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e5e31-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="e5e31-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e5e31-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e5e31-123">Schema Name</span></span>  <br/> |<span data-ttu-id="e5e31-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e5e31-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="e5e31-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e5e31-125">Validation File</span></span>  <br/> |<span data-ttu-id="e5e31-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e5e31-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e5e31-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e5e31-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="e5e31-128">False</span><span class="sxs-lookup"><span data-stu-id="e5e31-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e5e31-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="e5e31-129">See also</span></span>



[<span data-ttu-id="e5e31-130">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="e5e31-130">ReminderItemAction</span></span>](reminderitemaction.md)


- [<span data-ttu-id="e5e31-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e5e31-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

