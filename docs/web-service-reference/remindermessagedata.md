---
title: ReminderMessageData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04dd4987-baaf-4ebe-ae58-ad962c2f8fa1
description: O elemento ReminderMessageData especifica os dados em uma mensagem de lembrete.
ms.openlocfilehash: f2632062cd02581c426f7dbfa2a33d53e5594d72
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458548"
---
# <a name="remindermessagedata"></a><span data-ttu-id="ba556-103">ReminderMessageData</span><span class="sxs-lookup"><span data-stu-id="ba556-103">ReminderMessageData</span></span>

<span data-ttu-id="ba556-104">O elemento **ReminderMessageData** especifica os dados em uma mensagem de lembrete.</span><span class="sxs-lookup"><span data-stu-id="ba556-104">The **ReminderMessageData** element specifies the data in a reminder message.</span></span> 
  
```XML
<ReminderMessageData>
   <ReminderText></ReminderText>
   <Location></Location>
   <StartTime></StartTime>
   <EndTime></EndTime>
   <AssociatedCalendarItemId></AssociatedCalendarItemId>
</ReminderMessageData>

```

 <span data-ttu-id="ba556-105">**ReminderMessageDataType**</span><span class="sxs-lookup"><span data-stu-id="ba556-105">**ReminderMessageDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba556-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ba556-106">Attributes and elements</span></span>

<span data-ttu-id="ba556-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ba556-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba556-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ba556-108">Attributes</span></span>

<span data-ttu-id="ba556-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba556-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba556-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ba556-110">Child elements</span></span>

<span data-ttu-id="ba556-111">[ReminderText](remindertext.md)  |  [Local](location.md)  |  [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md)  |  [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md)  |  [AssociatedCalendarItemId](associatedcalendaritemid.md)</span><span class="sxs-lookup"><span data-stu-id="ba556-111">[ReminderText](remindertext.md) | [Location](location.md) | [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [AssociatedCalendarItemId](associatedcalendaritemid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ba556-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ba556-112">Parent elements</span></span>

[<span data-ttu-id="ba556-113">Message</span><span class="sxs-lookup"><span data-stu-id="ba556-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="ba556-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="ba556-114">Remarks</span></span>

<span data-ttu-id="ba556-115">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ba556-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="ba556-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba556-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="ba556-117">As versões do Exchange que começam com o número de compilação 15.00.0913.09 podem incluir o elemento **AssociatedCalendarItemId** como um elemento filho do elemento **ReminderMessageData** .</span><span class="sxs-lookup"><span data-stu-id="ba556-117">Versions of Exchange starting with build number 15.00.0913.09 can include the **AssociatedCalendarItemId** element as a child element of the **ReminderMessageData** element.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ba556-118">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ba556-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba556-119">Namespace</span><span class="sxs-lookup"><span data-stu-id="ba556-119">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ba556-120">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ba556-120">Schema Name</span></span>  <br/> |<span data-ttu-id="ba556-121">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ba556-121">Types schema</span></span>  <br/> |
|<span data-ttu-id="ba556-122">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ba556-122">Validation File</span></span>  <br/> |<span data-ttu-id="ba556-123">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ba556-123">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ba556-124">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ba556-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="ba556-125">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="ba556-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba556-126">Também consulte</span><span class="sxs-lookup"><span data-stu-id="ba556-126">See also</span></span>



[<span data-ttu-id="ba556-127">Message</span><span class="sxs-lookup"><span data-stu-id="ba556-127">Message</span></span>](message-ex15websvcsotherref.md)


- [<span data-ttu-id="ba556-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ba556-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

