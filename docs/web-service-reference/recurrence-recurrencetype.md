---
title: Recurrence (RecurrenceType)
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
ms.assetid: 3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12
description: O elemento de recorrência contém o padrão de recorrência para itens de calendário e solicitações de reunião.
ms.openlocfilehash: d9c6009e11eb5b66cdd749b8e085935060f99ab7
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353347"
---
# <a name="recurrence-recurrencetype"></a>Recurrence (RecurrenceType)

O elemento de **Recorrência** contém o padrão de recorrência para itens de calendário e solicitações de reunião. 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
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
      <RelativeMonthlyRecurrence/> 
      <NumberedRecurrence/>
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
      <RelativeYearlyRecurrence/> 
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
      <DailyRecurrence/> 
      <NoEndRecurrence/>
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
      <DailyRecurrence/> 
      <EndDateRecurrence/>
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
      <DailyRecurrence/> 
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
      <AbsoluteMonthlyRecurrence/> 
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
      <WeeklyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NumberedRecurrence/> 
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
      <RelativeMonthlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

**RecurrenceType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Descreve um padrão de recorrência anual relativa.  <br/> |
|[AbsoluteYearlyRecurrence](absoluteyearlyrecurrence.md) <br/> |Representa um padrão de recorrência anual.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Descreve um padrão de recorrência mensal relativa para um item de calendário recorrente.  <br/> |
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |Representa um padrão de recorrência mensal.  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Descreve a frequência, em semanas e os dias em um item de calendário ou uma tarefa recorrente.  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |Descreve a frequência, em dias, no qual um item de calendário ou uma tarefa recorrente.  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |Descreve um padrão de recorrência que não tem uma data de término definidas.  <br/> O uso deste elemento exclui o uso dos elementos [EndDateRecurrence](enddaterecurrence.md) e [NumberedRecurrence](numberedrecurrence.md) .  <br/> |
|[EndDateRecurrence](enddaterecurrence.md) <br/> |Descreve a data de início e a data final do padrão de recorrência de um item.  <br/> O uso deste elemento exclui o uso dos elementos [NoEndRecurrence](noendrecurrence.md) e [NumberedRecurrence](numberedrecurrence.md) .  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |Descreve a data de início e o número de ocorrências de um item recorrente.  <br/> O uso deste elemento exclui o uso dos elementos [NoEndRecurrence](noendrecurrence.md) e [EndDateRecurrence](enddaterecurrence.md) .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no armazenamento do Exchange  <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento é válido se [CalendarItemType](calendaritemtype.md) tem o valor de RecurringMaster. 
  
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

