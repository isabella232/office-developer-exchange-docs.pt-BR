---
title: FreeBusyViewOptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyViewOptions
api_type:
- schema
ms.assetid: c07f3ddb-874b-4d30-a60e-7e5c7793bb6f
description: O elemento FreeBusyViewOptions Especifica o tipo de informações de disponibilidade retornadas na resposta.
ms.openlocfilehash: 703fc6a3625d24cf874a785600e13ee4505b506f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752373"
---
# <a name="freebusyviewoptions"></a><span data-ttu-id="e2025-103">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="e2025-103">FreeBusyViewOptions</span></span>

<span data-ttu-id="e2025-104">O elemento **FreeBusyViewOptions** Especifica o tipo de informações de disponibilidade retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="e2025-104">The **FreeBusyViewOptions** element specifies the type of free/busy information returned in the response.</span></span> 
  
[<span data-ttu-id="e2025-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="e2025-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="e2025-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="e2025-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
```xml
<FreeBusyViewOptions>
   <TimeWindow>...</TimeWindow>
   <MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
<RequestedView>...</RequestedView>
</FreeBusyViewOptions>

```

 <span data-ttu-id="e2025-107">**FreeBusyViewOptionsType**</span><span class="sxs-lookup"><span data-stu-id="e2025-107">**FreeBusyViewOptionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2025-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e2025-108">Attributes and elements</span></span>

<span data-ttu-id="e2025-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e2025-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2025-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="e2025-110">Attributes</span></span>

<span data-ttu-id="e2025-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e2025-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2025-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e2025-112">Child elements</span></span>

|<span data-ttu-id="e2025-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e2025-113">**Element**</span></span>|<span data-ttu-id="e2025-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e2025-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2025-115">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="e2025-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="e2025-116">Identifica o intervalo de tempo consultado para as informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="e2025-116">Identifies the time span queried for the user availability information.</span></span>  <br/> |
|[<span data-ttu-id="e2025-117">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="e2025-117">MergedFreeBusyIntervalInMinutes</span></span>](mergedfreebusyintervalinminutes.md) <br/> |<span data-ttu-id="e2025-118">Representa a diferença de horário entre dois slots sucessivos no modo de exibição **FreeBusyMerged** .</span><span class="sxs-lookup"><span data-stu-id="e2025-118">Represents the time difference between two successive slots in the **FreeBusyMerged** view.</span></span>  <br/> |
|[<span data-ttu-id="e2025-119">RequestedView</span><span class="sxs-lookup"><span data-stu-id="e2025-119">RequestedView</span></span>](requestedview.md) <br/> |<span data-ttu-id="e2025-120">Define o tipo de informações de calendário que um cliente solicitar.</span><span class="sxs-lookup"><span data-stu-id="e2025-120">Defines the type of calendar information that a client requests.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e2025-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e2025-121">Parent elements</span></span>

|<span data-ttu-id="e2025-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e2025-122">**Element**</span></span>|<span data-ttu-id="e2025-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e2025-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2025-124">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="e2025-124">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="e2025-125">Contém os argumentos usados para obter informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="e2025-125">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="e2025-126">Este é um elemento raiz.</span><span class="sxs-lookup"><span data-stu-id="e2025-126">This is a root element.</span></span>  <br/> <span data-ttu-id="e2025-127">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="e2025-127">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e2025-128">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="e2025-128">Remarks</span></span>

<span data-ttu-id="e2025-129">Este elemento não é necessário e somente pode ocorrer uma vez se usada.</span><span class="sxs-lookup"><span data-stu-id="e2025-129">This element is not required and can only occur once if used.</span></span> <span data-ttu-id="e2025-130">Esse valor pode ser null se o valor do elemento [SuggestionsViewOptions](suggestionsviewoptions.md) não for nulo.</span><span class="sxs-lookup"><span data-stu-id="e2025-130">This value can be null if the value of the [SuggestionsViewOptions](suggestionsviewoptions.md) element is not null.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e2025-131">O esquema que descreve este elemento está localizado no diretório /epi/ do computador que está executando o Microsoft® Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="e2025-131">The schema that describes this element is located in the /epi/ directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="example"></a><span data-ttu-id="e2025-132">Example</span><span class="sxs-lookup"><span data-stu-id="e2025-132">Example</span></span>

<span data-ttu-id="e2025-133">O exemplo a seguir obtém uma lista de reuniões e um fluxo de informações de disponibilidade em intervalos de 60 minutos.</span><span class="sxs-lookup"><span data-stu-id="e2025-133">The following example obtains a list of meetings and a free/busy stream in 60-minute intervals.</span></span>
  
```
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
        <MailboxData xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Email>
            <Name></Name>
            <Address>someone@ExServer.example.com</Address>
            <RoutingType>SMTP</RoutingType>
          </Email>
          <AttendeeType>Organizer</AttendeeType>
          <ExcludeConflicts>false</ExcludeConflicts>
          <ExcludeNonWorkingHours>false</ExcludeNonWorkingHours>
        </MailboxData>
      </MailboxDataArray>
      <FreeBusyViewOptions xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <TimeWindow>
          <StartTime>2006-02-06T00:00:00</StartTime>
          <EndTime>2006-02-25T23:59:59</EndTime>
        </TimeWindow>
        <MergedFreeBusyIntervalInMinutes>60</MergedFreeBusyIntervalInMinutes>
        <RequestedView>FreeBusyMerged</RequestedView>
      </FreeBusyViewOptions>
    </GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="e2025-134">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e2025-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2025-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="e2025-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e2025-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e2025-136">Schema Name</span></span>  <br/> |<span data-ttu-id="e2025-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e2025-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="e2025-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e2025-138">Validation File</span></span>  <br/> |<span data-ttu-id="e2025-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e2025-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e2025-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e2025-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="e2025-141">False</span><span class="sxs-lookup"><span data-stu-id="e2025-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2025-142">Ver também</span><span class="sxs-lookup"><span data-stu-id="e2025-142">See also</span></span>



[<span data-ttu-id="e2025-143">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e2025-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="e2025-144">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="e2025-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

