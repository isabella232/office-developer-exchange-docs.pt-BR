---
title: Interval
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Interval
api_type:
- schema
ms.assetid: d0c97a5f-96be-40c6-b7d4-abf4c3870adf
description: O elemento Interval define o intervalo entre dois itens recorrentes consecutivos.
ms.openlocfilehash: 6df46865d7a89a0bfde9afc5f84ffdb78d956a30
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541025"
---
# <a name="interval"></a>Interval

O **elemento Interval** define o intervalo entre dois itens recorrentes consecutivos. 
  
```xml
<Interval/>
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
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |Representa um padrão de recorrência mensal.  <br/> |
|[DailyRegeneration](dailyregeneration.md) <br/> |Descreve a frequência, em dias, em que uma tarefa é regenerada.  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |Descreve a frequência, em dias, na qual uma tarefa é recorrência.  <br/> |
|[MonthlyRegeneration](monthlyregeneration.md) <br/> |Descreve a frequência, em meses, na qual uma tarefa é regenerada.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Descreve um padrão mensal relativo para uma tarefa recorrente.  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Descreve a frequência, em semanas, em que e os dias em que uma tarefa é recorrência.  <br/> |
|[WeeklyRegeneration](weeklyregeneration.md) <br/> |Descreve a frequência, em semanas, na qual uma tarefa é regenerada.  <br/> |
|[YearlyRegeneration](yearlyregeneration.md) <br/> |Descreve a frequência, em anos, na qual uma tarefa é regenerada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um inteiro é necessário.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

