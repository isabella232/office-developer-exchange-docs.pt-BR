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
description: O elemento RecurringDayTransition representa uma transição de fuso horário que ocorre no mesmo dia cada ano.
ms.openlocfilehash: 913345188547ce9903809fdc1cbbbe3e20ae7f36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825012"
---
# <a name="recurringdaytransition"></a>RecurringDayTransition

O elemento **RecurringDayTransition** representa uma transição de fuso horário que ocorre no mesmo dia cada ano. 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[To](to.md) <br/> |Especifica o [período](period.md) ou [TransitionsGroup](transitionsgroup.md) que é o destino da transição fuso horário.  <br/> |
|[TimeOffset](timeoffset.md) <br/> |Representa o deslocamento de duração do tempo Universal Coordenado (UTC) para a transição de fuso horário.  <br/> |
|[Mês (transição de fuso horário)](month-time-zone-transition.md) <br/> |Representa o mês em que ocorre a transição de fuso horário.  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |Representa o dia da semana em que ocorre a transição de fuso horário.  <br/> |
|[Ocorrência (transição de fuso horário)](occurrence-time-zone-transition.md) <br/> |Representa a ocorrência do dia da semana do mês em que ocorre a transição do fuso horário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Transições](transitions.md) <br/> |Representa uma coleção de transições de fuso horário.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Representa uma coleção de transições de fuso horário.  <br/> |
   
## <a name="remarks"></a>Coment�rios

Um exemplo de uma transição de fuso horário que poderia ser representado pelo elemento [RecurringDayTransition](recurringdaytransition.md) é uma transição que ocorre na segunda terça-feira de fevereiro a cada ano. 
  
O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

