---
title: DayOfWeek (fuso horário)
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
ms.openlocfilehash: 7bc05f417268ccfb20adae12e2694d8360023ab2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457841"
---
# <a name="dayofweek-timezone"></a>DayOfWeek (fuso horário)

O elemento **DayOfWeek** representa o dia da semana em que ocorre a transição de fuso horário. 
  
```xml
<DayOfWeek>...</DayOfWeek>
```

**DayOfWeektype**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Representa um deslocamento do tempo relativo ao UTC (tempo Universal Coordenado) representado pelo elemento [Bias (UTC)](bias-utc.md) .<br/><br/>Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão nas regiões nas quais o horário de verão é observado.<br/><br/>A seguir estão as expressões XPath para este elemento:<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Representa um deslocamento do tempo relativo ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) nas regiões em que o horário de verão é observado.<br/><br/>Esse elemento também contém informações sobre quando ocorre a transição para o horário de Verão do horário padrão.<br/><br/>A seguir estão as expressões XPath para este elemento:<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Representa uma transição de fuso horário que ocorre no mesmo dia a cada ano.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. O valor de texto é representado por uma enumeração que tem os seguintes valores possíveis:
  
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

Um elemento [StandardTime](standardtime.md) que contém um elemento [DayOrder](dayorder.md) que tem um valor de 5, um elemento [month](month.md) que tem um valor de 10, e um elemento **DayOfWeek** que tem um valor de domingo significa que a transição do horário padrão para o horário de Verão ocorre no quinto domingo do décimo mês. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
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

