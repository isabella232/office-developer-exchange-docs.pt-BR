---
title: FirstDayOfWeek
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FirstDayOfWeek
api_type:
- schema
ms.assetid: d6cf1bd3-a19b-4d5f-9e25-8e337a4939e0
description: O elemento FirstDayOfWeek especifica o primeiro dia da semana.
ms.openlocfilehash: 1b983cfc27d0e818a0487625b9af8c9e6b0afd93
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545087"
---
# <a name="firstdayofweek"></a>FirstDayOfWeek

O **elemento FirstDayOfWeek** especifica o primeiro dia da semana. 
  
```XML
<FirstDayOfWeek> Sunday | Monday | Tuesday | Wednesday | Thursday | Friday | Saturday</FirstDayOfWeek>
```

 **DayOfWeekType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Descreve um padrão de recorrência semanal.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento FirstDayOfWeek** indica qual dia da semana é usado como o primeiro dia da semana. Veja a seguir os valores de texto possíveis: 
  
- Domingo
    
- Segunda-feira
    
- Terça-feira
    
- Quarta-feira
    
- Quinta-feira
    
- Sexta-feira
    
- Sábado
    
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

