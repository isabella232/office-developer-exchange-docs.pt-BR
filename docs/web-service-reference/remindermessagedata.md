---
title: ReminderMessageData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04dd4987-baaf-4ebe-ae58-ad962c2f8fa1
description: O elemento ReminderMessageData Especifica os dados em uma mensagem de lembrete.
ms.openlocfilehash: a1d01dd24030b047bd8ad025f3e1cebed0da8e29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825067"
---
# <a name="remindermessagedata"></a><span data-ttu-id="e725e-103">ReminderMessageData</span><span class="sxs-lookup"><span data-stu-id="e725e-103">ReminderMessageData</span></span>

<span data-ttu-id="e725e-104">O elemento **ReminderMessageData** Especifica os dados em uma mensagem de lembrete.</span><span class="sxs-lookup"><span data-stu-id="e725e-104">The **ReminderMessageData** element specifies the data in a reminder message.</span></span> 
  
```XML
<ReminderMessageData>
   <ReminderText></ReminderText>
   <Location></Location>
   <StartTime></StartTime>
   <EndTime></EndTime>
   <AssociatedCalendarItemId></AssociatedCalendarItemId>
</ReminderMessageData>

```

 <span data-ttu-id="e725e-105">**ReminderMessageDataType**</span><span class="sxs-lookup"><span data-stu-id="e725e-105">**ReminderMessageDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e725e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e725e-106">Attributes and elements</span></span>

<span data-ttu-id="e725e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e725e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e725e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e725e-108">Attributes</span></span>

<span data-ttu-id="e725e-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e725e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e725e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e725e-110">Child elements</span></span>

<span data-ttu-id="e725e-111">[ReminderText](remindertext.md) | [local](location.md) | [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [AssociatedCalendarItemId](associatedcalendaritemid.md)</span><span class="sxs-lookup"><span data-stu-id="e725e-111">[ReminderText](remindertext.md) | [Location](location.md) | [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [AssociatedCalendarItemId](associatedcalendaritemid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e725e-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e725e-112">Parent elements</span></span>

[<span data-ttu-id="e725e-113">Mensagem</span><span class="sxs-lookup"><span data-stu-id="e725e-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="e725e-114">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="e725e-114">Remarks</span></span>

<span data-ttu-id="e725e-115">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e725e-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="e725e-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e725e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="e725e-117">Versões do Exchange, começando com o número de compilação 15.00.0913.09 podem incluir o elemento **AssociatedCalendarItemId** como um elemento filho do elemento **ReminderMessageData** .</span><span class="sxs-lookup"><span data-stu-id="e725e-117">Versions of Exchange starting with build number 15.00.0913.09 can include the **AssociatedCalendarItemId** element as a child element of the **ReminderMessageData** element.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="e725e-118">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e725e-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e725e-119">Namespace</span><span class="sxs-lookup"><span data-stu-id="e725e-119">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e725e-120">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e725e-120">Schema Name</span></span>  <br/> |<span data-ttu-id="e725e-121">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e725e-121">Types schema</span></span>  <br/> |
|<span data-ttu-id="e725e-122">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e725e-122">Validation File</span></span>  <br/> |<span data-ttu-id="e725e-123">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e725e-123">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e725e-124">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e725e-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="e725e-125">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="e725e-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e725e-126">Ver também</span><span class="sxs-lookup"><span data-stu-id="e725e-126">See also</span></span>



[<span data-ttu-id="e725e-127">Mensagem</span><span class="sxs-lookup"><span data-stu-id="e725e-127">Message</span></span>](message-ex15websvcsotherref.md)


- [<span data-ttu-id="e725e-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e725e-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

