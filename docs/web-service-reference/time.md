---
title: Hora
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Time
api_type:
- schema
ms.assetid: c4b98be7-141c-4ba8-97ef-9ad1ed19f61f
description: O elemento time representa o horário de transição do dia para e de horário padrão e horário de verão.
ms.openlocfilehash: 97c89fbcbdb85fcdd4d32a1d44075ac42adef053
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460292"
---
# <a name="time"></a>Hora

O elemento **time** representa o horário de transição do dia para e de horário padrão e horário de verão. 
  
```xml
<Time>...</Time>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Representa um deslocamento do tempo relativo ao UTC (tempo Universal Coordenado) representado pelo elemento [Bias (UTC)](bias-utc.md) . Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão nas regiões nas quais o horário de verão é observado.  <br/><br/>  A seguir estão as expressões XPath para o elemento [StandardTime](standardtime.md) : <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Representa um deslocamento do tempo relativo ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) nas regiões em que o horário de verão é observado. Esse elemento também contém informações sobre quando ocorre a transição para o horário de Verão do horário padrão.  <br/><br/>  A seguir estão as expressões XPath para o elemento [DaylightTime](daylighttime.md) :  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa horas, minutos e segundos no seguinte formato: hh: mm: SS.
  
## <a name="remarks"></a>Comentários

Quando o elemento **time** ocorre no elemento [DaylightTime](daylighttime.md) , ele representa a hora do dia em que ocorre a transição do horário de verão para o horário padrão. Quando o elemento [time](time.md) ocorre no elemento [StandardTime](standardtime.md) , ele representa a hora do dia em que ocorre a transição do horário padrão para o horário de verão. 
  
Esse elemento tem uma ocorrência mínima de zero e uma ocorrência máxima de um.
  
## <a name="example"></a>Exemplo

A parte a seguir de uma solicitação representa um tempo de transição de 2 A.M. do horário padrão para o horário de verão.
  
```xml
<StandardTime>
   <Bias>0</Bias>
   <Time>02:00:00</Time>
   <DayOrder>5</DayOrder>
   <Month>10</Month>
   <DayOfWeek>Sunday</DayOfWeek>
</StandardTime
```

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

