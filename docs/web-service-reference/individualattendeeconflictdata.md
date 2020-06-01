---
title: IndividualAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndividualAttendeeConflictData
api_type:
- schema
ms.assetid: d45d3c34-abe1-40da-afd3-23bc5c3ef474
description: O elemento IndividualAttendeeConflictData contém o status de disponibilidade de um usuário ou contato para uma janela de tempo que ocorre ao mesmo tempo que o tempo de reunião sugerido identificado no elemento Suggestion.
ms.openlocfilehash: 55210230259b78e5ed9c4f0744aae003cf2e7ae5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459311"
---
# <a name="individualattendeeconflictdata"></a>IndividualAttendeeConflictData

O elemento **IndividualAttendeeConflictData** contém o status de disponibilidade de um usuário ou contato para uma janela de tempo que ocorre ao mesmo tempo que o tempo de reunião sugerido identificado no elemento [suggestion](suggestion.md) . 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[SuggestionsResponse](suggestionsresponse.md)
  
[SuggestionDayResultArray](suggestiondayresultarray.md)
  
[SuggestionDayResult](suggestiondayresult.md)
  
[SuggestionArray](suggestionarray.md)
  
[La](suggestion.md)
  
[AttendeeConflictDataArray](attendeeconflictdataarray.md)
  
[IndividualAttendeeConflictData](individualattendeeconflictdata.md)
  
```xml
<IndividualAttendeeConflictData>
   <BusyType>...</BusyType>
</IndividualAttendeeConflictData>
```

 **IndividualAttendeeConflictData**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[BusyType](busytype.md) <br/> |Representa o status de disponibilidade de um usuário para um tempo de reunião sugerido.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AttendeeConflictDataArray](attendeeconflictdataarray.md) <br/> |Contém uma matriz de dados de conflito para participantes identificados no [GetUserAvailabilityRequest](getuseravailabilityrequest.md).  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Obtendo disponibilidade do usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

