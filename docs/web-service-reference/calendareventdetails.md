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
ms.openlocfilehash: 8df4f3ed4f66c7dcba00e1f0c5b0c383075da0a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751349"
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ID DO](id.md) <br/> |Representa a identificação de entrada do item do calendário.  <br/> |
|[Assunto (CalendarEventDetails)](subject-calendareventdetails.md) <br/> |Representa o assunto do item de calendário.  <br/> |
|[Local (CalendarEventDetails)](location-calendareventdetails.md) <br/> |Representa o campo de localização do item de calendário.  <br/> |
|[IsMeeting (CalendarEventDetails)](ismeeting-calendareventdetails.md) <br/> |Indica se o evento de calendário é uma reunião ou um compromisso.  <br/> |
|[IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) <br/> |Indica se o evento de calendário é uma instância de um item de calendário recorrente ou um item de calendário único.  <br/> |
|[IsException](isexception.md) <br/> |Indica se uma instância de um item de calendário recorrente é alterada do mestre.  <br/> |
|[IsReminderSet](isreminderset.md) <br/> |Indica se um lembrete tiver sido definido para o evento de calendário.  <br/> |
|[IsPrivate](isprivate.md) <br/> |Indica se o item do calendário é privado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarEvent](calendarevent.md) <br/> |Representa uma ocorrência de item de calendário exclusivo.  <br/> Este é a expressão XPath 2.0 para esse elemento:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="remarks"></a>Coment�rios

Todos os elementos filhos são listados na sequência em que ocorrem. 
  
Se o elemento [IsPrivate](isprivate.md) for **true**, todos os outros elementos no elemento [CalendarEventDetails](calendareventdetails.md) não são retornados na resposta. 
  
A operação GetUserAvailability não retorna informações detalhadas do chamador, a menos que o chamador tem acesso de leitura no calendário do usuário de destino. Você pode definir permissões de acesso usando o Shell de gerenciamento do Exchange.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Obtenção de disponibilidade do usuário](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

