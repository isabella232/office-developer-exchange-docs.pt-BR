---
title: Intervalo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Interval
api_type:
- schema
ms.assetid: d0c97a5f-96be-40c6-b7d4-abf4c3870adf
description: O elemento de intervalo define o intervalo entre dois itens recorrentes consecutivos.
ms.openlocfilehash: 55d26b5b1b51aca3effa93a2e6852c1ae57ef4b0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823962"
---
# <a name="interval"></a>Intervalo

O elemento de **intervalo** define o intervalo entre dois itens recorrentes consecutivos. 
  
```xml
<Interval/>
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
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |Representa um padrão de recorrência mensal.  <br/> |
|[DailyRegeneration](dailyregeneration.md) <br/> |Descreve a frequência, em dias, em que uma tarefa seja gerada novamente.  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |Descreve a frequência, em dias, em que é uma tarefa recorrente.  <br/> |
|[MonthlyRegeneration](monthlyregeneration.md) <br/> |Descreve a frequência, em meses, em que uma tarefa seja gerada novamente.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Descreve um padrão mensal relativo de uma tarefa recorrente.  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Descreve a frequência, em semanas, qual e os dias em que é uma tarefa recorrente.  <br/> |
|[WeeklyRegeneration](weeklyregeneration.md) <br/> |Descreve a frequência, em semanas, em que uma tarefa seja gerada novamente.  <br/> |
|[YearlyRegeneration](yearlyregeneration.md) <br/> |Descreve a frequência, em anos, em que uma tarefa seja gerada novamente.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto que representa um número inteiro.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

