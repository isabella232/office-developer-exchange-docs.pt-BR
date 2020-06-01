---
title: RecurringDayTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringDayTransition
api_type:
- schema
ms.assetid: 1ae28d14-c2b8-4084-9e76-e2e347a884ce
description: O elemento RecurringDayTransition representa uma transição de fuso horário que ocorre no mesmo dia a cada ano.
ms.openlocfilehash: 44c2a6ec4dbaaa52a2772cb5c35a84b14dd77f97
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468464"
---
# <a name="recurringdaytransition"></a>RecurringDayTransition

O elemento **RecurringDayTransition** representa uma transição de fuso horário que ocorre no mesmo dia a cada ano. 
  
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
|[To](to.md) <br/> |Especifica o [período](period.md) ou [TransitionsGroup](transitionsgroup.md) que é o destino da transição de fuso horário.  <br/> |
|[Timeoffset](timeoffset.md) <br/> |Representa a diferença de duração do tempo universal coordenado (UTC) para a transição de fuso horário.  <br/> |
|[Month (transição de fuso horário)](month-time-zone-transition.md) <br/> |Representa o mês em que ocorre a transição de fuso horário.  <br/> |
|[DayOfWeek (fuso horário)](dayofweek-timezone.md) <br/> |Representa o dia da semana em que ocorre a transição de fuso horário.  <br/> |
|[Ocorrência (transição de fuso horário)](occurrence-time-zone-transition.md) <br/> |Representa a ocorrência do dia da semana no mês em que ocorre a transição de fuso horário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Transições](transitions.md) <br/> |Representa uma coleção de transições de fuso horário.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Representa uma coleção de transições de fuso horário.  <br/> |
   
## <a name="remarks"></a>Comentários

Um exemplo de uma transição de fuso horário que pode ser representada pelo elemento [RecurringDayTransition](recurringdaytransition.md) é uma transição que ocorre na segunda terça-feira de fevereiro por ano. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

