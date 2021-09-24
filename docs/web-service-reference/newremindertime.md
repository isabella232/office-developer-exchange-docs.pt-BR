---
title: NewReminderTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: O elemento NewReminderTime especifica uma nova hora para um lembrete.
ms.openlocfilehash: 9e6cb75396f35f606bcd974e374f24957ee5d1ec
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515443"
---
# <a name="newremindertime"></a>NewReminderTime

O **elemento NewReminderTime** especifica uma nova hora para um lembrete. 
  
```XML
<NewReminderTime/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[ReminderItemAction](reminderitemaction.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento NewReminderTime** é uma nova hora para o lembrete. O **elemento NewReminderTime** é usado quando o [elemento ActionType](actiontype-reminderactiontype.md) é definido como **Snooze**, para atrasar o lembrete. O valor do **NewReminderTime** deve ser maior do que [o ReminderTime](remindertime.md) retornado pela [operação GetReminders.](getreminders-operation.md)
  
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



[ReminderItemAction](reminderitemaction.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

