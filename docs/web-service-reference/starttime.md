---
title: StartTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StartTime
api_type:
- schema
ms.assetid: 1fac7937-7a06-4d66-9d2a-14423bcb3b37
description: O elemento StartTime representa o início de um intervalo de tempo.
ms.openlocfilehash: e6d9034fa1b01f0f0969837761f4da7c36cea752
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531650"
---
# <a name="starttime"></a>StartTime

O **elemento StartTime** representa o início de um intervalo de tempo. 
  
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
|[TimeWindow](timewindow.md) <br/> |Identifica o período de tempo consultado para as informações de disponibilidade do usuário.  <br/><br/> Veja a seguir a expressão XPath para este elemento:  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Identifica o período de tempo consultado para obter informações detalhadas sobre os horários de reunião sugeridos.  <br/><br/> Veja a seguir a expressão XPath para este elemento: <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[Duration (UserOofSettings)](duration-useroofsettings.md) <br/> | Especifica a duração para a qual o status De Office (OOF) está habilitado se o elemento [OofState](oofstate.md) estiver definido como **Scheduled**.  <br/><br/>  Veja a seguir as possíveis expressões XPath para este elemento: <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[CalendarEvent](calendarevent.md) <br/> |Representa uma ocorrência de item de calendário exclusiva. Isso é usado para consultas de disponibilidade. O **elemento StartTime** é necessário no **elemento CalendarEvent.** O **elemento StartTime** no **elemento CalendarEvent** é exclusivo do tipo **CalendarEvent,** embora contenha os mesmos valores de faceta que os elementos **StartTime** no tipo **Duration** contêm.  <br/><br/> Veja a seguir a expressão XPath para este elemento:  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário.
  
## <a name="remarks"></a>Comentários

O [elemento EndTime](endtime.md) representa o fim do intervalo de tempo. 
  
O esquema inclui muitos elementos [StartTime.](starttime.md) 
  
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

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

