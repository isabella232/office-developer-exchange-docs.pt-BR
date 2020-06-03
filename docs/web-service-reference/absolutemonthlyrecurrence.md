---
title: AbsoluteMonthlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteMonthlyRecurrence
api_type:
- schema
ms.assetid: 178fa0ae-9dfc-417f-933c-d657d31c2161
description: O elemento AbsoluteMonthlyRecurrence representa um padrão de recorrência mensal.
ms.openlocfilehash: 3176cd30a1cfe7b2310f960ce377ab7a277e795a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460432"
---
# <a name="absolutemonthlyrecurrence"></a>AbsoluteMonthlyRecurrence

O elemento **AbsoluteMonthlyRecurrence** representa um padrão de recorrência mensal. 
  
```xml
<AbsoluteMonthlyRecurrence>
   <Interval/>
   <DayOfMonth/>
</AbsoluteMonthlyRecurrence>
```

 **AbsoluteMonthlyRecurrencePatternType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DayOfMonth](dayofmonth.md) <br/> |Descreve o dia em um mês em que ocorre um item recorrente. O intervalo de valores para essa propriedade é de 1 a 31. Se for um mês específico, esse valor será maior do que o número de dias no mês, o último dia do mês será assumido para essa propriedade.  <br/> |
|[Intervalo](interval.md) <br/> |Define o intervalo entre dois itens recorrentes consecutivos. Por exemplo, se o elemento **Interval** tem um valor de 5, o item recorrente ocorre a cada 5 meses. O intervalo de valores válidos é de 1 a 99.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Recorrência (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Contém informações de recorrência para tarefas recorrentes.  <br/> |
|[Recurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Contém o padrão de recorrência para itens de calendário e solicitações de reunião.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

