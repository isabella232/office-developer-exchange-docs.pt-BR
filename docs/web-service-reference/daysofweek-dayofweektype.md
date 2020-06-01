---
title: DaysOfWeek (DayOfWeektype)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaysOfWeek
api_type:
- schema
ms.assetid: ba8f990d-d37d-403d-b31f-55e5208c8ad5
description: O elemento DaysOfWeek descreve os dias da semana usados nos padrões de recorrência do item.
ms.openlocfilehash: 44552350679df1fec3d237d9b09f1a5feb9cc4b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458821"
---
# <a name="daysofweek-dayofweektype"></a>DaysOfWeek (DayOfWeektype)

O elemento **DaysOfWeek** descreve os dias da semana usados nos padrões de recorrência do item. 
  
```xml
<DaysOfWeek/>
```

**DayOfWeektype**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Descreve um padrão relativo de recorrência anual.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Descreve um padrão relativo de recorrência mensal.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. Veja a seguir os valores possíveis:
  
- Domingo    
- Segunda-feira    
- Terça-feira   
- Quarta-feira    
- Quinta-feira    
- Sexta-feira    
- Sábado    
- Day (não usado no TimeChangePatternTypes)    
- WEEKDAY (não usado no TimeChangePatternTypes)    
- WeekendDay (não usado no TimeChangePatternTypes)
    
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

