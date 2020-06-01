---
title: CalendarEventDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEventDetails
api_type:
- schema
ms.assetid: 2dca0192-b91b-4154-aa09-84da74e875e9
description: O elemento CalendarEventDetails fornece informações adicionais sobre um evento de calendário.
ms.openlocfilehash: 3e1dbba00bce4a1fdc53f3330527764c516890ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459060"
---
# <a name="calendareventdetails"></a>CalendarEventDetails

O elemento **CalendarEventDetails** fornece informações adicionais sobre um evento de calendário. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[CalendarEventArray](calendareventarray.md)
  
[CalendarEvent](calendarevent.md)
  
[CalendarEventDetails](calendareventdetails.md)
  
```xml
<CalendarEventDetails>
   <ID/>
   <Subject/>
   <Location/>
   <IsMeeting/>
   <IsRecurring/>
   <IsException/>
   <IsReminderSet/>
   <IsPrivate/>
</CalendarEventDetails>
```

 **CalendarEventDetails**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ID](id.md) <br/> |Representa a identificação de entrada do item do calendário.  <br/> |
|[Assunto (CalendarEventDetails)](subject-calendareventdetails.md) <br/> |Representa o assunto do item de calendário.  <br/> |
|[Local (CalendarEventDetails)](location-calendareventdetails.md) <br/> |Representa o campo local do item do calendário.  <br/> |
|[Iscumprimento (CalendarEventDetails)](ismeeting-calendareventdetails.md) <br/> |Indica se o evento de calendário é uma reunião ou um compromisso.  <br/> |
|[IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) <br/> |Indica se o evento de calendário é uma instância de um item de calendário recorrente ou de um único item de calendário.  <br/> |
|[IsException](isexception.md) <br/> |Indica se uma instância de um item de calendário recorrente é alterada do mestre.  <br/> |
|[ReminderSet](isreminderset.md) <br/> |Indica se um lembrete foi definido para o evento de calendário.  <br/> |
|[IsPrivate](isprivate.md) <br/> |Indica se o item de calendário é privado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarEvent](calendarevent.md) <br/> |Representa uma ocorrência de item de calendário exclusivo.  <br/> A seguir está a expressão XPath 2,0 para este elemento:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="remarks"></a>Comentários

Todos os elementos filho são listados na sequência em que ocorrem. 
  
Se o elemento [IsPrivate](isprivate.md) for **true**, todos os outros elementos no elemento [CalendarEventDetails](calendareventdetails.md) não serão retornados na resposta. 
  
A operação GetUserAvailability não retorna informações detalhadas do chamador, a menos que o chamador tenha acesso de leitura no calendário do usuário de destino. Você pode definir permissões de acesso usando o Shell de gerenciamento do Exchange.
  
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

