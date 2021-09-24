---
title: ActionType (ReminderActionType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0ffcdcf4-8ea3-483c-bb7f-0cd84126120c
description: O elemento ActionType especifica a ação a ser tomada no lembrete.
ms.openlocfilehash: d78725c75ad13a71d69d7749f0a71cd99d606929
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522254"
---
# <a name="actiontype-reminderactiontype"></a>ActionType (ReminderActionType)

O **elemento ActionType** especifica a ação a ser tomada no lembrete. 
  
```XML
<ActionType> Dismiss | Snooze </ActionType>
```

 **ReminderActionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[ReminderItemAction](reminderitemaction.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento ActionType** especifica a ação a ser tomada no lembrete. O valor de texto **de Dismiss** indica que o lembrete deve ser ignorado. O valor de texto **de Snooze** indica que o lembrete deve ser atrasado até o horário especificado pelo [elemento NewReminderTime.](newremindertime.md) 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [ReminderItemAction](reminderitemaction.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

