---
title: TimeZone (Availability)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeZone
api_type:
- schema
ms.assetid: d662ffae-1f93-4c08-85a4-c69de2f7c681
description: O elemento TimeZone contém elementos que identificam informações do fuso horário. Esse elemento também contém informações sobre a transição entre o horário padrão e o horário de verão.
ms.openlocfilehash: 7ca6f0f2d9950770055d19c04adab9b76b95c295
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538839"
---
# <a name="timezone-availability"></a>TimeZone (Availability)

O **elemento TimeZone** contém elementos que identificam informações do fuso horário. Esse elemento também contém informações sobre a transição entre o horário padrão e o horário de verão. 
  
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
|[Bias (UTC)](bias-utc.md) <br/> |Representa o deslocamento geral do TEMPO Universal Coordenado (UTC). Este valor está em minutos.  <br/> |
|[StandardTime](standardtime.md) <br/> |Representa um deslocamento do tempo em relação ao UTC representado pelo elemento [Bias (UTC).](bias-utc.md) Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão em regiões onde o horário de verão é observado.  <br/> |
|[DaylightTime](daylighttime.md) <br/> |Representa um deslocamento do tempo em relação ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) em regiões onde o horário de verão é observado. Esse elemento também contém informações sobre quando ocorre a transição para o horário de verão do horário padrão.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Contém os argumentos usados para obter informações de disponibilidade do usuário. Esse é um elemento raiz.  <br/> O **elemento TimeZone** na mensagem GetUserAvailabilityRequest representa o fuso horário no qual os valores DateTime na solicitação são especificados. Os valores DateTime retornados pelo serviço de Disponibilidade também estão nesse fuso horário.  <br/> Veja a seguir o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |Representa as configurações de fuso horário e o horário de trabalho para o usuário de caixa de correio solicitado.  <br/> O **elemento TimeZone** na mensagem GetUserAvailabilityResponse representa as configurações de fuso horário do usuário de caixa de correio solicitado.  <br/> Veja a seguir o XPath para este elemento:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento é necessário no [elemento GetUserAvailabilityRequest.](getuseravailabilityrequest.md) Esse elemento ocorre no máximo uma vez ou pelo menos zero vezes quando o elemento pai é o [elemento WorkingHours.](workinghours-ex15websvcsotherref.md) 
  
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
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserAvailability](getuseravailability-operation.md)
  
[Bias](bias.md)


[Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

