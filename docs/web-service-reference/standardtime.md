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
description: O elemento StandardTime representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) que é representado por um elemento Bias (UTC). Horário de verão em regiões onde o horário de verão é observado, esse elemento também contém informações sobre a transição para a hora padrão.
ms.openlocfilehash: 726c31ffba06c1c437711b88444ec5eba45b520d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825546"
---
# <a name="standardtime"></a>StandardTime

O elemento **StandardTime** representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) que é representado por um elemento [Bias (UTC)](bias-utc.md) . Horário de verão em regiões onde o horário de verão é observado, esse elemento também contém informações sobre a transição para a hora padrão. 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Bias](bias.md) <br/> |Representa o deslocamento de deslocamento UTC é identificado pelo elemento [Bias (UTC)](bias-utc.md) para o período padrão e o horário de verão. Este valor está em minutos.  <br/> |
|[Time](time.md) <br/> |Representa a hora de transição do dia de e para período padrão e o horário de verão.  <br/> |
|[DayOrder](dayorder.md) <br/> |Representa a ocorrência de _n_th do dia em que é especificado no elemento [DayOfWeek (TimeZone)](dayofweek-timezone.md) que representa a data de transição de e até o período padrão e o horário de verão.  <br/> |
|[Month](month.md) <br/> |Representa o mês de transição do ano para e de período padrão e o horário de verão.  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |Representa o dia da semana em que ocorre a transição entre o horário padrão e o horário de verão.  <br/> |
|[Ano](year.md) <br/> |Define um fuso horário que mudam dependendo do ano. Esse elemento é opcional. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Fuso horário (disponibilidade)](timezone-availability.md) <br/> | Contém os elementos que identificam as informações de fuso horário. Esse elemento também contém informações sobre a transição entre o período padrão e o horário de verão. <br/><br/>A seguir estão as expressões XPath para esse elemento: <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/> <br/> `/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="remarks"></a>Comentários

O elemento **StandardTime** representa um tempo de deslocamento é representado por um elemento [Bias (UTC)](bias-utc.md) . Quando o elemento filho [Bias](bias.md) for igual a 0, o tempo padrão é igual ao deslocamento bias de UTC representado pelo elemento [Bias (UTC)](bias-utc.md) . 
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra uma região em que o horário de verão é observado. A transição de horário de verão para a hora padrão é observada às 2h no quinto domingo do mês décimo.
  
```xml
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

