---
title: DayOfWeek (TimeZone)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 416e8892-ebb1-4fac-82cf-e27549a6c175
description: O elemento DayOfWeek representa o dia da semana em que ocorre a transição de fuso horário.
ms.openlocfilehash: 5b51a3692a1836d2d2448df88b0ec07ccf1d79a5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519895"
---
# <a name="dayofweek-timezone"></a>DayOfWeek (TimeZone)

O **elemento DayOfWeek** representa o dia da semana em que ocorre a transição de fuso horário. 
  
```xml
<DayOfWeek>...</DayOfWeek>
```

**DayOfWeekType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Representa um deslocamento do tempo em relação ao TEMPO Universal Coordenado (UTC) representado pelo elemento [Bias (UTC).](bias-utc.md)<br/><br/>Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão em regiões onde o horário de verão é observado.<br/><br/>Veja a seguir as expressões XPath para este elemento:<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Representa um deslocamento do tempo em relação ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) em regiões onde o horário de verão é observado.<br/><br/>Esse elemento também contém informações sobre quando ocorre a transição para o horário de verão do horário padrão.<br/><br/>Veja a seguir as expressões XPath para este elemento:<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Representa uma transição de fuso horário que ocorre no mesmo dia a cada ano.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. O valor do texto é representado por uma enumeração que tem os seguintes valores possíveis:
  
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

Um elemento [StandardTime](standardtime.md) que contém um elemento [DayOrder](dayorder.md) que tem um valor 5, um elemento [Month](month.md) que tem um valor 10 e um elemento **DayOfWeek** que tem um valor de domingo significa que a transição do horário padrão para o horário de verão ocorre no quinto domingo do décimo mês. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
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

