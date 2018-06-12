---
title: Bias
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bias
api_type:
- schema
ms.assetid: ae10aa44-e6d3-483d-a3e6-bb9c45966810
description: O elemento Bias representa o deslocamento do deslocamento de tempo Universal Coordenado (UTC) identificado pelo elemento Bias (UTC) para o período padrão e o horário de verão. Este valor está em minutos.
ms.openlocfilehash: 770bf97b030ac1293595560bc269f54896e35a15
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751273"
---
# <a name="bias"></a>Bias

O elemento **Bias** representa o deslocamento do deslocamento de tempo Universal Coordenado (UTC) identificado pelo elemento [Bias (UTC)](bias-utc.md) para o período padrão e o horário de verão. Este valor está em minutos. 
  
```xml
<Bias>...</Bias>
```

**int**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Representa um deslocamento, desde o momento em relação ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) . Horário de verão em regiões onde o horário de verão é observado, esse elemento também contém informações sobre a transição para a hora padrão.<br/><br/>A seguir estão as expressões XPath ao elemento [StandardTime](standardtime.md) :<br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Representa um deslocamento, desde o momento em relação ao UTC representado pelo [Bias (UTC)](bias-utc.md) elemento em regiões onde o horário de verão é observado. Esse elemento também contém informações sobre como ocorre a transição do horário de verão do período padrão.  <br/><br/>A seguir estão as expressões XPath ao elemento [DaylightTime](daylighttime.md) :<br/><br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. O valor de texto representa um número inteiro.
  
## <a name="remarks"></a>Coment�rios

O deslocamento usado para determinar a hora local só pode ser fornecido por um dos elementos **Bias** . A soma dos valores do elemento Bias fornecido pelo elemento [DaylightTime](daylighttime.md) ou o elemento [StandardTime](standardtime.md) mais o elemento [Bias (UTC)](bias-utc.md) identifica a hora local. 
  
## <a name="example"></a>Example

O exemplo a seguir mostra a parte de uma solicitação XML que identifica um usuário que tiver o horário de verão, ajustando o deslocamento do UTC por 60 minutos. Isso efetivamente torna o bias 420 minutos de UTC.
  
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

