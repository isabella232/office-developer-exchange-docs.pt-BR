---
title: Hora
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Time
api_type:
- schema
ms.assetid: c4b98be7-141c-4ba8-97ef-9ad1ed19f61f
description: O elemento Time representa a hora de transição do dia de e para a hora padrão e o horário de verão.
ms.openlocfilehash: d9cd83a7dcb0a296693e3daa1874b12294de5857
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513266"
---
# <a name="time"></a>Time

O **elemento Time** representa a hora de transição do dia de e para a hora padrão e o horário de verão. 
  
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
|[StandardTime](standardtime.md) <br/> | Representa um deslocamento do tempo em relação ao TEMPO Universal Coordenado (UTC) representado pelo elemento [Bias (UTC).](bias-utc.md) Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão em regiões onde o horário de verão é observado.  <br/><br/>  Veja a seguir as expressões XPath para o [elemento StandardTime:](standardtime.md) <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Representa um deslocamento do tempo em relação ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) em regiões onde o horário de verão é observado. Esse elemento também contém informações sobre quando ocorre a transição para o horário de verão do horário padrão.  <br/><br/>  Veja a seguir as expressões XPath para o [elemento DaylightTime:](daylighttime.md)  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor do texto representa horas, minutos e segundos no seguinte formato: hh:mm:ss.
  
## <a name="remarks"></a>Comentários

Quando o **elemento Time** ocorre no elemento [DaylightTime,](daylighttime.md) ele representa a hora do dia em que ocorre a transição do horário de verão para o horário padrão. Quando o [elemento Time](time.md) ocorre no [elemento StandardTime,](standardtime.md) ele representa a hora do dia em que ocorre a transição do horário padrão para o horário de verão. 
  
Esse elemento tem uma ocorrência mínima de zero e uma ocorrência máxima de um.
  
## <a name="example"></a>Exemplo

A parte a seguir de uma solicitação representa um tempo de transição de 2 da manhã. do horário padrão para o horário de verão.
  
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
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

