---
title: AssociatedCalendarItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AssociatedCalendarItemId
api_type:
- schema
ms.assetid: 5b29898c-ea59-4e6a-914c-c011ec754032
description: O elemento AssociatedCalendarItemId representa o item de calendário que está associado a um MeetingMessage, MeetingRequest, MeetingResponse, MeetingCancellation ou ReminderMessageData.
ms.openlocfilehash: 816372c38243ba0fe5a7606c264dd1c5107350f2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460880"
---
# <a name="associatedcalendaritemid"></a><span data-ttu-id="9c96b-103">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="9c96b-103">AssociatedCalendarItemId</span></span>

<span data-ttu-id="9c96b-104">O **elemento AssociatedCalendarItemId** representa o item de calendário que está associado a um [MeetingMessage](meetingmessage.md), [MeetingRequest](meetingrequest.md), [MeetingResponse](meetingresponse.md), [MeetingCancellation](meetingcancellation.md)ou [ReminderMessageData](remindermessagedata.md).</span><span class="sxs-lookup"><span data-stu-id="9c96b-104">The **AssociatedCalendarItemId** element represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md), [MeetingRequest](meetingrequest.md), [MeetingResponse](meetingresponse.md), [MeetingCancellation](meetingcancellation.md), or [ReminderMessageData](remindermessagedata.md).</span></span>
  
```XML
<AssociatedCalendarItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="9c96b-105">**ItemIdtype**</span><span class="sxs-lookup"><span data-stu-id="9c96b-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c96b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9c96b-106">Attributes and elements</span></span>

<span data-ttu-id="9c96b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9c96b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c96b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9c96b-108">Attributes</span></span>

|<span data-ttu-id="9c96b-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="9c96b-109">**Attribute**</span></span>|<span data-ttu-id="9c96b-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9c96b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9c96b-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="9c96b-111">**Id**</span></span> <br/> |<span data-ttu-id="9c96b-112">Identifica o item de calendário que está associado à reunião.</span><span class="sxs-lookup"><span data-stu-id="9c96b-112">Identifies the calendar item that is associated with meeting.</span></span>  <br/> |
|<span data-ttu-id="9c96b-113">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="9c96b-113">**ChangeKey**</span></span> <br/> |<span data-ttu-id="9c96b-114">Identifica uma versão específica do item de calendário que está associada a uma reunião.</span><span class="sxs-lookup"><span data-stu-id="9c96b-114">Identifies a specific version of the calendar item that is associated with a meeting.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9c96b-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9c96b-115">Child elements</span></span>

<span data-ttu-id="9c96b-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9c96b-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9c96b-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9c96b-117">Parent elements</span></span>

<span data-ttu-id="9c96b-118">[MeetingMessage](meetingmessage.md)  |  [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [ReminderMessageData](remindermessagedata.md)</span><span class="sxs-lookup"><span data-stu-id="9c96b-118">[MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [ReminderMessageData](remindermessagedata.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9c96b-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="9c96b-119">Remarks</span></span>

<span data-ttu-id="9c96b-120">As versões do Exchange que começam com o número de compilação 15.00.0913.09 podem incluir o elemento **AssociatedCalendarItemId** como um elemento filho do elemento **ReminderMessageData** .</span><span class="sxs-lookup"><span data-stu-id="9c96b-120">Versions of Exchange starting with build number 15.00.0913.09 can include the **AssociatedCalendarItemId** element as a child element of the **ReminderMessageData** element.</span></span> 
  
<span data-ttu-id="9c96b-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c96b-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c96b-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9c96b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c96b-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="9c96b-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9c96b-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9c96b-124">Schema Name</span></span>  <br/> |<span data-ttu-id="9c96b-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9c96b-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="9c96b-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9c96b-126">Validation File</span></span>  <br/> |<span data-ttu-id="9c96b-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9c96b-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9c96b-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9c96b-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="9c96b-129">False</span><span class="sxs-lookup"><span data-stu-id="9c96b-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c96b-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="9c96b-130">See also</span></span>

- [<span data-ttu-id="9c96b-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9c96b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

