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
description: O elemento Month representa o mês do ano de transição de e para hora padrão e horário de verão.
ms.openlocfilehash: f102dca4ed9e833b9742844cfd612c81dfd05e70
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468618"
---
# <a name="month"></a>Mês

O elemento **month** representa o mês do ano de transição de e para hora padrão e horário de verão. 
  
```xml
<Month>...</Month>
```

 **Rápido**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Representa um deslocamento do tempo relativo ao UTC (tempo Universal Coordenado) representado pelo elemento [Bias (UTC)](bias-utc.md) . Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão nas regiões nas quais o horário de verão é observado. <br/> <br/>  A seguir estão as expressões XPath para o elemento [StandardTime](standardtime.md) : <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Representa um deslocamento do tempo relativo ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) nas regiões em que o horário de verão é observado. Esse elemento também contém informações sobre quando ocorre a transição para o horário de Verão do horário padrão.  <br/><br/>  A seguir estão as expressões XPath para o elemento [DaylightTime](daylighttime.md) :  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. O valor representa a classificação ordinal do mês por ocorrência e deve ser um número entre 1 e 12. Este é um tipo de dados inteiro curto.
  
## <a name="remarks"></a>Comentários

Um elemento [StandardTime](standardtime.md) que contém um elemento [DayOrder](dayorder.md) que tem um valor de 5, um elemento **month** que tem um valor de 10, e um elemento [DayOfWeek (TimeZone)](dayofweek-timezone.md) que tem um valor de domingo significa que a transição do horário padrão para o horário de Verão ocorre no quinto domingo do décimo mês. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [Obtendo disponibilidade do usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

