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
description: O elemento FreeBusyViewOptions especifica o tipo de informações de disponibilidade retornadas na resposta.
ms.openlocfilehash: b67d3f461e0edaa82f074f75b0c1c54efc8af4d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459571"
---
# <a name="freebusyviewoptions"></a><span data-ttu-id="5adc7-103">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="5adc7-103">FreeBusyViewOptions</span></span>

<span data-ttu-id="5adc7-104">O elemento **FreeBusyViewOptions** especifica o tipo de informações de disponibilidade retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="5adc7-104">The **FreeBusyViewOptions** element specifies the type of free/busy information returned in the response.</span></span> 
  
[<span data-ttu-id="5adc7-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="5adc7-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="5adc7-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="5adc7-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
```xml
<FreeBusyViewOptions>
   <TimeWindow>...</TimeWindow>
   <MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
<RequestedView>...</RequestedView>
</FreeBusyViewOptions>

```

 <span data-ttu-id="5adc7-107">**FreeBusyViewOptionsType**</span><span class="sxs-lookup"><span data-stu-id="5adc7-107">**FreeBusyViewOptionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5adc7-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5adc7-108">Attributes and elements</span></span>

<span data-ttu-id="5adc7-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5adc7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5adc7-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="5adc7-110">Attributes</span></span>

<span data-ttu-id="5adc7-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5adc7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5adc7-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5adc7-112">Child elements</span></span>

|<span data-ttu-id="5adc7-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5adc7-113">**Element**</span></span>|<span data-ttu-id="5adc7-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5adc7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5adc7-115">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="5adc7-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="5adc7-116">Identifica o intervalo de tempo consultado para as informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="5adc7-116">Identifies the time span queried for the user availability information.</span></span>  <br/> |
|[<span data-ttu-id="5adc7-117">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="5adc7-117">MergedFreeBusyIntervalInMinutes</span></span>](mergedfreebusyintervalinminutes.md) <br/> |<span data-ttu-id="5adc7-118">Representa a diferença de tempo entre dois slots sucessivos no modo de exibição **FreeBusyMerged** .</span><span class="sxs-lookup"><span data-stu-id="5adc7-118">Represents the time difference between two successive slots in the **FreeBusyMerged** view.</span></span>  <br/> |
|[<span data-ttu-id="5adc7-119">RequestedView</span><span class="sxs-lookup"><span data-stu-id="5adc7-119">RequestedView</span></span>](requestedview.md) <br/> |<span data-ttu-id="5adc7-120">Define o tipo de informação do calendário que um cliente solicita.</span><span class="sxs-lookup"><span data-stu-id="5adc7-120">Defines the type of calendar information that a client requests.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5adc7-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5adc7-121">Parent elements</span></span>

|<span data-ttu-id="5adc7-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5adc7-122">**Element**</span></span>|<span data-ttu-id="5adc7-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5adc7-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5adc7-124">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="5adc7-124">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="5adc7-125">Contém os argumentos usados para obter informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="5adc7-125">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="5adc7-126">Este é um elemento raiz.</span><span class="sxs-lookup"><span data-stu-id="5adc7-126">This is a root element.</span></span>  <br/> <span data-ttu-id="5adc7-127">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="5adc7-127">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5adc7-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="5adc7-128">Remarks</span></span>

<span data-ttu-id="5adc7-129">Esse elemento não é obrigatório e só poderá ocorrer uma vez se for usado.</span><span class="sxs-lookup"><span data-stu-id="5adc7-129">This element is not required and can only occur once if used.</span></span> <span data-ttu-id="5adc7-130">Esse valor pode ser NULL se o valor do elemento [SuggestionsViewOptions](suggestionsviewoptions.md) não for NULL.</span><span class="sxs-lookup"><span data-stu-id="5adc7-130">This value can be null if the value of the [SuggestionsViewOptions](suggestionsviewoptions.md) element is not null.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5adc7-131">O esquema que descreve este elemento está localizado no diretório/EPI/do computador que está executando o Microsoft® Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="5adc7-131">The schema that describes this element is located in the /epi/ directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="example"></a><span data-ttu-id="5adc7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5adc7-132">Example</span></span>

<span data-ttu-id="5adc7-133">O exemplo a seguir obtém uma lista de reuniões e um fluxo de disponibilidade em intervalos de 60 minutos.</span><span class="sxs-lookup"><span data-stu-id="5adc7-133">The following example obtains a list of meetings and a free/busy stream in 60-minute intervals.</span></span>
  
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
            <Address>someone@ExServer.example.com</Address>
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
          <EndTime>2006-02-25T23:59:59</EndTime>
        </TimeWindow>
        <MergedFreeBusyIntervalInMinutes>60</MergedFreeBusyIntervalInMinutes>
        <RequestedView>FreeBusyMerged</RequestedView>
      </FreeBusyViewOptions>
    </GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="5adc7-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5adc7-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5adc7-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="5adc7-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5adc7-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5adc7-136">Schema Name</span></span>  <br/> |<span data-ttu-id="5adc7-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5adc7-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="5adc7-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5adc7-138">Validation File</span></span>  <br/> |<span data-ttu-id="5adc7-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5adc7-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5adc7-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5adc7-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="5adc7-141">False</span><span class="sxs-lookup"><span data-stu-id="5adc7-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5adc7-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="5adc7-142">See also</span></span>



[<span data-ttu-id="5adc7-143">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="5adc7-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="5adc7-144">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="5adc7-144">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

