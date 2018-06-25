---
title: DayOfWeek (TimeZone)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 416e8892-ebb1-4fac-82cf-e27549a6c175
description: O elemento DayOfWeek representa o dia da semana em que ocorre a transição de fuso horário.
ms.openlocfilehash: 7816b90000be36cf3a3354d26d978684bfdcfe40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751703"
---
# <a name="dayofweek-timezone"></a>DayOfWeek (TimeZone)

O elemento **DayOfWeek** representa o dia da semana em que ocorre a transição de fuso horário. 
  
```xml
<DayOfWeek>...</DayOfWeek>
```

**DayOfWeekType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) representado pelo elemento [Bias (UTC)](bias-utc.md) .<br/><br/>Horário de verão em regiões onde o horário de verão é observado, esse elemento também contém informações sobre a transição para a hora padrão.<br/><br/>A seguir estão as expressões XPath para esse elemento:<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Representa um deslocamento, desde o momento em relação ao UTC representado pelo [Bias (UTC)](bias-utc.md) elemento em regiões onde o horário de verão é observado.<br/><br/>Esse elemento também contém informações sobre como ocorre a transição do horário de verão do período padrão.<br/><br/>A seguir estão as expressões XPath para esse elemento:<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Representa uma transição de fuso horário que ocorre no mesmo dia cada ano.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. O valor de texto é representado por uma enumeração que tem os seguintes valores possíveis:
  
- Domingo    
- Segunda-feira    
- Terça-feira    
- Quarta-feira    
- Quinta-feira    
- Sexta-feira    
- Sábado    
- Dia    
- Dia da semana   
- WeekendDay
    
## <a name="remarks"></a>Comentários

Um elemento de [StandardTime](standardtime.md) que contém um elemento [DayOrder](dayorder.md) que tem um valor de 5, um elemento de [mês](month.md) que possui um valor de 10 e um elemento de **DayOfWeek** que tem um valor de domingo significa que a transição da hora padrão para o horário de verão economia de tempo ocorre no domingo do mês décimo quinto. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [Obtenção de disponibilidade do usuário](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

