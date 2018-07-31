---
title: Recurrence (TaskRecurrenceType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recurrence
api_type:
- schema
ms.assetid: 99f8414a-9110-4721-a6e5-ebf225d7ed0a
description: O elemento de recorrência contém informações de recorrência de tarefas recorrentes.
ms.openlocfilehash: 0ec43447e47050a0bd483d8441da88e4a7f08923
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354418"
---
# <a name="recurrence-taskrecurrencetype"></a>Recurrence (TaskRecurrenceType)

O elemento de **Recorrência** contém informações de recorrência de tarefas recorrentes. 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <MonthlyRegeneration/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <DailyRegeneration/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
       <DailyRegeneration/> 
       <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <DailyRegeneration/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
       <MonthlyRegeneration/> 
       <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <YearlyRegeneration/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <YearlyRegeneration/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRegeneration/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeYearlyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRegeneration/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <YearlyRegeneration/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeYearlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
       <MonthlyRegeneration/> 
       <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
       <DailyRecurrence/> 
       <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRegeneration/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```


**TaskRecurrenceType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Descreve um padrão de recorrência anual relativa de uma tarefa recorrente.  <br/> |
|[AbsoluteYearlyRecurrence](absoluteyearlyrecurrence.md) <br/> |Representa um padrão de recorrência anual de uma tarefa recorrente.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Descreve um padrão de recorrência mensal relativa de uma tarefa recorrente.  <br/> |
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |Representa um padrão de recorrência mensal para uma tarefa recorrente.  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Descreve a frequência, em semanas e os dias em que é uma tarefa recorrente.  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |Descreve a frequência, em dias, em que é uma tarefa recorrente.  <br/> |
|[DailyRegeneration](dailyregeneration.md) <br/> |Descreve o número de dias após a conclusão da tarefa a próxima ocorrência atual será vencimento.  <br/> |
|[WeeklyRegeneration](weeklyregeneration.md) <br/> |Descreve quantos semanas após a conclusão da tarefa a próxima ocorrência atual será vencimento.  <br/> |
|[MonthlyRegeneration](monthlyregeneration.md) <br/> |Descreve quantos meses após a conclusão da tarefa a próxima ocorrência atual será vencimento.  <br/> |
|[YearlyRegeneration](yearlyregeneration.md) <br/> |Descreve quantos anos após a conclusão da tarefa a próxima ocorrência atual será vencimento.  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |Descreve um padrão de recorrência que não tem uma data de término definidas.  <br/> O uso deste elemento exclui o uso dos elementos [EndDateRecurrence](enddaterecurrence.md) e [NumberedRecurrence](numberedrecurrence.md) .  <br/> |
|[EndDateRecurrence](enddaterecurrence.md) <br/> |Descreve a data de início e a data final do padrão de recorrência de um item.  <br/> O uso deste elemento exclui o uso dos elementos [NoEndRecurrence](noendrecurrence.md) e [NumberedRecurrence](numberedrecurrence.md) .  <br/> [EndDateRecurrence](enddaterecurrence.md) não pode ser usado em conjunto com um padrão de regeneração.  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |Descreve a data de início e o número de ocorrências de um item recorrente.  <br/> O uso deste elemento exclui o uso dos elementos [NoEndRecurrence](noendrecurrence.md) e [EndDateRecurrence](enddaterecurrence.md) .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Task](task.md) <br/> |Representa uma tarefa no armazenamento do Exchange.  <br/> |
   
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

