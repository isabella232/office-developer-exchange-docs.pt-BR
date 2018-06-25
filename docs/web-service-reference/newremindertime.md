---
title: NewReminderTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: O elemento NewReminderTime Especifica um novo horário para um lembrete.
ms.openlocfilehash: 9f3f509942c673c916cc646cd9519240aef6ea06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824531"
---
# <a name="newremindertime"></a>NewReminderTime

O elemento **NewReminderTime** Especifica um novo horário para um lembrete. 
  
```XML
<NewReminderTime/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[ReminderItemAction](reminderitemaction.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **NewReminderTime** é um novo horário para o lembrete. O elemento **NewReminderTime** é usado quando o elemento [ActionType](actiontype-reminderactiontype.md) é definir como **Snooze**, a fim de atraso do lembrete. O valor de **NewReminderTime** deve ser maior que o [ReminderTime](remindertime.md) retornado pela [operação de GetReminders](getreminders-operation.md).
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[ReminderItemAction](reminderitemaction.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

