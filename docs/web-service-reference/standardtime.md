---
title: StandardTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StandardTime
api_type:
- schema
ms.assetid: 13084726-ab24-4009-be99-c4a4273c9e05
description: O elemento StandardTime representa um deslocamento do tempo relativo ao UTC (tempo Universal Coordenado) que é representado pelo elemento Bias (UTC). Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão nas regiões nas quais o horário de verão é observado.
ms.openlocfilehash: 793f058840d4fd9216f03e660f5be0f7564906cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456399"
---
# <a name="standardtime"></a>StandardTime

O elemento **StandardTime** representa um deslocamento do tempo relativo ao UTC (tempo Universal Coordenado) que é representado pelo elemento [Bias (UTC)](bias-utc.md) . Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão nas regiões nas quais o horário de verão é observado. 
  
- [Fuso horário (disponibilidade)](timezone-availability.md)
- [StandardTime](standardtime.md)
  
```xml
<StandardTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</StandardTime>
```

 **SerializableTimeZoneTime**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Bias](bias.md) <br/> |Representa o deslocamento do deslocamento UTC identificado pelo elemento [Bias (UTC)](bias-utc.md) para horário padrão e horário de verão. Este valor está em minutos.  <br/> |
|[Time](time.md) <br/> |Representa o horário de transição do dia para e a partir do horário padrão e do horário de verão.  <br/> |
|[DayOrder](dayorder.md) <br/> |Representa a _n_th ocorrência do dia que é especificada no elemento [DayOfWeek (TimeZone)](dayofweek-timezone.md) que representa a data de transição de e para o horário padrão e o horário de verão.  <br/> |
|[Month](month.md) <br/> |Representa o mês de transição do ano de e para hora padrão e horário de verão.  <br/> |
|[DayOfWeek (fuso horário)](dayofweek-timezone.md) <br/> |Representa o dia da semana em que ocorre a transição para e a hora padrão e o horário de verão.  <br/> |
|[Year](year.md) <br/> |Define um fuso horário que muda dependendo do ano. Este elemento é opcional. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Fuso horário (disponibilidade)](timezone-availability.md) <br/> | Contém elementos que identificam informações de fuso horário. Esse elemento também contém informações sobre a transição entre o horário padrão e o horário de verão. <br/><br/>A seguir estão as expressões XPath para este elemento: <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/> <br/> `/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="remarks"></a>Comentários

O elemento **StandardTime** representa um tempo de deslocamento que é representado pelo elemento [Bias (UTC)](bias-utc.md) . Quando o elemento de [polar](bias.md) filho é igual a 0, o horário padrão é igual ao deslocamento de polaridade do UTC que é representado pelo elemento [Bias (UTC)](bias-utc.md) . 
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra uma região onde o horário de verão é observado. A transição do horário de verão para o horário padrão é observada às 6:00 no quinto domingo do décimo mês.
  
```xml
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>5</DayOrder>
    <Month>10</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>4</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
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

