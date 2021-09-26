---
title: RecurringDayTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecurringDayTransition
api_type:
- schema
ms.assetid: 1ae28d14-c2b8-4084-9e76-e2e347a884ce
description: O elemento RecurringDayTransition representa uma transição de fuso horário que ocorre no mesmo dia a cada ano.
ms.openlocfilehash: 3b567e5b906ec00bd71deb1c85f8049bb6de8e3b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542880"
---
# <a name="recurringdaytransition"></a>RecurringDayTransition

O **elemento RecurringDayTransition** representa uma transição de fuso horário que ocorre no mesmo dia a cada ano. 
  
```xml
<RecurringDayTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <DayOfWeek/>
   <Occurrence/>
</RecurringDayTransition>
```

 **RecurringDayTransitionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[To](to.md) <br/> |Especifica o [Period ou](period.md) [TransitionsGroup](transitionsgroup.md) que é o destino da transição de fuso horário.  <br/> |
|[TimeOffset](timeoffset.md) <br/> |Representa o deslocamento de duração do UTC (Tempo Universal Coordenado) para a transição do fuso horário.  <br/> |
|[Month (Time Zone Transition)](month-time-zone-transition.md) <br/> |Representa o mês em que ocorre a transição de fuso horário.  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |Representa o dia da semana em que ocorre a transição de fuso horário.  <br/> |
|[Occurrence (Time Zone Transition)](occurrence-time-zone-transition.md) <br/> |Representa a ocorrência do dia da semana no mês em que ocorre a transição de fuso horário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Transitions](transitions.md) <br/> |Representa uma coleção de transições de fuso horário.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Representa uma coleção de transições de fuso horário.  <br/> |
   
## <a name="remarks"></a>Comentários

Um exemplo de transição de fuso horário que poderia ser representado pelo [elemento RecurringDayTransition](recurringdaytransition.md) é uma transição que ocorre na segunda terça-feira de fevereiro de cada ano. 
  
O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

