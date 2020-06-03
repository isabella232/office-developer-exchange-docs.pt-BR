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
description: O elemento SuggestionsViewOptions contém as opções para obter informações de sugestão de reunião.
ms.openlocfilehash: f584b19997f98760bd4e438dcd48a5c18cc63e4b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44433991"
---
# <a name="suggestionsviewoptions"></a><span data-ttu-id="10838-103">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="10838-103">SuggestionsViewOptions</span></span>

<span data-ttu-id="10838-104">O elemento **SuggestionsViewOptions** contém as opções para obter informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="10838-104">The **SuggestionsViewOptions** element contains the options for obtaining meeting suggestion information.</span></span> 
  
[<span data-ttu-id="10838-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="10838-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="10838-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="10838-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
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

 <span data-ttu-id="10838-107">**SuggestionsViewOptionsType**</span><span class="sxs-lookup"><span data-stu-id="10838-107">**SuggestionsViewOptionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="10838-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="10838-108">Attributes and elements</span></span>

<span data-ttu-id="10838-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="10838-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10838-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="10838-110">Attributes</span></span>

<span data-ttu-id="10838-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10838-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="10838-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="10838-112">Child elements</span></span>

|<span data-ttu-id="10838-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="10838-113">**Element**</span></span>|<span data-ttu-id="10838-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="10838-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10838-115">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="10838-115">GoodThreshold</span></span>](goodthreshold.md) <br/> |<span data-ttu-id="10838-116">Especifica a porcentagem de participantes que devem ter o período de tempo aberto para que o período de tempo se qualifique como bom horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="10838-116">Specifies the percentage of attendees that must have the time period open for the time period to qualify as a good suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="10838-117">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="10838-117">MaximumResultsByDay</span></span>](maximumresultsbyday.md) <br/> |<span data-ttu-id="10838-118">Especifica o número de horas de reunião sugeridas por dia retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="10838-118">Specifies the number of suggested meeting times per day returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="10838-119">MaximumNonWorkHourResultsByDay</span><span class="sxs-lookup"><span data-stu-id="10838-119">MaximumNonWorkHourResultsByDay</span></span>](maximumnonworkhourresultsbyday.md) <br/> |<span data-ttu-id="10838-120">Especifica o número de resultados sugeridos para horários de reuniões fora de horas de trabalho normais por dia.</span><span class="sxs-lookup"><span data-stu-id="10838-120">Specifies the number of suggested results for meeting times outside regular working hours per day.</span></span>  <br/> |
|[<span data-ttu-id="10838-121">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="10838-121">MeetingDurationInMinutes</span></span>](meetingdurationinminutes.md) <br/> |<span data-ttu-id="10838-122">Especifica a duração da reunião a ser sugerida.</span><span class="sxs-lookup"><span data-stu-id="10838-122">Specifies the length of the meeting to be suggested.</span></span>  <br/> |
|[<span data-ttu-id="10838-123">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="10838-123">MinimumSuggestionQuality</span></span>](minimumsuggestionquality.md) <br/> |<span data-ttu-id="10838-124">Especifica a qualidade das sugestões de reunião a serem retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="10838-124">Specifies the quality of meeting suggestions to be returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="10838-125">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="10838-125">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="10838-126">Identifica o período de tempo que é consultado para informações detalhadas sobre os horários de reunião sugeridos.</span><span class="sxs-lookup"><span data-stu-id="10838-126">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="10838-127">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="10838-127">CurrentMeetingTime</span></span>](currentmeetingtime.md) <br/> |<span data-ttu-id="10838-128">Representa a hora de início de uma reunião que você deseja atualizar com os resultados de tempo de reunião sugeridos.</span><span class="sxs-lookup"><span data-stu-id="10838-128">Represents the start time of a meeting that you want to update with the suggested meeting time results.</span></span>  <br/> |
|[<span data-ttu-id="10838-129">GlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="10838-129">GlobalObjectId</span></span>](globalobjectid.md) <br/> |<span data-ttu-id="10838-130">Esse elemento não é usado.</span><span class="sxs-lookup"><span data-stu-id="10838-130">This element is not used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="10838-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="10838-131">Parent elements</span></span>

|<span data-ttu-id="10838-132">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="10838-132">**Element**</span></span>|<span data-ttu-id="10838-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="10838-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10838-134">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="10838-134">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="10838-135">Contém os argumentos usados para obter informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="10838-135">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="10838-136">Este é um elemento raiz.</span><span class="sxs-lookup"><span data-stu-id="10838-136">This is a root element.</span></span>  <br/> <span data-ttu-id="10838-137">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="10838-137">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="10838-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="10838-138">Remarks</span></span>

<span data-ttu-id="10838-139">Esse elemento não é obrigatório e só poderá ocorrer uma vez se for usado.</span><span class="sxs-lookup"><span data-stu-id="10838-139">This element is not required and can only occur once if used.</span></span> <span data-ttu-id="10838-140">Esse valor pode ser NULL se o valor do elemento [FreeBusyViewOptions](freebusyviewoptions.md) não for NULL.</span><span class="sxs-lookup"><span data-stu-id="10838-140">This value can be null if the value of the [FreeBusyViewOptions](freebusyviewoptions.md) element is not null.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="10838-141">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="10838-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="10838-142">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="10838-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="10838-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="10838-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="10838-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="10838-144">Schema Name</span></span>  <br/> |<span data-ttu-id="10838-145">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="10838-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="10838-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="10838-146">Validation File</span></span>  <br/> |<span data-ttu-id="10838-147">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="10838-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="10838-148">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="10838-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="10838-149">False</span><span class="sxs-lookup"><span data-stu-id="10838-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="10838-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="10838-150">See also</span></span>



[<span data-ttu-id="10838-151">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="10838-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="10838-152">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="10838-152">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

