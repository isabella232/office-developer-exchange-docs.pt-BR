---
title: ReminderItemAction
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fe67512c-5b15-4f07-8628-74cf873c2d71
description: O elemento ReminderItemAction especifica a ação para um item de lembrete.
ms.openlocfilehash: 60722235ed3e73e6a9923df8d3c63a6fc123599a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466224"
---
# <a name="reminderitemaction"></a><span data-ttu-id="d5633-103">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="d5633-103">ReminderItemAction</span></span>

<span data-ttu-id="d5633-104">O elemento **ReminderItemAction** especifica a ação para um item de lembrete.</span><span class="sxs-lookup"><span data-stu-id="d5633-104">The **ReminderItemAction** element specifies the action for a reminder item.</span></span> 
  
```XML
<ReminderItemAction>
   <ActionType></ActionType>
   <ItemId></ItemId>
   <NewReminderTime></NewReminderTime>
</ReminderItemAction>
```

 <span data-ttu-id="d5633-105">**ReminderItemActionType**</span><span class="sxs-lookup"><span data-stu-id="d5633-105">**ReminderItemActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5633-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d5633-106">Attributes and elements</span></span>

<span data-ttu-id="d5633-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d5633-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5633-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d5633-108">Attributes</span></span>

<span data-ttu-id="d5633-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5633-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5633-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d5633-110">Child elements</span></span>

<span data-ttu-id="d5633-111">[ActionType (ReminderActionType)](actiontype-reminderactiontype.md)  |  [ItemId](itemid.md)  |  [NewReminderTime](newremindertime.md)</span><span class="sxs-lookup"><span data-stu-id="d5633-111">[ActionType (ReminderActionType)](actiontype-reminderactiontype.md) | [ItemId](itemid.md) | [NewReminderTime](newremindertime.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d5633-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d5633-112">Parent elements</span></span>

[<span data-ttu-id="d5633-113">ReminderItemActions</span><span class="sxs-lookup"><span data-stu-id="d5633-113">ReminderItemActions</span></span>](reminderitemactions.md)
  
## <a name="remarks"></a><span data-ttu-id="d5633-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="d5633-114">Remarks</span></span>

<span data-ttu-id="d5633-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d5633-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d5633-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d5633-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5633-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d5633-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5633-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="d5633-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d5633-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d5633-119">Schema Name</span></span>  <br/> |<span data-ttu-id="d5633-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d5633-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="d5633-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d5633-121">Validation File</span></span>  <br/> |<span data-ttu-id="d5633-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d5633-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d5633-123">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d5633-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5633-124">False</span><span class="sxs-lookup"><span data-stu-id="d5633-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5633-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="d5633-125">See also</span></span>



[<span data-ttu-id="d5633-126">ReminderItemActions</span><span class="sxs-lookup"><span data-stu-id="d5633-126">ReminderItemActions</span></span>](reminderitemactions.md)


- [<span data-ttu-id="d5633-127">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d5633-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

