---
title: ReminderItemAction
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fe67512c-5b15-4f07-8628-74cf873c2d71
description: O elemento ReminderItemAction especifica a ação de um item de lembrete.
ms.openlocfilehash: 7cd6898bb44ecd442a02f162008225d904396ba0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512461"
---
# <a name="reminderitemaction"></a>ReminderItemAction

O **elemento ReminderItemAction** especifica a ação de um item de lembrete. 
  
```XML
<ReminderItemAction>
   <ActionType></ActionType>
   <ItemId></ItemId>
   <NewReminderTime></NewReminderTime>
</ReminderItemAction>
```

 **ReminderItemActionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[ActionType (ReminderActionType)](actiontype-reminderactiontype.md)  |  [ItemId](itemid.md)  |  [NewReminderTime](newremindertime.md)
  
### <a name="parent-elements"></a>Elementos pai

[ReminderItemActions](reminderitemactions.md)
  
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



[ReminderItemActions](reminderitemactions.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

