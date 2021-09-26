---
title: DayOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DayOrder
api_type:
- schema
ms.assetid: 3022f839-12a2-42a9-820e-3ea585ce8657
description: O elemento DayOrder representa a nth ocorrência do dia especificado no elemento DayOfWeek (TimeZone) que representa a data de transição de e para a hora padrão e o horário de verão.
ms.openlocfilehash: bc216984a92fef58ac6f46dc4646a0deca837563
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543440"
---
# <a name="dayorder"></a>DayOrder

O **elemento DayOrder** representa a _n_th do dia especificado no elemento [DayOfWeek (TimeZone)](dayofweek-timezone.md) que representa a data de transição de e para a hora padrão e o horário de verão. 
  
```xml
<DayOrder>...</DayOrder>
```

**short**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Representa um deslocamento do tempo em relação ao TEMPO Universal Coordenado (UTC) representado pelo elemento [Bias (UTC).](bias-utc.md)<br/><br/>Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão em regiões onde o horário de verão é observado.<br/><br/>Veja a seguir as expressões XPath para o [elemento StandardTime:](standardtime.md)<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Representa um deslocamento do tempo em relação ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) em regiões onde o horário de verão é observado.<br/><br/>Esse elemento também contém informações sobre quando ocorre a transição para o horário de verão do horário padrão.<br/><br/>Veja a seguir as expressões XPath para o [elemento DaylightTime:](daylighttime.md)<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. O valor do **elemento DayOrder** pode ser de 1 a 5. O valor máximo para esse elemento pode ser 4 ou 5, dependendo do mês e do ano. 
  
## <a name="remarks"></a>Comentários

Um elemento [StandardTime](standardtime.md) que contém um elemento **DayOrder** que tem um valor de 5, um elemento [Month](month.md) que tem um valor 10 e um elemento [DayOfWeek (TimeZone)](dayofweek-timezone.md) que tem um valor de domingo significa que a transição do horário padrão para o horário de verão ocorre no quinto domingo do décimo mês. 
  
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

