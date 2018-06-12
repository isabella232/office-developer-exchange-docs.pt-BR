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
description: O elemento de tempo representa a hora de transição do dia de e para período padrão e o horário de verão.
ms.openlocfilehash: 716487fb7ed64dbaa6fa97caf1ea608e4673d2ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837724"
---
# <a name="time"></a>Hora

O elemento de **tempo** representa a hora de transição do dia de e para período padrão e o horário de verão. 
  
```xml
<Time>...</Time>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) representado pelo elemento [Bias (UTC)](bias-utc.md) . Horário de verão em regiões onde o horário de verão é observado, esse elemento também contém informações sobre a transição para a hora padrão.  <br/><br/>  A seguir estão as expressões XPath ao elemento [StandardTime](standardtime.md) : <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Representa um deslocamento, desde o momento em relação ao UTC representado pelo [Bias (UTC)](bias-utc.md) elemento em regiões onde o horário de verão é observado. Esse elemento também contém informações sobre como ocorre a transição do horário de verão do período padrão.  <br/><br/>  A seguir estão as expressões XPath ao elemento [DaylightTime](daylighttime.md) :  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa horas, minutos e segundos no seguinte formato: hh.
  
## <a name="remarks"></a>Coment�rios

Quando o elemento de **tempo** ocorre no elemento [DaylightTime](daylighttime.md) , ela representa a hora do dia em que ocorre a transição de horário de verão para a hora padrão. Quando o elemento de [tempo](time.md) ocorre no elemento [StandardTime](standardtime.md) , ela representa a hora do dia em que ocorre a transição da hora padrão para o horário de verão. 
  
Este elemento tem uma ocorrência mínima de zero e uma ocorrência de máxima de um.
  
## <a name="example"></a>Example

A seguinte parte de uma solicitação representa um tempo de transição de 2h da manhã da hora padrão para o horário de verão.
  
```xml
<StandardTime>
   <Bias>0</Bias>
   <Time>02:00:00</Time>
   <DayOrder>5</DayOrder>
   <Month>10</Month>
   <DayOfWeek>Sunday</DayOfWeek>
</StandardTime
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

