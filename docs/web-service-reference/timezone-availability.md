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
description: O elemento TimeZone contém elementos que identificam as informações de fuso horário. Esse elemento também contém informações sobre a transição entre o período padrão e o horário de verão.
ms.openlocfilehash: dc2466e8039819edc82294ff05f1746ada64cb43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837765"
---
# <a name="timezone-availability"></a>Fuso horário (disponibilidade)

O elemento **TimeZone** contém elementos que identificam as informações de fuso horário. Esse elemento também contém informações sobre a transição entre o período padrão e o horário de verão. 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 **SerializableTimeZone**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Bias (UTC)](bias-utc.md) <br/> |Representa o deslocamento geral do tempo Universal Coordenado (UTC). Este valor está em minutos.  <br/> |
|[StandardTime](standardtime.md) <br/> |Representa um deslocamento, desde o momento em relação ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) . Horário de verão em regiões onde o horário de verão é observado, esse elemento também contém informações sobre a transição para a hora padrão.  <br/> |
|[DaylightTime](daylighttime.md) <br/> |Representa um deslocamento, desde o momento em relação ao UTC representado pelo [Bias (UTC)](bias-utc.md) elemento em regiões onde o horário de verão é observado. Esse elemento também contém informações sobre como ocorre a transição do horário de verão do período padrão.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Contém os argumentos usados para obter informações de disponibilidade do usuário. Este é um elemento raiz.  <br/> O elemento de **fuso horário** na mensagem GetUserAvailabilityRequest representa o fuso horário em que os valores de data/hora na solicitação são especificados. Os valores de data/hora retornados pelo serviço de disponibilidade também estão neste fuso horário.  <br/> Este é o XPath a este elemento:  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |Representa as configurações de fuso horário e o horário de trabalho para o usuário de caixa de correio solicitada.  <br/> O elemento de **fuso horário** na mensagem GetUserAvailabilityResponse representa as configurações de fuso horário do usuário da caixa de correio solicitada.  <br/> Este é o XPath a este elemento:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a>Coment�rios

Esse elemento é necessário no elemento [GetUserAvailabilityRequest](getuseravailabilityrequest.md) . Esse elemento ocorre no máximo uma vez ou menos zero vezes quando o elemento pai é o elemento [WorkingHours](workinghours-ex15websvcsotherref.md) . 
  
## <a name="example"></a>Example

O exemplo a seguir mostra a parte de uma solicitação XML que identifica um deslocamento do UTC de 8 horas no aplicativo cliente.
  
```XML
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetUserAvailability](getuseravailability-operation.md)
  
[Bias](bias.md)


[Obtenção de disponibilidade do usuário](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

