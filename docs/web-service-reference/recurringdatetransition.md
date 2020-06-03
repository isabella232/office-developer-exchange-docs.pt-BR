---
title: RecurringDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringDateTransition
api_type:
- schema
ms.assetid: 52fe1e05-3c50-40a1-8752-5c3c64c9f1ed
description: O elemento RecurringDateTransition representa uma transição de fuso horário que ocorre em uma data específica por ano.
ms.openlocfilehash: 2acbd3afb50a92d4e4f3d7b552eecb36fe59be8b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461573"
---
# <a name="recurringdatetransition"></a>RecurringDateTransition

O elemento **RecurringDateTransition** representa uma transição de fuso horário que ocorre em uma data específica por ano. 
  
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
|[To](to.md) <br/> |Especifica o [período](period.md) ou [TransitionsGroup](transitionsgroup.md) que é o destino da transição de fuso horário.  <br/> |
|[Timeoffset](timeoffset.md) <br/> |Representa a diferença de duração do tempo universal coordenado (UTC) para a transição de fuso horário.  <br/> |
|[Month (transição de fuso horário)](month-time-zone-transition.md) <br/> |Representa o mês em que ocorre a transição de fuso horário.  <br/> |
|[Day](day.md) <br/> |Representa o dia do mês em que ocorre a transição de fuso horário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Transições](transitions.md) <br/> |Representa uma coleção de transições de fuso horário.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Representa uma coleção de transições de fuso horário.  <br/> |
   
## <a name="remarks"></a>Comentários

Um exemplo de uma transição de fuso horário que pode ser representada pelo elemento [RecurringDateTransition](recurringdatetransition.md) é uma transição que ocorre em 15 de março a cada ano. 
  
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

