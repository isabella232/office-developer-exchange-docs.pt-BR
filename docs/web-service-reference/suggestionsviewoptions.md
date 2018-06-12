---
title: SuggestionsViewOptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionsViewOptions
api_type:
- schema
ms.assetid: bb04ae38-e62d-4a69-a479-8ff326ca726e
description: O elemento de SuggestionsViewOptions contém as opções para obter informações de sugestão de reunião.
ms.openlocfilehash: 09ff317ae0b2ebf1eadc89dc3bb1cf5b3ae19dcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837675"
---
# <a name="suggestionsviewoptions"></a><span data-ttu-id="0f75d-103">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="0f75d-103">SuggestionsViewOptions</span></span>

<span data-ttu-id="0f75d-104">O elemento de **SuggestionsViewOptions** contém as opções para obter informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="0f75d-104">The **SuggestionsViewOptions** element contains the options for obtaining meeting suggestion information.</span></span> 
  
[<span data-ttu-id="0f75d-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="0f75d-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="0f75d-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="0f75d-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
```xml
<SuggestionsViewOptions>
   <GoodThreshold>...</GoodThreshold>
   <MaximumResultsByDay>...</MaximumResultsByDay>
   <MaximumNonWorkingHourResultsByDay>...</MaximumNonWorkingHourResultsByDay>
   <MeetingDurationInMinutes>...</MeetingDurationInMinutes>
   <MinimumSuggestionQuality>...</MinimumSuggestionQuality>
   <SuggestionIntervalInMinutes>...</SuggestionIntervalInMinutes>
   <DetailedSuggestionsWindow>...</DetailedSuggestionsWindow>
   <CurrentMeetingTime>...</CurrentMeetingTime>
   <GlobalObjectId>...</GlobalObjectId>
</SuggestionsViewOptions>
```

 <span data-ttu-id="0f75d-107">**SuggestionsViewOptionsType**</span><span class="sxs-lookup"><span data-stu-id="0f75d-107">**SuggestionsViewOptionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f75d-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0f75d-108">Attributes and elements</span></span>

<span data-ttu-id="0f75d-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0f75d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f75d-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="0f75d-110">Attributes</span></span>

<span data-ttu-id="0f75d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0f75d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f75d-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0f75d-112">Child elements</span></span>

|<span data-ttu-id="0f75d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0f75d-113">**Element**</span></span>|<span data-ttu-id="0f75d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0f75d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f75d-115">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="0f75d-115">GoodThreshold</span></span>](goodthreshold.md) <br/> |<span data-ttu-id="0f75d-116">Especifica a porcentagem de participantes que devem ter o período de tempo open para o período de tempo para se qualificar como um horário de reunião sugerido BOM.</span><span class="sxs-lookup"><span data-stu-id="0f75d-116">Specifies the percentage of attendees that must have the time period open for the time period to qualify as a good suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="0f75d-117">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="0f75d-117">MaximumResultsByDay</span></span>](maximumresultsbyday.md) <br/> |<span data-ttu-id="0f75d-118">Especifica o número de vezes que a reunião sugerido por dia retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="0f75d-118">Specifies the number of suggested meeting times per day returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="0f75d-119">MaximumNonWorkHourResultsByDay</span><span class="sxs-lookup"><span data-stu-id="0f75d-119">MaximumNonWorkHourResultsByDay</span></span>](maximumnonworkhourresultsbyday.md) <br/> |<span data-ttu-id="0f75d-120">Especifica o número de resultados sugeridos para horários fora do horário normal de trabalho por dia da reunião.</span><span class="sxs-lookup"><span data-stu-id="0f75d-120">Specifies the number of suggested results for meeting times outside regular working hours per day.</span></span>  <br/> |
|[<span data-ttu-id="0f75d-121">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="0f75d-121">MeetingDurationInMinutes</span></span>](meetingdurationinminutes.md) <br/> |<span data-ttu-id="0f75d-122">Especifica o comprimento da reunião a ser sugerido.</span><span class="sxs-lookup"><span data-stu-id="0f75d-122">Specifies the length of the meeting to be suggested.</span></span>  <br/> |
|[<span data-ttu-id="0f75d-123">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="0f75d-123">MinimumSuggestionQuality</span></span>](minimumsuggestionquality.md) <br/> |<span data-ttu-id="0f75d-124">Especifica a qualidade das sugestões de reunião a serem retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="0f75d-124">Specifies the quality of meeting suggestions to be returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="0f75d-125">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="0f75d-125">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="0f75d-126">Identifica o intervalo de tempo que está sendo consultado para obter informações detalhadas sobre reuniões sugeridas.</span><span class="sxs-lookup"><span data-stu-id="0f75d-126">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="0f75d-127">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="0f75d-127">CurrentMeetingTime</span></span>](currentmeetingtime.md) <br/> |<span data-ttu-id="0f75d-128">Resultados de tempo representa a hora de início de uma reunião que você deseja atualizar com a reunião sugerida.</span><span class="sxs-lookup"><span data-stu-id="0f75d-128">Represents the start time of a meeting that you want to update with the suggested meeting time results.</span></span>  <br/> |
|[<span data-ttu-id="0f75d-129">GlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="0f75d-129">GlobalObjectId</span></span>](globalobjectid.md) <br/> |<span data-ttu-id="0f75d-130">Este elemento não é usado.</span><span class="sxs-lookup"><span data-stu-id="0f75d-130">This element is not used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0f75d-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0f75d-131">Parent elements</span></span>

|<span data-ttu-id="0f75d-132">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0f75d-132">**Element**</span></span>|<span data-ttu-id="0f75d-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0f75d-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f75d-134">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="0f75d-134">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="0f75d-135">Contém os argumentos usados para obter informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f75d-135">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="0f75d-136">Este é um elemento raiz.</span><span class="sxs-lookup"><span data-stu-id="0f75d-136">This is a root element.</span></span>  <br/> <span data-ttu-id="0f75d-137">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="0f75d-137">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0f75d-138">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="0f75d-138">Remarks</span></span>

<span data-ttu-id="0f75d-139">Este elemento não é necessário e somente pode ocorrer uma vez se usada.</span><span class="sxs-lookup"><span data-stu-id="0f75d-139">This element is not required and can only occur once if used.</span></span> <span data-ttu-id="0f75d-140">Esse valor pode ser null se o valor do elemento [FreeBusyViewOptions](freebusyviewoptions.md) não for nulo.</span><span class="sxs-lookup"><span data-stu-id="0f75d-140">This value can be null if the value of the [FreeBusyViewOptions](freebusyviewoptions.md) element is not null.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0f75d-141">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="0f75d-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="0f75d-142">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0f75d-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f75d-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="0f75d-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0f75d-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0f75d-144">Schema Name</span></span>  <br/> |<span data-ttu-id="0f75d-145">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0f75d-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="0f75d-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0f75d-146">Validation File</span></span>  <br/> |<span data-ttu-id="0f75d-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0f75d-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0f75d-148">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0f75d-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="0f75d-149">False</span><span class="sxs-lookup"><span data-stu-id="0f75d-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0f75d-150">Ver também</span><span class="sxs-lookup"><span data-stu-id="0f75d-150">See also</span></span>



[<span data-ttu-id="0f75d-151">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="0f75d-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="0f75d-152">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="0f75d-152">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

