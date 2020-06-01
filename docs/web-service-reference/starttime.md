---
title: StartTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTime
api_type:
- schema
ms.assetid: 1fac7937-7a06-4d66-9d2a-14423bcb3b37
description: O elemento StartTime representa o início de um período de tempo.
ms.openlocfilehash: 16bee698b65dc512a709e2af9ddfe8629347fee3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458562"
---
# <a name="starttime"></a>StartTime

O elemento **StartTime** representa o início de um período de tempo. 
  
```xml
<StartTime/
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
|[TimeWindow](timewindow.md) <br/> |Identifica o intervalo de tempo consultado para as informações de disponibilidade do usuário.  <br/><br/> A seguir está a expressão XPath para este elemento:  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Identifica o período de tempo que é consultado para informações detalhadas sobre os horários de reunião sugeridos.  <br/><br/> A seguir está a expressão XPath para este elemento: <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[Duração (UserOofSettings)](duration-useroofsettings.md) <br/> | Especifica a duração para a qual o status de ausência temporária (OOF) é habilitado se o elemento [OofState](oofstate.md) estiver definido como **agendado**.  <br/><br/>  A seguir estão as possíveis expressões XPath para este elemento: <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[CalendarEvent](calendarevent.md) <br/> |Representa uma ocorrência de item de calendário exclusivo. Isso é usado para consultas de disponibilidade. O elemento **StartTime** é necessário no elemento **CalendarEvent** . O elemento **StartTime** no elemento **CalendarEvent** é exclusivo para o tipo **CalendarEvent** , embora contenha os mesmos valores de faceta que os elementos **StartTime** no tipo de **duração** contêm.  <br/><br/> A seguir está a expressão XPath para este elemento:  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório.
  
## <a name="remarks"></a>Comentários

O elemento [EndTime](endtime.md) representa o final do intervalo de tempo. 
  
O esquema inclui muitos elementos [StartTime](starttime.md) . 
  
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

