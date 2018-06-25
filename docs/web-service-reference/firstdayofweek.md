---
title: Primeiro_dia_semana
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FirstDayOfWeek
api_type:
- schema
ms.assetid: d6cf1bd3-a19b-4d5f-9e25-8e337a4939e0
description: O elemento Primeiro_dia_semana Especifica o primeiro dia da semana.
ms.openlocfilehash: 99858d17213d077ce7c51ad1c746588f2f3939a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752312"
---
# <a name="firstdayofweek"></a>Primeiro_dia_semana

O elemento **Primeiro_dia_semana** Especifica o primeiro dia da semana. 
  
```XML
<FirstDayOfWeek> Sunday | Monday | Tuesday | Wednesday | Thursday | Friday | Saturday</FirstDayOfWeek>
```

 **DayOfWeekType**
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

O valor de texto do elemento **Primeiro_dia_semana** indica qual dia da semana é usado como o primeiro dia da semana. Estes são os valores de texto possíveis: 
  
- Domingo
    
- Segunda-feira
    
- Terça-feira
    
- Quarta-feira
    
- Quinta-feira
    
- Sexta-feira
    
- Sábado
    
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

