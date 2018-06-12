---
title: DayOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOrder
api_type:
- schema
ms.assetid: 3022f839-12a2-42a9-820e-3ea585ce8657
description: O elemento DayOrder representa a enésima ocorrência do dia especificado no elemento DayOfWeek (TimeZone) que representa a data de transição de e até o período padrão e o horário de verão.
ms.openlocfilehash: 03ee678611a6cf58a7256ded67ab4d0a8a06a7ee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751708"
---
# <a name="dayorder"></a>DayOrder

O elemento **DayOrder** representa a ocorrência de _n_th do dia especificado no elemento [DayOfWeek (TimeZone)](dayofweek-timezone.md) que representa a data de transição de e até o período padrão e o horário de verão. 
  
```xml
<DayOrder>...</DayOrder>
```

**curto**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) representado pelo elemento [Bias (UTC)](bias-utc.md) .<br/><br/>Horário de verão em regiões onde o horário de verão é observado, esse elemento também contém informações sobre a transição para a hora padrão.<br/><br/>A seguir estão as expressões XPath ao elemento [StandardTime](standardtime.md) :<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Representa um deslocamento, desde o momento em relação ao UTC representado pelo [Bias (UTC)](bias-utc.md) elemento em regiões onde o horário de verão é observado.<br/><br/>Esse elemento também contém informações sobre como ocorre a transição do horário de verão do período padrão.<br/><br/>A seguir estão as expressões XPath ao elemento [DaylightTime](daylighttime.md) :<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. O valor para o elemento **DayOrder** pode ser de 1 a 5. O valor máximo para esse elemento pode ser 4 ou 5, dependendo do mês e ano. 
  
## <a name="remarks"></a>Coment�rios

Um elemento de [StandardTime](standardtime.md) que contém um elemento **DayOrder** que tem um valor de 5, um elemento de [mês](month.md) que possui um valor de 10 e um elemento de [DayOfWeek (TimeZone)](dayofweek-timezone.md) que tem um valor de domingo significa que a transição da hora padrão para Horário de verão ocorre no domingo do mês décimo quinto. 
  
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

