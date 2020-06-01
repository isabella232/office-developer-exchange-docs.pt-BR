---
title: Reminder
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54dd748a-23a5-4ea2-88f2-b74c68a3c48f
description: O elemento Reminder especifica um lembrete para uma tarefa ou um item de calendário.
ms.openlocfilehash: 71e54d920a169b8060d22bb7d7d294208c344c2e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457484"
---
# <a name="reminder"></a><span data-ttu-id="147f2-103">Reminder</span><span class="sxs-lookup"><span data-stu-id="147f2-103">Reminder</span></span>

<span data-ttu-id="147f2-104">O elemento **Reminder** especifica um lembrete para uma tarefa ou um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="147f2-104">The **Reminder** element specifies a reminder for a task or a calendar item.</span></span> 
  
```XML
<Reminder>
   <Subject></Subject>
   <Location></Location>
   <ReminderTime></ReminderTime>
   <StartDate></StartDate>
   <EndDate></EndDate>
   <ItemId></ItemId>
   <RecurringMasterItemId></RecurringMasterItemId>
   <ReminderGroup></ReminderGroup>
   <UID></UID>
</Reminder>

```

 <span data-ttu-id="147f2-105">**Remindertype**</span><span class="sxs-lookup"><span data-stu-id="147f2-105">**ReminderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="147f2-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="147f2-106">Attributes and elements</span></span>

<span data-ttu-id="147f2-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="147f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="147f2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="147f2-108">Attributes</span></span>

<span data-ttu-id="147f2-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="147f2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="147f2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="147f2-110">Child elements</span></span>

<span data-ttu-id="147f2-111">[Assunto](subject.md)  |  [Local](location.md)  |  [ReminderTime](remindertime.md)  |  [StartDate](startdate.md)  |  [EndDate (Remindertype)](enddate-remindertype.md)  |  [ItemId](itemid.md)  |  [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md)  |  Um dos [lembretes](remindergroup.md)  |  [UID](uid.md)</span><span class="sxs-lookup"><span data-stu-id="147f2-111">[Subject](subject.md) | [Location](location.md) | [ReminderTime](remindertime.md) | [StartDate](startdate.md) | [EndDate (ReminderType)](enddate-remindertype.md) | [ItemId](itemid.md) | [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md) | [ReminderGroup](remindergroup.md) | [UID](uid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="147f2-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="147f2-112">Parent elements</span></span>

[<span data-ttu-id="147f2-113">Lembretes</span><span class="sxs-lookup"><span data-stu-id="147f2-113">Reminders</span></span>](reminders.md)
  
## <a name="remarks"></a><span data-ttu-id="147f2-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="147f2-114">Remarks</span></span>

<span data-ttu-id="147f2-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="147f2-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="147f2-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="147f2-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="147f2-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="147f2-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="147f2-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="147f2-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="147f2-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="147f2-119">Schema Name</span></span>  <br/> |<span data-ttu-id="147f2-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="147f2-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="147f2-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="147f2-121">Validation File</span></span>  <br/> |<span data-ttu-id="147f2-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="147f2-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="147f2-123">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="147f2-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="147f2-124">False</span><span class="sxs-lookup"><span data-stu-id="147f2-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="147f2-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="147f2-125">See also</span></span>



[<span data-ttu-id="147f2-126">Lembretes</span><span class="sxs-lookup"><span data-stu-id="147f2-126">Reminders</span></span>](reminders.md)


- [<span data-ttu-id="147f2-127">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="147f2-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

