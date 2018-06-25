---
title: GetReminders
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 943c3d5d-7d29-4d70-932c-8a4fe44a0037
description: O elemento GetReminders Especifica uma solicitação para receber lembretes.
ms.openlocfilehash: f4ecc858af2150bb3f88ebdf9ed541892f2fead1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752608"
---
# <a name="getreminders"></a><span data-ttu-id="ef970-103">GetReminders</span><span class="sxs-lookup"><span data-stu-id="ef970-103">GetReminders</span></span>

<span data-ttu-id="ef970-104">O elemento **GetReminders** Especifica uma solicitação para receber lembretes.</span><span class="sxs-lookup"><span data-stu-id="ef970-104">The **GetReminders** element specifies a request to get reminders.</span></span> 
  
```XML
<GetReminders>
   <BeginTime/>
   <EndTime/>
   <MaxItems/>
   <ReminderType/>
</GetReminders>

```

 <span data-ttu-id="ef970-105">**GetRemindersType**</span><span class="sxs-lookup"><span data-stu-id="ef970-105">**GetRemindersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef970-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ef970-106">Attributes and elements</span></span>

<span data-ttu-id="ef970-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ef970-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef970-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ef970-108">Attributes</span></span>

<span data-ttu-id="ef970-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ef970-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ef970-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ef970-110">Child elements</span></span>

<span data-ttu-id="ef970-111">[BeginTime](begintime.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [MaxItems](maxitems.md) | [ReminderType](remindertype.md)</span><span class="sxs-lookup"><span data-stu-id="ef970-111">[BeginTime](begintime.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [MaxItems](maxitems.md) | [ReminderType](remindertype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ef970-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ef970-112">Parent elements</span></span>

<span data-ttu-id="ef970-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ef970-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ef970-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="ef970-114">Remarks</span></span>

<span data-ttu-id="ef970-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ef970-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ef970-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ef970-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef970-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ef970-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef970-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="ef970-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ef970-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ef970-119">Schema Name</span></span>  <br/> |<span data-ttu-id="ef970-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ef970-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ef970-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ef970-121">Validation File</span></span>  <br/> |<span data-ttu-id="ef970-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ef970-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ef970-123">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ef970-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="ef970-124">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="ef970-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef970-125">Ver também</span><span class="sxs-lookup"><span data-stu-id="ef970-125">See also</span></span>



- [<span data-ttu-id="ef970-126">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ef970-126">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

