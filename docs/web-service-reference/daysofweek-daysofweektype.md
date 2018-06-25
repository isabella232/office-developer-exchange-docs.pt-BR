---
title: DaysOfWeek (DaysOfWeekType)
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
ms.assetid: c56f997d-28f3-4590-97b0-cb71f016dbe4
description: O elemento DaysOfWeek descreve os dias da semana que são usados em padrões de recorrência do item.
ms.openlocfilehash: 0b730ff5a7bc9aa6b324fc080022d056c5342296
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751713"
---
# <a name="daysofweek-daysofweektype"></a>DaysOfWeek (DaysOfWeekType)

O elemento **DaysOfWeek** descreve os dias da semana que são usados em padrões de recorrência do item. 
  
```XML
<DaysOfWeek/>
```

**DaysOfWeekType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Descreve um padrão de recorrência semanal.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. Veja a seguir os valores possíveis:
  
- Domingo    
- Segunda-feira    
- Terça-feira    
- Quarta-feira    
- Quinta-feira    
- Sexta-feira    
- Sábado    
- Dia (esse valor não é válido para um padrão de recorrência semanal)    
- Weekday (esse valor não é válido para um padrão de recorrência semanal)    
- WeekendDay (esse valor não é válido para um padrão de recorrência semanal)
    
Um padrão de recorrência semanal pode conter vários valores. Valores são separados por um caractere de espaço. Por exemplo, para uma recorrência semanal às terças e quintas-feiras, o valor de texto será "Terça-feira quinta-feira".
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

