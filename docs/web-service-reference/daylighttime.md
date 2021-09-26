---
title: DaylightTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DaylightTime
api_type:
- schema
ms.assetid: 9f551ee4-d945-477c-b981-9554b197d26d
description: O elemento DaylightTime representa um deslocamento do horário em relação ao HORÁRIO UNIVERSAL Coordenado (UTC) representado pelo elemento Bias (UTC) em regiões onde o horário de verão é observado. Esse elemento também contém informações sobre quando ocorre a transição para o horário de verão do horário padrão.
ms.openlocfilehash: 95d09fe01602f2d55d1a39dc7164a3f60a328f2a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543426"
---
# <a name="daylighttime"></a>DaylightTime

O **elemento DaylightTime** representa um deslocamento do horário em relação ao HORÁRIO UNIVERSAL Coordenado (UTC) representado pelo elemento [Bias (UTC)](bias-utc.md) em regiões onde o horário de verão é observado. Esse elemento também contém informações sobre quando ocorre a transição para o horário de verão do horário padrão. 
  
- [TimeZone (Availability)](timezone-availability.md) 
- [DaylightTime](daylighttime.md)
  
```xml
<DaylightTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</DaylightTime>
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
|[Time](time.md) <br/> |Representa a hora de transição do dia de e para a hora padrão e o horário de verão.  <br/> |
|[DayOrder](dayorder.md) <br/> |Representa a _n_th do dia especificado no elemento [DayOfWeek (TimeZone)](dayofweek-timezone.md) que representa a data de transição de e para o horário padrão e o horário de verão.  <br/> |
|[Month](month.md) <br/> |Representa o mês de transição do ano de e para a hora padrão e o horário de verão.  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |Representa o dia da semana em que ocorre a transição de e para a hora padrão e o horário de verão.  <br/> |
|[Year](year.md) <br/> |Usado para definir um fuso horário que muda dependendo do ano. Esse elemento é opcional. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TimeZone (Availability)](timezone-availability.md) <br/> | Contém elementos que identificam informações de fuso horário.<br/><br/>Esse elemento também contém informações sobre a transição entre o horário padrão e o horário de verão.<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="example"></a>Exemplo

A seguinte solicitação parcial GetUserAvailability representa um aplicativo cliente em um local que reconhece o horário de verão.
  
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
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

