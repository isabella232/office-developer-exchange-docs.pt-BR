---
title: GetUserAvailabilityResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserAvailabilityResponse
api_type:
- schema
ms.assetid: 6999510a-d60e-43da-8964-57b5fb3e9d11
description: O elemento GetUserAvailabilityResponse é o elemento raiz que contém as propriedades que definem informações de disponibilidade do usuário ou informações de tempo de reunião sugeridas.
ms.openlocfilehash: ceb24bc8b31a7d7313add213c26bef5efd3c89ae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458212"
---
# <a name="getuseravailabilityresponse"></a><span data-ttu-id="39519-103">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="39519-103">GetUserAvailabilityResponse</span></span>

<span data-ttu-id="39519-104">O elemento **GetUserAvailabilityResponse** é o elemento raiz que contém as propriedades que definem informações de disponibilidade do usuário ou informações de tempo de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="39519-104">The **GetUserAvailabilityResponse** element is the root element that contains the properties that define user availability information or suggested meeting time information.</span></span> 
  
```xml
<GetUserAvailabilityResponse>
   <FreeBusyResponseArray>...</FreeBusyResponseArray>
   <SuggestionsResponse>...</SuggestionsResponse>
</GetUserAvailabilityResponse>
```

 <span data-ttu-id="39519-105">**GetUserAvailabilityResponseType**</span><span class="sxs-lookup"><span data-stu-id="39519-105">**GetUserAvailabilityResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="39519-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="39519-106">Attributes and elements</span></span>

<span data-ttu-id="39519-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="39519-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="39519-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="39519-108">Attributes</span></span>

<span data-ttu-id="39519-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="39519-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="39519-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="39519-110">Child elements</span></span>

|<span data-ttu-id="39519-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="39519-111">**Element**</span></span>|<span data-ttu-id="39519-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="39519-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39519-113">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="39519-113">FreeBusyResponseArray</span></span>](freebusyresponsearray.md) <br/> |<span data-ttu-id="39519-114">Contém as informações de disponibilidade dos usuários solicitados e o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="39519-114">Contains the requested users' availability information and the response status.</span></span>  <br/> |
|[<span data-ttu-id="39519-115">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="39519-115">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="39519-116">Contém informações de status de resposta e dados de sugestão para sugestões de reunião solicitadas.</span><span class="sxs-lookup"><span data-stu-id="39519-116">Contains response status information and suggestion data for requested meeting suggestions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="39519-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="39519-117">Parent elements</span></span>

<span data-ttu-id="39519-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="39519-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="39519-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="39519-119">Remarks</span></span>

<span data-ttu-id="39519-120">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="39519-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="39519-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39519-121">Example</span></span>

<span data-ttu-id="39519-122">O exemplo a seguir de uma resposta GetUserAvailability mostra uma resposta a uma solicitação GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="39519-122">The following example of a GetUserAvailability response shows a response to a GetUserAvailability request.</span></span>
  
```
<?xml version="1.0" encoding="utf-8" ?>
<GetUserAvailabilityResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <FreeBusyResponseArray xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <FreeBusyResponse>
      <ResponseMessage ResponseClass="Success">
        <Path select="/m:GetUserAvailabilityRequest/MailboxDataArray[0]" />
      </ResponseMessage>
      <FreeBusyView>
        <FreeBusyViewType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Detailed</FreeBusyViewType>
        <CalendarEventArray xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <CalendarEvent>
            <StartTime>2006-02-28T19:00:00-08:00</StartTime>
            <EndTime>2006-02-28T23:30:00-08:00</EndTime>
            <BusyType>OOF</BusyType>
            <IsPrivate>false</IsPrivate>
            <CalendarEventDetails>
              <ID>00000</ID>
              <Subject>Exercise</Subject>
              <Location>the gym</Location>
              <IsMeeting>false</IsMeeting>
              <IsRecurring>false</IsRecurring>
              <IsException>false</IsException>
              <IsReminderSet>true</IsReminderSet>
            </CalendarEventDetails>
          </CalendarEvent>
        </CalendarEventArray>
        <WorkingHours xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <TimeZone>
            <Bias>480</Bias>
            <StandardTime>
              <Bias>0</Bias>
              <Time>02:00:00</Time>
              <DayOrder>5</DayOrder>
              <Month>10</Month>
              <DayOfWeek>Sunday</DayOfWeek>
            </StandardTime>
            <DaylightTime>
              <Bias>-60</Bias>
              <Time>02:00:00</Time>
              <DayOrder>1</DayOrder>
              <Month>4</Month>
              <DayOfWeek>Sunday</DayOfWeek>
            </DaylightTime>
          </TimeZone>
          <WorkingPeriodArray>
            <WorkingPeriod>
              <DayOfWeek>Monday Tuesday Wednesday Thursday Friday</DayOfWeek>
              <StartTimeInMinutes>480</StartTimeInMinutes>
              <EndTimeInMinutes>1020</EndTimeInMinutes>
            </WorkingPeriod>
          </WorkingPeriodArray>
        </WorkingHours>
      </FreeBusyView>
    </FreeBusyResponse>
  </FreeBusyResponseArray>
</GetUserAvailabilityResponse>
```

<span data-ttu-id="39519-123">O conteúdo do elemento [ID](id.md) foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="39519-123">The [ID](id.md) element contents were shortened to preserve readability.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="39519-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="39519-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="39519-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="39519-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="39519-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="39519-126">Schema Name</span></span>  <br/> |<span data-ttu-id="39519-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="39519-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="39519-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="39519-128">Validation File</span></span>  <br/> |<span data-ttu-id="39519-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="39519-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="39519-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="39519-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="39519-131">False</span><span class="sxs-lookup"><span data-stu-id="39519-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="39519-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="39519-132">See also</span></span>



[<span data-ttu-id="39519-133">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="39519-133">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)


[<span data-ttu-id="39519-134">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="39519-134">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

