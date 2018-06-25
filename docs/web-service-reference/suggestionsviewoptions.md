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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837675"
---
# <a name="suggestionsviewoptions"></a>SuggestionsViewOptions

O elemento de **SuggestionsViewOptions** contém as opções para obter informações de sugestão de reunião. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
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

 **SuggestionsViewOptionsType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GoodThreshold](goodthreshold.md) <br/> |Especifica a porcentagem de participantes que devem ter o período de tempo open para o período de tempo para se qualificar como um horário de reunião sugerido BOM.  <br/> |
|[MaximumResultsByDay](maximumresultsbyday.md) <br/> |Especifica o número de vezes que a reunião sugerido por dia retornados na resposta.  <br/> |
|[MaximumNonWorkHourResultsByDay](maximumnonworkhourresultsbyday.md) <br/> |Especifica o número de resultados sugeridos para horários fora do horário normal de trabalho por dia da reunião.  <br/> |
|[MeetingDurationInMinutes](meetingdurationinminutes.md) <br/> |Especifica o comprimento da reunião a ser sugerido.  <br/> |
|[MinimumSuggestionQuality](minimumsuggestionquality.md) <br/> |Especifica a qualidade das sugestões de reunião a serem retornados na resposta.  <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Identifica o intervalo de tempo que está sendo consultado para obter informações detalhadas sobre reuniões sugeridas.  <br/> |
|[CurrentMeetingTime](currentmeetingtime.md) <br/> |Resultados de tempo representa a hora de início de uma reunião que você deseja atualizar com a reunião sugerida.  <br/> |
|[GlobalObjectId](globalobjectid.md) <br/> |Este elemento não é usado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Contém os argumentos usados para obter informações de disponibilidade do usuário. Este é um elemento raiz.  <br/> Este é o XPath a este elemento:  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento não é necessário e somente pode ocorrer uma vez se usada. Esse valor pode ser null se o valor do elemento [FreeBusyViewOptions](freebusyviewoptions.md) não for nulo. 
  
> [!NOTE]
> O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente. 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetUserAvailability](getuseravailability-operation.md)


[Obtenção de disponibilidade do usuário](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

