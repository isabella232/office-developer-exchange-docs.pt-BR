---
title: AbsoluteMonthlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AbsoluteMonthlyRecurrence
api_type:
- schema
ms.assetid: 178fa0ae-9dfc-417f-933c-d657d31c2161
description: O elemento AbsoluteMonthlyRecurrence representa um padrão de recorrência mensal.
ms.openlocfilehash: 7fcc1811a7c42fc653344fb3c052adac820d6a5d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546914"
---
# <a name="absolutemonthlyrecurrence"></a>AbsoluteMonthlyRecurrence

O **elemento AbsoluteMonthlyRecurrence** representa um padrão de recorrência mensal. 
  
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
|[DayOfMonth](dayofmonth.md) <br/> |Descreve o dia em um mês em que ocorre um item recorrente. O intervalo de valores dessa propriedade é de 1 a 31. Se para um determinado mês esse valor for maior do que o número de dias no mês, o último dia do mês será assumido para essa propriedade.  <br/> |
|[Intervalo](interval.md) <br/> |Define o intervalo entre dois itens recorrentes consecutivos. Por exemplo, se o **elemento Interval** tiver um valor 5, o item recorrente ocorrerá a cada 5 meses. O intervalo de valores válidos é de 1 a 99.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Recurrence (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Contém informações de recorrência para tarefas recorrentes.  <br/> |
|[Recurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Contém o padrão de recorrência para itens de calendário e solicitações de reunião.  <br/> |
   
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

