---
title: NewReminderTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: O elemento NewReminderTime Especifica um novo horário para um lembrete.
ms.openlocfilehash: 9f3f509942c673c916cc646cd9519240aef6ea06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824531"
---
# <a name="newremindertime"></a><span data-ttu-id="53e18-103">NewReminderTime</span><span class="sxs-lookup"><span data-stu-id="53e18-103">NewReminderTime</span></span>

<span data-ttu-id="53e18-104">O elemento **NewReminderTime** Especifica um novo horário para um lembrete.</span><span class="sxs-lookup"><span data-stu-id="53e18-104">The **NewReminderTime** element specifies a new time for a reminder.</span></span> 
  
```XML
<NewReminderTime/>
```

 <span data-ttu-id="53e18-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="53e18-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="53e18-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="53e18-106">Attributes and elements</span></span>

<span data-ttu-id="53e18-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="53e18-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="53e18-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="53e18-108">Attributes</span></span>

<span data-ttu-id="53e18-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="53e18-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="53e18-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="53e18-110">Child elements</span></span>

<span data-ttu-id="53e18-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="53e18-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="53e18-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="53e18-112">Parent elements</span></span>

[<span data-ttu-id="53e18-113">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="53e18-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="53e18-114">Text value</span><span class="sxs-lookup"><span data-stu-id="53e18-114">Text value</span></span>

<span data-ttu-id="53e18-115">O valor de texto do elemento **NewReminderTime** é um novo horário para o lembrete.</span><span class="sxs-lookup"><span data-stu-id="53e18-115">The text value of the **NewReminderTime** element is a new time for the reminder.</span></span> <span data-ttu-id="53e18-116">O elemento **NewReminderTime** é usado quando o elemento [ActionType](actiontype-reminderactiontype.md) é definir como **Snooze**, a fim de atraso do lembrete.</span><span class="sxs-lookup"><span data-stu-id="53e18-116">The **NewReminderTime** element is used when the [ActionType](actiontype-reminderactiontype.md) element is set to **Snooze**, in order to delay the reminder.</span></span> <span data-ttu-id="53e18-117">O valor de **NewReminderTime** deve ser maior que o [ReminderTime](remindertime.md) retornado pela [operação de GetReminders](getreminders-operation.md).</span><span class="sxs-lookup"><span data-stu-id="53e18-117">The value of the **NewReminderTime** must be greater than the [ReminderTime](remindertime.md) returned by the [GetReminders operation](getreminders-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="53e18-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="53e18-118">Remarks</span></span>

<span data-ttu-id="53e18-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="53e18-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="53e18-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="53e18-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="53e18-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="53e18-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="53e18-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="53e18-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="53e18-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="53e18-123">Schema Name</span></span>  <br/> |<span data-ttu-id="53e18-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="53e18-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="53e18-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="53e18-125">Validation File</span></span>  <br/> |<span data-ttu-id="53e18-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="53e18-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="53e18-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="53e18-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="53e18-128">False</span><span class="sxs-lookup"><span data-stu-id="53e18-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="53e18-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="53e18-129">See also</span></span>



[<span data-ttu-id="53e18-130">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="53e18-130">ReminderItemAction</span></span>](reminderitemaction.md)


- [<span data-ttu-id="53e18-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="53e18-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

