---
title: RelativeYearlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RelativeYearlyRecurrence
api_type:
- schema
ms.assetid: 25b67876-9979-4a30-a637-357ea10a93b8
description: O elemento RelativeYearlyRecurrence descreve um padrão de recorrência anual relativa.
ms.openlocfilehash: ce8d2b134ce1fa34cbce8bd2fa921cab18d908a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825057"
---
# <a name="relativeyearlyrecurrence"></a>RelativeYearlyRecurrence

O elemento **RelativeYearlyRecurrence** descreve um padrão de recorrência anual relativa. 
  
```xml
<RelativeYearlyRecurrence>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
   <Month/>
</RelativeYearlyRecurrence>
```

 **RelativeYearlyRecurrencePatternType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DaysOfWeek (DayOfWeekType)](daysofweek-dayofweektype.md) <br/> |Descreve os dias da semana que são usados em padrões de recorrência do item.  <br/> |
|[DayOfWeekIndex](dayofweekindex.md) <br/> |Descreve qual semana em um mês é usada em um padrão de recorrência anual relativa.  <br/> |
|[Mês (recorrência do Item)](month-item-recurrence.md) <br/> |Descreve o mês quando um item recorrente anual ocorre.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Recorrência (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Contém informações de recorrência de tarefas recorrentes.  <br/> |
|[Recorrência (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Contém o padrão de recorrência para itens de calendário e solicitações de reunião.  <br/> |
|[Standard](standard.md) <br/> |Representa a data e hora de quando o tempo é alterado de horário de verão para a hora padrão.  <br/> |
|[Horário de verão](daylight.md) <br/> |Representa a data e hora de quando o tempo é alterado do período padrão para o horário de verão.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

