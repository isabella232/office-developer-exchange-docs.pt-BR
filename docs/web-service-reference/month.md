---
title: Mês
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: b12ac64f-b230-4573-be05-c86a428c4965
description: O elemento de mês representa o mês de transição do ano para e de período padrão e o horário de verão.
ms.openlocfilehash: 73d052ef16bc51cd574eb8b04e21546f97347258
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824476"
---
# <a name="month"></a>Mês

O elemento de **mês** representa o mês de transição do ano para e de período padrão e o horário de verão. 
  
```xml
<Month>...</Month>
```

 **Curto**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) representado pelo elemento [Bias (UTC)](bias-utc.md) . Horário de verão em regiões onde o horário de verão é observado, esse elemento também contém informações sobre a transição para a hora padrão. <br/> <br/>  A seguir estão as expressões XPath ao elemento [StandardTime](standardtime.md) : <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Representa um deslocamento, desde o momento em relação ao UTC representado pelo [Bias (UTC)](bias-utc.md) elemento em regiões onde o horário de verão é observado. Esse elemento também contém informações sobre como ocorre a transição do horário de verão do período padrão.  <br/><br/>  A seguir estão as expressões XPath ao elemento [DaylightTime](daylighttime.md) :  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. O valor representa a posição ordinal do mês pela ocorrência e deve ser um número entre 1 e 12. Este é um tipo de dados de inteiro curto.
  
## <a name="remarks"></a>Coment�rios

Um elemento de [StandardTime](standardtime.md) que contém um elemento [DayOrder](dayorder.md) que tem um valor de 5, um elemento de **mês** que possui um valor de 10 e um elemento de [DayOfWeek (TimeZone)](dayofweek-timezone.md) que tem um valor de domingo significa que a transição da hora padrão para Horário de verão ocorre no domingo do mês décimo quinto. 
  
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

