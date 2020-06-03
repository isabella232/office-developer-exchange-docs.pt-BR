---
title: Fuso horário (disponibilidade)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZone
api_type:
- schema
ms.assetid: d662ffae-1f93-4c08-85a4-c69de2f7c681
description: O elemento TimeZone contém elementos que identificam informações de fuso horário. Esse elemento também contém informações sobre a transição entre o horário padrão e o horário de verão.
ms.openlocfilehash: ba4b0a4805dba54450e01e89c5e9ef746404b716
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460271"
---
# <a name="timezone-availability"></a>Fuso horário (disponibilidade)

O elemento **timezone** contém elementos que identificam informações de fuso horário. Esse elemento também contém informações sobre a transição entre o horário padrão e o horário de verão. 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 **SerializableTimeZone**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Bias (UTC)](bias-utc.md) <br/> |Representa o deslocamento geral do tempo universal coordenado (UTC). Este valor está em minutos.  <br/> |
|[StandardTime](standardtime.md) <br/> |Representa um deslocamento do tempo relativo ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) . Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão nas regiões nas quais o horário de verão é observado.  <br/> |
|[DaylightTime](daylighttime.md) <br/> |Representa um deslocamento do tempo relativo ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) nas regiões em que o horário de verão é observado. Esse elemento também contém informações sobre quando ocorre a transição para o horário de Verão do horário padrão.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Contém os argumentos usados para obter informações de disponibilidade do usuário. Este é um elemento raiz.  <br/> O elemento **timezone** na mensagem GetUserAvailabilityRequest representa o fuso horário em que os valores DateTime da solicitação são especificados. Os valores DateTime retornados pelo serviço de disponibilidade também estão neste fuso horário.  <br/> Este é o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |Representa as configurações de fuso horário e as horas de trabalho do usuário de caixa de correio solicitado.  <br/> O elemento **timezone** na mensagem GetUserAvailabilityResponse representa as configurações de fuso horário do usuário de caixa de correio solicitado.  <br/> Este é o XPath para este elemento:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento é obrigatório no elemento [GetUserAvailabilityRequest](getuseravailabilityrequest.md) . Esse elemento ocorre no máximo uma vez ou pelo menos zero vezes quando o elemento pai é o elemento [WorkingHours](workinghours-ex15websvcsotherref.md) . 
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra parte de uma solicitação XML que identifica um deslocamento do UTC de 8 horas no aplicativo cliente.
  
```XML
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>11</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>2</DayOrder>
    <Month>3</Month>
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



[Operação GetUserAvailability](getuseravailability-operation.md)
  
[Bias](bias.md)


[Obtendo disponibilidade do usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

