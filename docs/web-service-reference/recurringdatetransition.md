---
title: RecurringDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecurringDateTransition
api_type:
- schema
ms.assetid: 52fe1e05-3c50-40a1-8752-5c3c64c9f1ed
description: O elemento RecurringDateTransition representa uma transição de fuso horário que ocorre em uma data específica a cada ano.
ms.openlocfilehash: 864f3f539c5440fbfc539ca6c2042b3d9edca267
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529360"
---
# <a name="recurringdatetransition"></a>RecurringDateTransition

O **elemento RecurringDateTransition** representa uma transição de fuso horário que ocorre em uma data específica a cada ano. 
  
```xml
<RecurringDateTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <Day/>
</RecurringDateTransition>
```

 **RecurringDateTransitionType**
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
|[Day](day.md) <br/> |Representa o dia do mês em que ocorre a transição de fuso horário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Transitions](transitions.md) <br/> |Representa uma coleção de transições de fuso horário.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Representa uma coleção de transições de fuso horário.  <br/> |
   
## <a name="remarks"></a>Comentários

Um exemplo de uma transição de fuso horário que poderia ser representada pelo [elemento RecurringDateTransition](recurringdatetransition.md) é uma transição que ocorre em 15 de março de cada ano. 
  
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

