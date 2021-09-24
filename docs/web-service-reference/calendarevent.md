---
title: CalendarEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarEvent
api_type:
- schema
ms.assetid: 91958c01-1fcb-4ac0-8601-5e5b434c988a
description: O elemento CalendarEvent representa uma ocorrência de item de calendário exclusiva.
ms.openlocfilehash: fd57517595659f2081c82fe9f4665ce2c39059fe
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514820"
---
# <a name="calendarevent"></a>CalendarEvent

O **elemento CalendarEvent** representa uma ocorrência de item de calendário exclusiva. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[CalendarEventArray](calendareventarray.md)
  
[CalendarEvent](calendarevent.md)
  
```xml
<CalendarEvent>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
   <BusyType>...</BusyType>
   <CalendarEventDetails>...</CalendarEventDetails>
</CalendarEvent>
```

 **CalendarEvent**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |Representa o início de um evento de calendário. Esse é um elemento filho necessário.  <br/> |
|[EndTime](endtime.md) <br/> |Representa o fim de um evento de calendário. Esse é um elemento filho necessário.  <br/> |
|[BusyType](busytype.md) <br/> |Representa o conjunto de status de ocupado/livre para um evento de calendário. Esse é um elemento filho necessário.  <br/> |
|[CalendarEventDetails](calendareventdetails.md) <br/> |Fornece informações adicionais para um evento de calendário. Este é um elemento filho opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarEventArray](calendareventarray.md) <br/> |Contém um conjunto de ocorrências de item de calendário exclusivas que representam a disponibilidade do usuário solicitado.  <br/> Veja a seguir a expressão XPath 2.0 para este elemento:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray` <br/> |
   
## <a name="remarks"></a>Comentários

Os horários de compromisso e de reunião são retornados no fuso horário do cliente. Todos os elementos filho são listados na sequência em que ocorrem. O nível de detalhes fornecido por esse elemento depende das permissões concedidas ao solicitante.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

