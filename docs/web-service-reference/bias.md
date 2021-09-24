---
title: Bias
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Bias
api_type:
- schema
ms.assetid: ae10aa44-e6d3-483d-a3e6-bb9c45966810
description: O elemento Bias representa o deslocamento do deslocamento do tempo universal coordenado (UTC) identificado pelo elemento Bias (UTC) para horário padrão e horário de verão. Este valor está em minutos.
ms.openlocfilehash: 557605380dbda8c980272edcf445bb8099e14ada
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516094"
---
# <a name="bias"></a>Bias

O **elemento Bias** representa o deslocamento do deslocamento do tempo universal coordenado (UTC) identificado pelo elemento Bias [(UTC)](bias-utc.md) para horário padrão e horário de verão. Este valor está em minutos. 
  
```xml
<Bias>...</Bias>
```

**int**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Representa um deslocamento do tempo em relação ao UTC representado pelo elemento [Bias (UTC).](bias-utc.md) Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão em regiões onde o horário de verão é observado.<br/><br/>Veja a seguir as expressões XPath para o [elemento StandardTime:](standardtime.md)<br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Representa um deslocamento do tempo em relação ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) em regiões onde o horário de verão é observado. Esse elemento também contém informações sobre quando ocorre a transição para o horário de verão do horário padrão.  <br/><br/>Veja a seguir as expressões XPath para o [elemento DaylightTime:](daylighttime.md)<br/><br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. O valor de texto representa um inteiro.
  
## <a name="remarks"></a>Comentários

O deslocamento usado para determinar a hora local só pode ser fornecido por um dos elementos **Bias.** A soma dos valores do elemento Bias fornecidos pelo elemento [DaylightTime](daylighttime.md) ou pelo [elemento StandardTime](standardtime.md) mais o elemento [Bias (UTC)](bias-utc.md) identifica a hora local. 
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra parte de uma solicitação XML que identifica um usuário que observa o horário de verão ajustando o deslocamento do UTC em -60 minutos. Isso efetivamente faz com que o viés 420 minutos do UTC.
  
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

