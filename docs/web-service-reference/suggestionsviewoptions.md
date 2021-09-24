---
title: SuggestionsViewOptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SuggestionsViewOptions
api_type:
- schema
ms.assetid: bb04ae38-e62d-4a69-a479-8ff326ca726e
description: O elemento SuggestionsViewOptions contém as opções para obter informações de sugestão de reunião.
ms.openlocfilehash: ba3591b88e581d45c811100a53b0a74e4bb8e010
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522611"
---
# <a name="suggestionsviewoptions"></a>SuggestionsViewOptions

O **elemento SuggestionsViewOptions** contém as opções para obter informações de sugestão de reunião. 
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GoodThreshold](goodthreshold.md) <br/> |Especifica a porcentagem de participantes que devem ter o período de tempo aberto para o período de tempo para se qualificar como um bom tempo de reunião sugerido.  <br/> |
|[MaximumResultsByDay](maximumresultsbyday.md) <br/> |Especifica o número de horários de reunião sugeridos por dia retornados na resposta.  <br/> |
|[MaximumNonWorkHourResultsByDay](maximumnonworkhourresultsbyday.md) <br/> |Especifica o número de resultados sugeridos para horários de reunião fora das horas de trabalho regulares por dia.  <br/> |
|[MeetingDurationInMinutes](meetingdurationinminutes.md) <br/> |Especifica a duração da reunião a ser sugerida.  <br/> |
|[MinimumSuggestionQuality](minimumsuggestionquality.md) <br/> |Especifica a qualidade das sugestões de reunião a serem retornadas na resposta.  <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Identifica o período de tempo consultado para obter informações detalhadas sobre os horários de reunião sugeridos.  <br/> |
|[CurrentMeetingTime](currentmeetingtime.md) <br/> |Representa a hora de início de uma reunião que você deseja atualizar com os resultados sugeridos do horário de reunião.  <br/> |
|[GlobalObjectId](globalobjectid.md) <br/> |Esse elemento não é usado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Contém os argumentos usados para obter informações de disponibilidade do usuário. Esse é um elemento raiz.  <br/> Veja a seguir o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento não é obrigatório e só pode ocorrer uma vez se usado. Esse valor pode ser nulo se o valor do [elemento FreeBusyViewOptions](freebusyviewoptions.md) não for nulo. 
  
> [!NOTE]
> O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserAvailability](getuseravailability-operation.md)


[Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

