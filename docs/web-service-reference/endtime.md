---
title: EndTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTime
api_type:
- schema
ms.assetid: 82e4ef4f-a557-4044-b9b7-d91622f4ac55
description: O elemento EndTime representa o final de um intervalo de tempo.
ms.openlocfilehash: 5a30b32ecfeafe582cd07dd662aacb0a960257c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462989"
---
# <a name="endtime"></a>EndTime

O elemento **EndTime** representa o final de um intervalo de tempo. 
  
```xml
<EndTime>dateTime</EndTime>
```

 **dateTime**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TimeWindow](timewindow.md) <br/> |Identifica o intervalo de tempo consultado para as informações de disponibilidade do usuário.<br/><br/> A seguir está a expressão XPath para este elemento:<br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Identifica o período de tempo que é consultado para informações detalhadas sobre os horários de reunião sugeridos.<br/><br/> A seguir está a expressão XPath para este elemento:<br/><br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.  <br/> |
|[Duração (UserOofSettings)](duration-useroofsettings.md) <br/> | Especifica a duração para a qual o status de ausência temporária (OOF) é habilitado se o elemento [OofState](oofstate.md) estiver definido como **agendado**.  <br/><br/>  A seguir estão as possíveis expressões XPath para este elemento:<br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[Ocorrência](occurrence.md) <br/> |Representa uma única ocorrência modificada de um item de calendário recorrente.  <br/> |
|[CalendarEvent](calendarevent.md) <br/> |Representa uma ocorrência de item de calendário exclusivo. Isso é usado para consultas de disponibilidade. O elemento **EndTime** é necessário no elemento **CalendarEvent** . O elemento **EndTime** no elemento **CalendarEvent** é exclusivo para o tipo **CalendarEvent** .<br/><br/> A seguir está a expressão XPath para este elemento:<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório.
  
## <a name="remarks"></a>Comentários

O elemento [StartTime](starttime.md) representa o início de um período de tempo. 
  
A hora de término representa o horário do cliente.
  
O esquema inclui muitos elementos [EndTime](endtime.md) . 
  
> [!NOTE]
> O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [Obtendo disponibilidade do usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

