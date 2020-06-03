---
title: GetUserAvailabilityRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserAvailabilityRequest
api_type:
- schema
ms.assetid: 7906711b-80a1-42ae-8b33-26eeac036a5a
description: O elemento GetUserAvailabilityRequest contém os argumentos usados para obter informações de disponibilidade do usuário. Este é um elemento raiz.
ms.openlocfilehash: 6c2e2c5452b6379171e49cf6aea2d437152ecb9b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459115"
---
# <a name="getuseravailabilityrequest"></a><span data-ttu-id="dc1b1-104">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="dc1b1-104">GetUserAvailabilityRequest</span></span>

<span data-ttu-id="dc1b1-105">O elemento **GetUserAvailabilityRequest** contém os argumentos usados para obter informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-105">The **GetUserAvailabilityRequest** element contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="dc1b1-106">Este é um elemento raiz.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-106">This is a root element.</span></span> 
  
```xml
<GetUserAvailabilityRequest>
   <TimeZone>...</TimeZone>
   <MailboxDataArray>...</MailboxDataArray>
   <FreeBusyViewOptions>...</FreeBusyViewOptions>
   <SuggestionsViewOptions>...</SuggestionsViewOptions>
</GetUserAvailabilityRequest>
```

 <span data-ttu-id="dc1b1-107">**GetUserAvailabilityRequestType**</span><span class="sxs-lookup"><span data-stu-id="dc1b1-107">**GetUserAvailabilityRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc1b1-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="dc1b1-108">Attributes and elements</span></span>

<span data-ttu-id="dc1b1-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc1b1-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="dc1b1-110">Attributes</span></span>

<span data-ttu-id="dc1b1-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dc1b1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc1b1-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dc1b1-112">Child elements</span></span>

|<span data-ttu-id="dc1b1-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dc1b1-113">**Element**</span></span>|<span data-ttu-id="dc1b1-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dc1b1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc1b1-115">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="dc1b1-115">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> |<span data-ttu-id="dc1b1-116">Contém elementos que identificam informações de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-116">Contains elements that identify time zone information.</span></span> <span data-ttu-id="dc1b1-117">Esse elemento também contém informações sobre a transição entre o horário padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-117">This element also contains information about the transition between standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="dc1b1-118">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="dc1b1-118">MailboxDataArray</span></span>](mailboxdataarray.md) <br/> |<span data-ttu-id="dc1b1-119">Contém uma lista de caixas de correio para consultar informações de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-119">Contains a list of mailboxes to query for availability information.</span></span>  <br/> |
|[<span data-ttu-id="dc1b1-120">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="dc1b1-120">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="dc1b1-121">Especifica o tipo de informações de disponibilidade retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-121">Specifies the type of free/busy information returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="dc1b1-122">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="dc1b1-122">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="dc1b1-123">Contém as opções para obter informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-123">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dc1b1-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dc1b1-124">Parent elements</span></span>

<span data-ttu-id="dc1b1-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dc1b1-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dc1b1-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="dc1b1-126">Remarks</span></span>

<span data-ttu-id="dc1b1-127">O esquema que descreve este elemento está localizado no diretório/EWS/do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-127">The schema that describes this element is located in the /EWS/ directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="dc1b1-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc1b1-128">Example</span></span>

<span data-ttu-id="dc1b1-129">O exemplo a seguir mostra uma solicitação de informações de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-129">The following example shows a request for free/busy information.</span></span>
  
```
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
      <MailboxDataArray>
        <MailboxData xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Email>
            <Name></Name>
            <Address>someone@exchangeserver.example.com</Address>
            <RoutingType>SMTP</RoutingType>
          </Email>
          <AttendeeType>Organizer</AttendeeType>
          <ExcludeConflicts>false</ExcludeConflicts>
          <ExcludeNonWorkingHours>false</ExcludeNonWorkingHours>
        </MailboxData>
      </MailboxDataArray>
      <FreeBusyViewOptions xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <TimeWindow>
          <StartTime>2006-02-06T00:00:00</StartTime>
          <EndTime>2006-02-30T23:59:59</EndTime>
        </TimeWindow>
        <MergedFreeBusyIntervalInMinutes>60</MergedFreeBusyIntervalInMinutes>
        <RequestedView>FreeBusyMerged</RequestedView>
      </FreeBusyViewOptions>
    </GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="dc1b1-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="dc1b1-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc1b1-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="dc1b1-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dc1b1-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dc1b1-132">Schema Name</span></span>  <br/> |<span data-ttu-id="dc1b1-133">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="dc1b1-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dc1b1-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dc1b1-134">Validation File</span></span>  <br/> |<span data-ttu-id="dc1b1-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dc1b1-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dc1b1-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="dc1b1-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="dc1b1-137">False</span><span class="sxs-lookup"><span data-stu-id="dc1b1-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc1b1-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="dc1b1-138">See also</span></span>



[<span data-ttu-id="dc1b1-139">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="dc1b1-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="dc1b1-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="dc1b1-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="dc1b1-141">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="dc1b1-141">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

